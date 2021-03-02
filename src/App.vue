<template>
	<div id="app">
		<NavBar />
	
			<Hero class="pt-32" />
			<ProjectsList class="pt-7" />
	
	</div>
</template>

<script>
	
	

	import Hero from './components/Hero'
	import ProjectsList from './components/ProjectsList'
	import NavBar from './components/NavBar'
	export default {
		name: 'App',
		components: { NavBar, ProjectsList, Hero },
		data(){
			return {
			
			}
		}
	}
</script>

<style lang="scss">
	.container {
		max-width: 90%;
	}
</style>
