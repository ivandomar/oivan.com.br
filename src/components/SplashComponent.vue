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
	font-size: 25vw;
	line-height: 25vw;
	letter-spacing: 8vw;
	text-align: center;
	margin-right: -8vw;
}

h2 {
	color: #555;
	text-align: center;
	font-size: 2vw;
	letter-spacing: 0.7rem;
	margin-right: -0.7vw;
}

@media screen and (max-width: 767px) {
	h1 {
		font-size: 30vw;
		letter-spacing: 8vw;
		line-height: 30vw;
	}
}
</style>
