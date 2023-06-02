<script setup>
import HelloWorld from "./components/HelloWorld.vue";
import Gc7 from "./components/Gc7.vue";
import Card from "./components/Card.vue";
</script>

<template>

	<div class="app">
		
		<Card>
			<template v-slot:title>
			<h3>Un Autre Titre de Card direct depuis App</h3>
		</template>
		</Card>
		
		<Gc7 msg="Gc7 Card Depuis App" />
		
		<HelloWorld msg="HelloWorld: Vite + Vue" />
	</div>


</template>
