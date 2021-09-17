<template>
  <transition appear name="fade">
    <main>
      <FirstLayer />
      <SecondLayer id="padding-scroll-content" />
      <ThirdLayer />
      <FourthLayer />
    </main>
  </transition>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style scoped>
.fade-enter-active,
.fade-leave-active {
  transition: all 2s;
}
.fade-enter,
.fade-leave-to {
  opacity: 0;
  transform: translate3D(0, -20px, 0);
}
</style>
