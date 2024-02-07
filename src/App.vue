<template>
  <div>
    <DanBamHeader></DanBamHeader>
    <DanBamBody></DanBamBody>
    <DanBamNav></DanBamNav>
    <DanBamChap></DanBamChap>
    <DanBamBodyMenu></DanBamBodyMenu>
  </div>
</template>

<script>
import DanBamHeader from './components/DanBamHeader.vue'
import DanBamBody from './components/DanBamBody.vue'
import DanBamNav from './components/DanBamNav.vue';
import DanBamChap from './components/DanBamChap.vue';
import DanBamBodyMenu from './components/DanBamBodyMenu.vue';

  export default {
    components: {
    DanBamHeader,
    DanBamBody,
    DanBamNav,
    DanBamChap,
    DanBamBodyMenu
}
  }
</script>

<style scoped>

</style>
