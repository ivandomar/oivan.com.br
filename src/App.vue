<script setup lang="ts">
import { RouterView } from 'vue-router';
import HelloWorld from './components/HelloWorld.vue';
</script>

<template>
	<div class="wrapper">
		<HelloWorld msg="You did it!" />
	</div>

	<RouterView />
</template>

<style scoped>
header {
	line-height: 1.5;
	max-height: 100vh;
}
</style>
