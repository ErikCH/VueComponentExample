<template>
  <div class="flex items-center justify-center">
    <h2
      class="w-1/2 h-32 text-3xl text-green-800 border-green-800 shadow-outline"
    >
      <!-- {{ $erik }} -->
      {{ message }}
      <span>Child</span>
      <div class="text-2xl italic font-bold">Received: {{ message }}</div>
    </h2>
  </div>
</template>

<script>
import { mapGetters } from "vuex";
export default {
  //   props: ["message"],
  computed: {
    ...mapGetters({ message: "getMessage" })
  }
};
</script>

<style scoped></style>
