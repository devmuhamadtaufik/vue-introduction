<template>
  <div class="text-white flex flex-col items-center">
    <div>Ini gambar {{ title }}</div>
    <div
      class="bg-sky-500 rounded w-60 h-80 flex items-center justify-center my-2"
      @click="emits('redirect')"
    >
      <div class="bg-white w-52 h-72">
        <slot name="image"></slot>
      </div>
    </div>
    <div>{{ message }}</div>
  </div>
</template>

<script setup>
import { defineProps, defineEmits } from "vue";

const emits = defineEmits(["redirect"]);
const props = defineProps(["title", "message"]);
</script>
