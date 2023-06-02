<script setup lang="ts">

import CustomBtn from './components/CustomBtn.vue'

const title = "My App";

</script>

<template>
	
	<div class="app">
		<h1 class="blue">{{ title }}</h1>
		<p class="justify">
			Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quam sed
			explicabo possimus cum doloremque culpa fugit, animi at amet libero ullam
			temporibus quaerat, in deserunt.
		</p>
		
		<CustomBtn actionBtn = "Test !"/>
	</div>
	
</template>
