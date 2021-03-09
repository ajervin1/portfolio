<template>
	<article class="border bg-white shadow-lg rounded">
		<img :src="`./${project.img}`" class="img-fluid  rounded-top">
		<div class="meta text-center p-3">
			<h3 class="h5">{{ project.title }}</h3>
			<p class="text-muted">{{ project.description }}</p>
			<a class="btn btn-success  w-50" :href="`${project.url}`">View</a>
		</div>
	
	</article>
</template>

<script>
	export default {
		name: 'ProjectItem',
		props: [ 'project' ]
		
	}
</script>
