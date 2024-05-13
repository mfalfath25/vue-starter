<script setup lang="ts">
import { ref } from 'vue'

defineProps<{ msg: string }>()

const count = ref(0)
</script>

<template>
  <div
    class="flex h-screen flex-col items-center justify-center gap-2 bg-slate-200"
  >
    <h1>{{ msg }}</h1>

    <div>
      <button
        class="rounded-lg bg-slate-800 p-2 text-white"
        type="button"
        @click="count++"
      >
        count is {{ count }}
      </button>
    </div>
  </div>
</template>

<style scoped></style>
