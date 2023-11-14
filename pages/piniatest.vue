<template>
  <nav>
    <NuxtLink to="/piniatest2">piniatest2</NuxtLink>
  </nav>
  <div>
    <input type="button" @click="store.increment()" value="increment" />
    {{ store.count }}
    {{ store.doubleCount }}
  </div>
</template>

<script setup lang="ts">
import { useCounterStore } from "../stores/counter";

const store = useCounterStore();
</script>

<style scoped></style>
