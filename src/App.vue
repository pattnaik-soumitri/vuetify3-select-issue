<template>
<v-app>
  <v-container>

    <v-select 
      :items="['Apple', 'Orange']"
      label="Pick a fruit"
      v-model="fruit"
      @change="() => console.log('It Works!')"
    />

    You have selected: {{fruit}}
  </v-container>
</v-app>
</template>

<script setup>
import { ref } from 'vue';

// The v-model
const fruit = ref();

</script>
