<template>
	<div id="app" class="">
		<NavBar/>
		
		<Hero class="py-20"/>
		<ProjectsList class="pt-7 pb-7"/>
	
	</div>
</template>

<script>
	
	
	
	import Hero from './components/Hero'
	import ProjectsList from './components/ProjectsList'
	import NavBar from './components/NavBar'
	
	export default {
		name: 'App',
		components: { NavBar, ProjectsList, Hero },
		data () {
			return {}
		}
	}
</script>

<style lang="scss">
	.container {
		max-width: 90%;
	}
</style>
