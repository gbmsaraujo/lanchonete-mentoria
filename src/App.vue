<template>
	<h1 class="titulo">{{ title }}</h1>
	<div id="ct-components">
		<realizar-pedido />
	</div>
</template>

<script>
	import RealizarPedido from "./components/RealizarPedido.vue";

	export default {
		name: "App",
		components: {
			RealizarPedido
		},
		data() {
			return {
				title: "Projeto Lanchonete Mentoria"
			};
		}
	};
</script>

<style scoped>
	.titulo {
		@apply text-lg bg-red-300 text-center p-4;
	}
</style>
