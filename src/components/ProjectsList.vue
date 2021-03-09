<template>
	<section class="projects bg-gray-300">
		<div class="container">
			<div class="projects-top text-center mb-3">
				<h2>My Portfolio</h2>
				<p class="text-gray-600">Most recent projects I have completed</p>
			</div>
			<div class="row">
				<div class="col-md-4 mb-4" v-for="project in projects">
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
						title: 'Instagram Clone',
						img: require('@/images/insta.png'),
						description: 'Search Users, View User Images or Videos',
						url: 'https://instascraper.netlify.app/'
					},
					{
						title: 'Tiktok Clone',
						img: require('@/images/tiktok.png'),
						description: 'Search Users and view their TikTok posts',
						url: 'https://tiktock.netlify.app/'
					},
				
					{
						title: 'Twitch Clips',
						img: require('@/images/twitch.png'),
						description: 'View Twitch\'s top clips',
						url: 'https://twitchy.netlify.app/'
					},
			
					{
						title: 'Business Landing Page',
						img: require('@/images/landing.png'),
						description: 'Landing Page For A Local Business',
						url: 'https://ajlanding.netlify.app/'
					}
				]
			}
		}
	}
</script>
