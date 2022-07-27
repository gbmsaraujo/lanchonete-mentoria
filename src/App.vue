<template>
	<h1 class="titulo">{{ title }}</h1>
	<div id="ct-components">
		<realizar-pedido
		/>
	</div>
</template>

<script>
	import RealizarPedido from "./components/RealizarPedido.vue";
	import { v4 as uuid } from "uuid";

	export default {
		name: "App",
		components: {
			RealizarPedido
		},
		data() {
			return {
				title: "Projeto Lanchonete Mentoria",
					molhos: [
					{
						id: uuid(),
						molho: "ketchup",
						descricao: "molho de ketchup",
						imgSrc: require("@/assets/molhos/ketchup.png"),
						preco: 0.5
					},
					{
						id: uuid(),
						molho: "mostarda",
						descricao: "molho de mostarda",
						imgSrc: require("@/assets/molhos/mostarda.png"),
						preco: 0.5
					},
					{
						id: uuid(),
						molho: "maionese",
						descricao: "molho de maionese",
						imgSrc: require("@/assets/molhos/maionese.png"),
						preco: 0.5
					}
				],
				saladas: [
					{
						id: uuid(),
						salada: "alface",
						descricao: "salada tipo alface",
						imgSrc: require("@/assets/saladas/alface.png"),
						preco: 1.0
					},
					{
						id: uuid(),
						salada: "tomate",
						descricao: "salada tipo tomate",
						imgSrc: require("@/assets/saladas/tomate.png"),
						preco: 1.0
					},
					{
						id: uuid(),
						molho: "pimentao",
						descricao: "salada tipo pimentao",
						imgSrc: require("@/assets/saladas/pimentao.png"),
						preco: 1.0
					},
					{
						id: uuid(),
						molho: "azeitona",
						descricao: "salada tipo azeitona",
						imgSrc: require("@/assets/saladas/azeitona.png"),
						preco: 1.0
					}
				],
				acompanhamentos: [
					{
						id: uuid(),
						acompanhamento: "batata-frita",
						imgSrc: require("@/assets/acompanhamentos/batata-frita.png"),
						preco: 5.0
					},
					{
						id: uuid(),
						acompanhamento: "nuggets",
						imgSrc: require("@/assets/acompanhamentos/nuggets.png"),
						preco: 5.0
					},
					{
						id: uuid(),
						acompanhamento: "sorvete",
						imgSrc: require("@/assets/acompanhamentos/sorvete.png"),
						preco: 2.0
					}
				],
				bebidas: [
					{ id: uuid(), bebida: "Coca-Cola Lata", preco: 4.0 },
					{ id: uuid(), bebida: "Heineken Long Neck", preco: 7.0 },
					{ id: uuid(), bebida: "Água sem Gás", preco: 2.0 },
					{ id: uuid(), bebida: "Ice Tea", preco: 4.0 }
				],
			};
		}
	};
</script>

<style scoped>
	.titulo {
		@apply text-lg bg-red-300 text-center p-4;
	}
</style>
