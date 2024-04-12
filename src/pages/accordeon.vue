<script setup lang="ts">
import { ref } from 'vue'
const maVar = ref(true)
const maVar2 = ref(1)
</script>

<template>
<p>Page Accordéon</p>
<p>la variable vaut : {{ maVar }}</p>

<button @click="maVar = false">Cacher</button>

<button @click="maVar = true">Montrer</button>

<button @click="maVar = !maVar">Bascule</button>

<button @click="maVar == 1" class="text-2xl"> Montrer 1 </button>
<h1 v-show="maVar == 2" class="text-2xl"> Contenu 1 </h1>

<button click@="maVar2 = false ? 0 : 1 "> </button>

  <h1 v-show="maVar2" class="text-2xl">Bonjour tout le monde !</h1>
</template>
