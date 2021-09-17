<template>
  <div>
    <h1 class="title">{{ text }}</h1>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  props: {
    text: { type: String, required: true },
  },
})
</script>

<style scoped>
.title {
  font-weight: bold;
  font-family: Poppins;
  font-size: 36px;
  line-height: 46px;
  color: #fff;
  margin-bottom: -10px;
}
</style>
