<template>
	<div id="app" class="container">
		<NavBar  class="mb-4"/>
		<About  class="mb-4"/>
		<Projects />
	</div>
</template>

<script>
	
	
	import NavBar from './components/NavBar'
	import About from './components/About'
	import Footer from './components/Footer'
	import Projects from './components/Projects'
	export default {
		name: 'App',
		components: { Projects, Footer,   About, NavBar },
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
