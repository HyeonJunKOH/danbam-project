<template>
  <div>
    <DanBamHeader></DanBamHeader>
    <DanBamBody></DanBamBody>
    <DanBamNav></DanBamNav>
  </div>
</template>

<script>
import DanBamHeader from './components/DanBamHeader.vue'
import DanBamBody from './components/DanBamBody.vue'
import DanBamNav from './components/DanBamNav.vue';

  export default {
    components: {
    DanBamHeader,
    DanBamBody,
    DanBamNav
}
  }
</script>

<style scoped>

</style>
