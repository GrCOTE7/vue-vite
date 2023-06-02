<script setup>
import { ref, watch } from "vue";
import Card from "./Card.vue";

defineProps({
	msg: String,
});

const count = ref(7);

watch(count, cl);

function cl(count) {
	console.log("gc7", count);
}
</script>

<template>
	<div class="blue">
		
		<h2>{{ msg }}</h2>
		
		<div class="card">
		<button type="button" @click="count++">count is {{ count }}</button>
		
	</div>
	
	<card>
		<template v-slot:title>
			<h3>Un Autre Titre de Carte dans Gc7.vue</h3>
		</template>
		<p>Un autre contenu de carte dans Gc7.vue</p>
	</card>
</div>
	
</template>

<style scoped>
a {
	will-change: filter;
	transition: filter 300ms;
}

a:hover {
	filter: drop-shadow(0 0 0.7em #000562aa);
}
</style>
