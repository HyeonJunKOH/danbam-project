<template>
  <div>
    <DanBamHeader></DanBamHeader>
    <DanBamBody></DanBamBody>
    <DanBamNav></DanBamNav>
    <DanBamChap></DanBamChap>
  </div>
</template>

<script>
import DanBamHeader from './components/DanBamHeader.vue'
import DanBamBody from './components/DanBamBody.vue'
import DanBamNav from './components/DanBamNav.vue';
import DanBamChap from './components/DanBamChap.vue';

  export default {
    components: {
    DanBamHeader,
    DanBamBody,
    DanBamNav,
    DanBamChap
}
  }
</script>

<style scoped>

</style>
