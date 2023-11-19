<script setup lang='ts'>
import PDFViewer from './PDFViewer.vue';
import example from './example.pdf'
</script>

<template>
  <div style="display: flex;justify-content: center;
  align-items: center;height: 100vh;">
    <PDFViewer :src="example" />
  </div>
</template>
