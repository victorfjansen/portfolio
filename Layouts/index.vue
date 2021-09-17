<template>
  <div>
    <Header />
    <div class="overlay">
      <h1>Jansen</h1>
    </div>
    <Container>
      <Nuxt />
    </Container>
    <Footer />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import { gsap } from 'gsap'

export default Vue.extend({
  mounted() {
    setTimeout(() => {
      this.overflow()
    }, 10)
  },
  methods: {
    overflow() {
      const body = document.querySelector('body')
      body?.classList.add('overflow-hidden')
      this.TweenMax()
      setTimeout(() => {
        body?.classList.remove('overflow-hidden')
      }, 3000)
    },
    TweenMax() {
      gsap.fromTo(
        '.overlay h1',
        { opacity: 1 },
        { opacity: 0, y: -60, duration: 1, delay: 1 }
      )
      gsap.fromTo(
        '.overlay',
        { top: '0' },
        { top: '-100%', duration: 1, delay: 2 }
      )
    },
  },
})
</script>

<style scoped></style>
