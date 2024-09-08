<script setup lang="ts">
import githubIcon from '@/assets/icons/github-icon.png';
import linkedinIcon from '@/assets/icons/linkedin-icon.png';

import { LINKEDIN_HINT, GITHUB_HINT } from '@/constants/messages/hints/contact-hints';

defineProps<{
	type: 'linkedin' | 'github';
	link: string;
}>();
</script>

<template>
	<a :href="link" :title="hint" target="blank" class="contact-mean">
		<img :src="icon" alt="Ícone do meio de contato" class="contact-mean-icon" />
	</a>
</template>

<style scoped>
a.contact-mean {
	margin: 1em 2em;
	padding: 2em;
	border-radius: 0.2em;
	transition: background-color 0.2s ease-in;
}

a.contact-mean:hover {
	background: rgba(0, 0, 0, 0.05);
}

img {
	width: 36px;
}
</style>

<script lang="ts">
export default {
	computed: {
		icon() {
			switch (this.type) {
				case 'linkedin':
					return linkedinIcon;
				case 'github':
					return githubIcon;
				default:
					return '';
			}
		},
		hint() {
			switch (this.type) {
				case 'linkedin':
					return LINKEDIN_HINT;
				case 'github':
					return GITHUB_HINT;
				default:
					return '';
			}
		},
	},
};
</script>
