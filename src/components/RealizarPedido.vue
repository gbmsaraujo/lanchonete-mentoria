<template>
	<div></div>
</template>

<script>
	import { v4 as uuid } from "uuid";
	export default {
		name: "RealizarPedido",
		props: {},
		data() {
			return {

				molhos: [
					{
						id: uuid(),
						molho: "ketchup",
						descricao: "molho de ketchup",
						img: "@/assets/molhos/ketchup.png",
						preco: 0.5
					},
					{
						id: uuid(),
						molho: "mostarda",
						descricao: "molho de mostarda",
						img: "@/assets/molhos/mostarda.png",
						preco: 0.5
					},
					{
						id: uuid(),
						molho: "maionese",
						descricao: "molho de maionese",
						img: "@/assets/molhos/maionese.png",
						preco: 0.5
					}
				],
				saladas: [
					{
						id: uuid(),
						salada: "alface",
						descricao: "salada tipo alface",
						img: "@/assets/saladas/alface.png",
						preco: 1.0
					},
					{
						id: uuid(),
						salada: "tomate",
						descricao: "salada tipo tomate",
						img: "@/assets/saladas/tomate.png",
						preco: 1.0
					},
					{
						id: uuid(),
						molho: "pimentao",
						descricao: "salada tipo pimentao",
						img: "@/assets/saladas/pimentao.png",
						preco: 1.0
					},
					{
						id: uuid(),
						molho: "azeitona",
						descricao: "salada tipo azeitona",
						img: "@/assets/saladas/azeitona.png",
						preco: 1.0
					}
				],
				acompanhamentos: [
					{
						id: uuid(),
						acompanhamento: "batata-frita",
						img: "@/assets/acompanhamentos/batata-frita.png",
						preco: 5.0
					},
					{
						id: uuid(),
						acompanhamento: "nuggets",
						img: "@/assets/acompanhamentos/nuggets.png",
						preco: 5.0
					},
					{
						id: uuid(),
						acompanhamento: "sorvete",
						img: "@/assets/acompanhamentos/sorvete.png",
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

<style></style>
