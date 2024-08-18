<template>
	<div class="application">
		<nuxt-layout>
			<nuxt-page />
		</nuxt-layout>
		<ClientOnly>
			<MiniApp />
		</ClientOnly>
	</div>
</template>

<script lang="ts" setup>
import MiniApp from '@main/MiniApp.vue';

defineOptions({ name: 'Application' });
</script>
