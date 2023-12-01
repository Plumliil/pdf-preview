<script setup lang='ts'>
import PDFViewer from './PDFViewer.vue';
import example from './example.pdf'
</script>

<template>
  <div style="display: flex;justify-content: center;
  align-items: center;height: 100vh;width: 100vw;">
    <PDFViewer :src="example" />
  </div>
</template>

<style>
* {
  margin: 0;
  padding: 0;
}
</style>
