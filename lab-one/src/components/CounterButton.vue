<template>
    <button @click="$event => count++">{{ count }}</button>
</template>

<script setup>
import {ref} from "vue";
const count = ref(0)
</script>