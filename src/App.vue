<script setup>
import Frame from "./components/Frame.vue";

function redirectToMain() {
  window.location.href = "https://blue.kumparan.com/image/upload/v1634025439/01gkk38w81p6gf02yzv7zzkep7.jpg";
}
</script>

<template>
  <Frame
    class="text-black"
    title="ikan mas"
    message="Ikan mas adalah ikan yang berwarna emas"
    @redirect="redirectToMain"
  >
    <template #image>
      <img
        src="https://blue.kumparan.com/image/upload/v1634025439/01gkk38w81p6gf02yzv7zzkep7.jpg"
        class="h-full object-cover object-right"
      />
    </template>
  </Frame>
</template>
