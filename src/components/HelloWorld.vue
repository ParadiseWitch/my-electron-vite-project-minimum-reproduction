<script setup lang="ts">

defineProps<{ msg: string }>()

const openBrowser = async () => {
  window.ipcRenderer.send('openBrowser')
}
</script>

<template>
  <div class="card">
    <button type="button" @click="openBrowser" >openBrowser</button>
  </div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
