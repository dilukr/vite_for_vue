<template>
  <div>{{ readersNumber }} {{ book.title }}</div>
</template>

<script>


import { h, ref, reactive } from 'vue';
import { onMounted, onUpdated, onUnmounted } from 'vue';

export default {
  setup() {
    onMounted(() => {
      console.log('mounted!')
    })
    onUpdated(() => {
      console.log('updated!')
    })
    onUnmounted(() => {
      console.log('unmounted!')
    })
    const readersNumber = ref(110)
    const book = reactive({ title: 'Vue 3 Guide' })
    // 请注意，我们需要在这里显式地暴露ref值
    return () => h('div', [readersNumber.value, book.title])
  }
}
</script>
