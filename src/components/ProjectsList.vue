<template>
	<section class="projects bg-secondary">
		<div class="container">
			<div class="projects-top text-center mb-3">
				<h2>My Portfolio</h2>
				<p class="text-muted">Most recent projects I have completed</p>
			</div>
			<div class="row">
				<div class="col-4 mb-4" v-for="project in projects">
					<ProjectItem :project="project"/>
				</div>
			</div>
		</div>
	
	</section>
</template>

<script>
	import ProjectItem from './ProjectItem'
	
	export default {
		name: 'ProjectsList',
		components: { ProjectItem },
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
