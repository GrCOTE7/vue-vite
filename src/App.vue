<script setup>
import CustomBtn from "./components/CustomBtn.vue";

const title = "My App";

const info = "Hello !"

// const infoProps = [{ descr: "descr" }, { status: "infodescr" }];
</script>
<script>
// export default {
// 	components: {
// 		CustomBtn,
// 	},
// 	data() {
// 		return {
// 			info: "Hello World!",
// 		};
// 	},
// };
</script>

<template>
	<div class="app">
		<h1 class="blue">{{ title }}</h1>
		<p class="justify">
			Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quam sed
			explicabo possimus cum doloremque culpa fugit, animi at amet libero ullam
			temporibus quaerat, in deserunt.
		</p>
		
		{{ info }} (dans parent)
		<hr>
		
		<custom-btn actionBtn="Yes !" :info="info">
			<br />Parent says : → console.log('Yes !')
		</custom-btn>
	</div>
</template>
