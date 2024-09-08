<script setup lang="ts">
import { RouterView } from 'vue-router';
import ContactBarComponent from './components/ContactBarComponent.vue';
import SplashComponent from './components/SplashComponent.vue';
</script>

<template>
	<div class="wrapper">
		<SplashComponent title="o ivan" subtitle="engenheiro de software + soluções digitais" />

		<RouterView />

		<ContactBarComponent />
	</div>
</template>

<style scoped>
.wrapper {
	position: relative;
	display: flex;
	flex-direction: column;
	justify-content: center;
	height: 100vh;
}
</style>
