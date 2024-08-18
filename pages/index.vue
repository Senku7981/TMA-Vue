<template>
	<div class="index">
		the Index page
		{{ webApp.initData }}
	</div>
</template>

<script setup lang="ts">
import { useWebApp } from 'vue-tg';

defineOptions({ name: 'Index' });

const webApp = useWebApp();
</script>

<style scoped></style>
