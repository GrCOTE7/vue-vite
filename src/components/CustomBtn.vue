<script setup>
defineProps({
	actionBtn: String,
});
</script>

<template>
	My Btn
	<button @click="console.log(actionBtn)">
		{{ actionBtn ?? 'ooo' }}
	</button>
	<slot>Default msg</slot>
</template>
