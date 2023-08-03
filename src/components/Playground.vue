<template>
  <div>
    <Datepicker v-model="date" inline />
  </div>
</template>

<script setup>
import { ref, computed } from 'vue';
import Datepicker from '@vuepic/vue-datepicker';
import '@vuepic/vue-datepicker/dist/main.css';

const date = ref();
const isDelivery = ref(false);
const allowedDates = computed(() => {
  if (delivery.value)
    return ['2023-08-11T00:00:00+02:00', '2023-08-10T00:00:00+02:00'];
  else return ['2023-08-09T00:00:00+02:00'];
});
</script>
a
