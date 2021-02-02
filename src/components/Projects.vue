<template>
	<main class="projects mb-5">
		<h2 class="text-secondary mb-4">Projects</h2>
		<div class="row">
			<div class="col-12 col-md-4 mb-5" v-for="project in projects">
				<article class="card h-100">
					<img :src="project.img" class="card-img-top">
					<div class="card-body">
						<h6>
							{{ project.title }}
						</h6>
						<p>
							{{ project.description }}
						</p>
						<a class="btn btn-primary btn-sm" :href="project.url">View Project</a>
					</div>
				</article>
			</div>
		</div>
	
	</main>
</template>

<script>
	export default {
		name: 'Projects',
		data () {
			return {
				projects: [
					{
						title: 'Youtube Converter',
						img: require('@/images/youtube.png'),
						description: 'Download Youtube Videos and convert them to mp3 or mp4',
						url: 'https://ytconverter.netlify.app/'
					},
					{
						title: 'Twitch Clips',
						img: require('@/images/twitch.png'),
						description: 'View all of Twitch\'s top clips',
						url: 'https://twitchy.netlify.app/'
					},
					{
						title: 'Tiktok Clone',
						img: require('@/images/tiktok.png'),
						description: 'View TikTok Posts and Search Tiktok\'s',
						url: 'https://tiktock.netlify.app/'
					},
					{
						title: 'Business Landing Page',
						img: require('@/images/landing.png'),
						description: 'Landing Page For Local Business',
						url: 'https://ajlanding.netlify.app/'
					}
				]
			}
		}
	}
</script>
