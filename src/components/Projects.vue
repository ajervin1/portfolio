<template>
	<main class="projects mb-5">
		<h2 class="text-secondary mb-4">Projects</h2>
		<div class="row">
			<div class="col-4" v-for="project in projects">
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
						img: require('@/images/yt.jpg'),
						description: 'Download Youtube Videos and convert them to mp3 or mp4',
						url: 'https://ytconverter.netlify.app/'
					},
					{
						title: 'Twitch Clips',
						img: require('@/images/twitch.jpg'),
						description: 'View all of Twitch\'s top clips',
						url: 'https://twitchy.netlify.app/'
					},
					{
						title: 'Reddit Clone',
						img: require('@/images/reddit.jpg'),
						description: 'View Popular Subreddits and corresponding posts',
						url: 'https://ajreddit.netlify.app/'
					}
				]
			}
		}
	}
</script>
