<script lang="ts" setup>
import { MainButton, useWebAppPopup } from 'vue-tg';

import { useWebApp } from 'vue-tg';

const { showAlert } = useWebAppPopup();
const webApp = useWebApp();
</script>

<template>
	{{ webApp.initData }}
	platform
	{{ webApp.version }}
	init Data
	{{ webApp.initDataUnsafe }}
	<MainButton text="Open alert" @click="() => showAlert('Hello!')" />
</template>
