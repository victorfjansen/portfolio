<template>
  <section class="fourth-section">
    <p>Confira alguns de Meus Projetos:</p>
    <div class="project-cards">
      <Card />
      <Card />
      <Card />
    </div>
  </section>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style scoped>
.fourth-section {
  margin: 130px auto;
}
p {
  font-family: Poppins;
  color: #e3e5e8;
  font-size: 16px;
}

.project-cards {
  gap: 40px;
  margin-top: 140px;
  display: flex;
  flex-wrap: wrap;
}

@media (max-width: 1300px) {
  .fourth-section {
    margin-top: 300px;
  }
}
</style>
