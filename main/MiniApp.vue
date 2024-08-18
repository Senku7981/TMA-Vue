<script lang="ts" setup>
import { MainButton, useWebAppPopup, useWebApp } from 'vue-tg';

const { showAlert } = useWebAppPopup();
const webApp = useWebApp();

webApp.sendData;
</script>

<template>
	<MainButton text="Open alert" @click="() => showAlert('Hello!')" />
</template>
