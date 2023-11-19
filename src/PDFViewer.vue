<script setup lang='ts'>
import { onMounted, ref } from 'vue';

const props = withDefaults(
  defineProps<{
    width: string,
    height: string,
    src: string | BlobPart
  }>(),
  {
    width: "100%",
    height: "100%",
    src: ''
  }
)
const pdfUrl = ref<string>()
onMounted(() => {
  if (typeof props.src === 'string') {
    pdfUrl.value = props.src
  } else {
    pdfUrl.value = window.URL.createObjectURL(new Blob([props.src]))
  }
})

</script>

<template>
  <iframe v-bind="props" :src="`./pdfjs/web/viewer.html?file=${props.src}`" frameborder="0"></iframe>
</template>

<style scoped  lang='less'></style>