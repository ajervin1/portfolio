<template>
	<main class="about">
		<!--Row-->
		<section class="row">
			<!--Text-->
			<div class="col-7">
				<article class="about-text-container">
					<h2 class="mb-1 text-primary font-weight-medium display-4 mb-0">Anthony Ervin</h2>
					<small class="mb-2 d-inline-block font-size-lg">Software Developer</small>
					<p class="lead text-secondary line-height-h2">
						Vue.js/Node.js Devloper based in Phoenix, Arizona. I specialize in frontend
						development and enjoy working on applications that communicate with various
						apis.
						I've been working on a lot of exciting projects and I'm ready for new ones.
					</p>
				</article>
			</div>
			<!--Text-->
			<!--Image-->
			<div class="col-5 d-flex justify-content-end">
				<div class="image-container">
					<img class="rounded-circle shadow-lg"
					     src="../images/profile.jpg"
					/>
				</div>
			
			</div>
			<!--Image-->
		</section>
		<!--Row-->
	</main>
</template>

<script>
	export default {
		name: 'About',
		data () {
			return {}
		}
	}
</script>
<style>
	.image-container {
		width: 300px;
		
	}
</style>
