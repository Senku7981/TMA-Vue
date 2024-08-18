<script lang="ts" setup>
import { MainButton, useWebAppPopup } from 'vue-tg';

import { useWebApp } from 'vue-tg';

const { showAlert } = useWebAppPopup();
const webApp = useWebApp();
</script>

<template>
	{{ webApp.initData }}
	<MainButton text="Open alert" @click="() => showAlert('Hello!')" />
</template>
