<template>
  <a href="https://api.whatsapp.com/send?phone=5527992415328" target="_blank">
    <vs-card vs-theme="dark" class="card">
      <template #title>
        <h3>{{ title }}</h3>
      </template>
      <template #img>
        <img :src="require(`@/assets/img/more.png`)" :alt="src" />
      </template>
      <template #text>
        <p>{{ text }}</p>
      </template>
    </vs-card></a
  >
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  props: {
    title: { type: String, default: 'O Nosso Projeto' },
    text: {
      type: String,
      default:
        'Clique Aqui Para entrar em contato para que possamos desenvolver! Seu projeto pode estar aqui!',
    },
    src: { type: String, default: '@/assets/img/more.png' },
  },
})
</script>

<style scoped>
.card {
  max-width: 320px;
}

a {
  text-decoration: none;
}

@media (max-width: 1300px) {
  .black-card {
    max-width: 280px;
  }
}

@media (max-width: 1090px) {
  .black-card {
    max-width: 240px;
  }
}
</style>
