<script setup lang="ts">
defineProps<{
	type: 'linkedin' | 'github';
	link: string;
}>();
</script>

<template>
	<a :href="link" target="blank" class="contact-mean">
		<img :src="icon" alt="Ícone do meio de contato" class="contact-mean-icon" />
	</a>
</template>

<style scoped></style>

<script lang="ts">
export default {
	computed: {
		icon() {
			switch (this.type) {
				case 'linkedin':
					return '@/assets/icons/linkedin-icon.png';
				case 'github':
					return '@/assets/icons/github-icon.png';
				default:
					return '';
			}
		},
	},
};
</script>
