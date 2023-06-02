<script setup>
defineProps({
	actionBtn: String,
});
</script>

<template>
	My Btn
	<button @click="console.log('Yes !')">
		{{ actionBtn ?? 'ooo' }}
	</button>
</template>
