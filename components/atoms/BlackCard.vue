<template>
  <div class="black-card">
    <h2 class="title-card">{{ title }}</h2>
    <p class="text-card">
      {{ text }}
    </p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  props: {
    title: { type: String, required: true },
    text: { type: String, required: true },
  },
})
</script>

<style scoped lang="scss">
.black-card {
  width: 260px;
  background: #141417;
  border: solid 1px #252525;
  padding: 30px;
  border-radius: 50px;
  display: flex;
  flex-direction: column;
  text-align: center;
  gap: 18px;
  transition: all ease 0.3s;
  .title-card {
    font-size: 1em;
    font-weight: bold;
  }
  .text-card {
    font-size: 12px;
    font-weight: 400;
    line-height: auto;
  }
  &:hover {
    transform: translate(0, -5px);
    box-shadow: 2px 4px 4px rgba(0, 0, 0, 0.7);
  }
}

@media (max-width: 1300px) {
  .black-card {
    width: 200px;
  }
}
</style>
