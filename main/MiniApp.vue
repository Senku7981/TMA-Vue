<script lang="ts" setup>
import { MainButton, useWebAppPopup, useWebApp } from 'vue-tg';

const { showAlert } = useWebAppPopup();
const webApp = useWebApp();
</script>

<template>
	<MainButton text="Open alert" @click="() => showAlert(webApp.initData)" />
</template>
