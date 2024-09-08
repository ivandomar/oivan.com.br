<script setup lang="ts">
defineProps<{
	title: string;
	subtitle: string;
}>();
</script>

<template>
	<div id="splash-wrapper">
		<h1>{{ title }}</h1>
		<h2>{{ subtitle }}</h2>
	</div>
</template>

<style scoped>
#splash-wrapper {
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
}

h1 {
	position: relative;
	color: #222;
	text-align: center;
	font-weight: bolder;
	font-size: 20rem;
	line-height: 20rem;
	letter-spacing: 5rem;
}

h2 {
	color: #555;
	text-align: center;
	font-size: 2rem;
	letter-spacing: 1rem;
}
</style>
