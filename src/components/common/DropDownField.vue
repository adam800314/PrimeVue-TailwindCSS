<template>
  <div class="card flex justify-center">
    <Dropdown
      v-model="selectedCity"
      :options="cities"
      optionLabel="name"
      placeholder="Select a City"
      class="w-full md:w-[14rem]"
    />
  </div>
</template>

<script setup>
import { ref } from "vue";

const selectedCity = ref();
import Dropdown from "primevue/dropdown";

const cities = ref([
  { name: "New York", code: "NY" },
  { name: "Rome", code: "RM" },
  { name: "London", code: "LDN" },
  { name: "Istanbul", code: "IST" },
  { name: "Paris", code: "PRS" },
]);
</script>
