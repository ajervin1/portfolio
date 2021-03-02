<template>
	<article class="border bg-white shadow-lg rounded">
		<img :src="`./${project.img}`" class="">
		<div class="meta text-center p-3">
			<h3 class="h5">{{ project.title }}</h3>
			<p class="text-muted">{{ project.description }}</p>
			<a class="btn btn-primary w-50 btn-sm" :href="`./${project.url}`">View</a>
		</div>
	
	</article>
</template>

<script>
	export default {
		name: 'ProjectItem',
		props: [ 'project' ]
		
	}
</script>
