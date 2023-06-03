<script setup>
defineProps({
	actionBtn: String,
	info: String,
});
// console.log(this.info)
</script>

<template>
	My Btn
	<button @click="console.log(actionBtn)">
		{{ actionBtn ?? "ooo" }}</button
	><br />

	<hr>
	<hr>
	{{ info }} (dans enfant)
	<!--
	-->
</template>
