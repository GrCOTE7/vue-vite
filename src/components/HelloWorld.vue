<script setup>

import { ref, watch } from "vue";
import Gc7 from './Gc7.vue'
import card from "./Card.vue";

defineProps({
	msg: String,
});

const count = ref(0);

watch(count, cl);

function cl(count) {
	console.log('helloworld', count);
}

</script>

<template>

	<h2>{{ msg }}</h2>

	<div class="card">
		<button type="button" @click="count++">count is {{ count }}</button>
	</div>
	
	<card>
		<template v-slot:title>
			<h3>Un Titre de Carte from HelloWorld</h3>
		</template>
		<p>Un autre contenu de carte from HelloWorld</p>
	</card>
	
	<card>
		<template v-slot:title>
			<h3>Un autre Titre de Carte from HelloWorld</h3>
			<p>Sans content for slot</p>
		</template>
	</card>
	
	<Gc7 msg="Gc7.vue in HelloWorld">
		<slot name="Card">Gc7 Vue</slot>
	</Gc7>
	
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
