<template>
 <div>
  <h1 class="titulo">{{title}}</h1>
 </div>
</template>

<script>

export default {
  name: 'App',
  components: {

  },
  data(){
    return{
      title:"Projeto Lanchonete Mentoria",
    }
  }

}
</script>

<style scoped>
  .titulo{
    @apply text-lg bg-red-300 text-center p-4
  }
</style>
