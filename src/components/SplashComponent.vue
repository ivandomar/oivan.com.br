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
	height: 100vh;
	flex-direction: column;
	justify-content: center;
	align-items: center;
}

h1 {
	font-weight: bolder;
	font-size: 2.6rem;
	position: relative;
	top: -10px;
}
</style>
