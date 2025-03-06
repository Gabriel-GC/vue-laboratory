<script setup>
import CoffeePlan from './components/CoffeePlan.vue';
import { ref } from 'vue';

const plans = ref(['Sozinho', 'Acompanhado', 'Aventureiro', 'Viciado', 'Familiar'])
</script>

<template>
  <div class="content">
    <h1 class="title">Coffee Plans</h1>

    <h2 class="subtitle">Viajamos pelo mundo para encontrar o melhor café de origem única para você</h2>

    <div class="plans">
      <CoffeePlan v-for="plan in plans" :key="plan" :name="plan"></CoffeePlan>
    </div>

  </div>
</template>
