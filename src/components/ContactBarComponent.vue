<script setup lang="ts">
import ContactMeanComponent from './ContactMeanComponent.vue';
</script>

<template>
	<div id="contact-bar">
		<ContactMeanComponent type="linkedin" link="https://linkedin.com/in/ivancezanne" />
		<ContactMeanComponent type="github" link="https://github.com/ivandomar" />
	</div>
</template>

<style scoped>
#contact-bar {
	position: relative;
	display: flex;
	justify-content: center;
	align-items: baseline;
	margin-top: 5rem;
}
</style>
