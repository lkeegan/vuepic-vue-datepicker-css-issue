<template>
  <div>
    <Datepicker v-model="date" :enable-time-picker="false" :start-date="new Date(1980, 1, 1)" :prevent-min-max-navigation="true" :hide-navigation="['month', 'year', 'calender', 'time']" no-today inline :auto-apply="true" :keep-action-row="false" :flow="['year', 'month', 'calendar']" style="width: 400pt; padding-left: 10pt"/>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import Datepicker from '@vuepic/vue-datepicker';
import '@vuepic/vue-datepicker/dist/main.css';

const date = ref();
</script>
