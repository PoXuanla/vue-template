<template>
  <div>
    <h1 class="text-3xl font-bold underline">Tailwind</h1>
    <hello-world msg="Vite + Vue" />
    {{ result }}
  </div>
</template>

<script setup lang="ts">
const item1 = ref(0);
const item2 = ref(2);
const item3 = ref(4);
const item4 = ref(6);
const item5 = ref(8);
const list = [item1, item2, item3, item4, item5];
const result = useArrayEvery(list, (i) => i % 2 === 0);
// result.value: true
// result.value: false
</script>

<style scoped></style>
