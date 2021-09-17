<template>
  <footer class="footer">
    <Container class="footer-content">
      <p>Copyright © {{ date }}</p>
      <p>Created by <span class="bold">Victor Jansen</span></p>
    </Container>
  </footer>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  computed: {
    date(): number {
      return new Date().getFullYear()
    },
  },
})
</script>

<style scoped lang="scss">
.footer {
  width: 100%;
  margin-top: 180px;
  height: 58px;
  .footer-content {
    font-size: 13px;
    display: grid;
    height: 100%;
    grid-auto-flow: column;
    justify-content: space-between;
    align-items: center;
    p {
      color: #e3e5e8;
      .bold {
        font-weight: bold;
      }
    }
  }
}

@media (max-width: 1300px) {
  .footer {
    margin-top: 300px;
  }
}

@media (max-width: 700px) {
  .footer {
    margin-top: 200px;
  }
}
</style>
