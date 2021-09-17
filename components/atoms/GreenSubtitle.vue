<template>
  <div>
    <p class="subtitle-green">{{ text }}</p>
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
.subtitle-green {
  font-weight: 500;
  font-family: Poppins;
  font-size: 24px;
  color: #7bea95;
  margin-bottom: 10px;
  margin-top: 10px;
}

@media (max-width: 700px) {
  .subtitle-green {
    font-size: 16px;
    margin-bottom: 20px;
  }
}
</style>
