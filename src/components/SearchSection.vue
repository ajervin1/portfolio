<template>
	
	<div class="bg-gray-900 p-5 text-white flex justify-between items-center">
		<div class="left-column flex items-center">
			<div class="mr-3">
				<input type="search" placeholder="Search" class="px-2 py-3 w-64 rounded"/>
			</div>
			<div>
				<span>within 50 miles of Michigan</span>
			</div>
		</div>
		<div class="right-column">
			<button class="px-6 py-2 border border-gray-600 mr-2">Groups</button>
			<button class="px-6 py-2 bg-gray-600">Calendar</button>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'SearchSection',
		data () {
			return {}
		}
	}
</script>
