<script setup>
defineProps({
	actionBtn: String,
});
</script>

<template>
	My Btn
	<button @click="console.log(actionBtn)">
		{{ actionBtn ?? 'ooo' }}
	</button><br>
	<slot>Default slot</slot><br>
	<slot name="actionDescr">Default actionDescr</slot>
</template>
