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
header {
	line-height: 1.5;
	max-height: 100vh;
}
</style>
