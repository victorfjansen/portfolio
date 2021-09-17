<template>
  <section class="layer3-grid">
    <div>
      <h1 class="title">
        Unique && <span class="green-word">beautiful Design</span>
      </h1>

      <p class="subtitle">
        Me especializei em novas tecnologias para te dar um negócio único.<br />
        O seu Design. O seu sistema.<br />
        Mais bonito e sempre performático.
      </p>
      <vs-button
        class="darkButton"
        size="large"
        href="https://www.instagram.com/victorjansenf/"
        blank
      >
        Entrar em contato

        <template #animate>
          <i class="fab fa-whatsapp"></i>
        </template>
      </vs-button>
    </div>

    <div class="img">
      <img src="@/assets/img/layer3.svg" alt="" />
    </div>
  </section>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style scoped lang="scss">
.layer3-grid {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  height: 450px;
  align-items: center;
  margin-top: 200px;
  div {
    margin: 0 auto;
  }
  .darkButton {
    margin-top: 22px;
    font-size: 12px;
    font-family: Poppins;
    font-weight: bold;
  }
}

.img {
  width: 427px;
  height: 407px;
  img {
    width: 100%;
    height: 100%;
  }
}

.button {
  display: flex;
  margin-left: -5px;

  .darkButton {
    border: solid 2px #555555;
  }
}

.green-word {
  color: #5aed7d;
}

.title {
  font-weight: bold;
  font-family: Poppins;
  font-size: 36px;
  line-height: 46px;
  color: #fff;
  margin-bottom: -10px;
}

.subtitle {
  margin-top: 40px;
  color: #e3e5e8;
  font-size: 16px;
  font-weight: 400;
}

@media (max-width: 700px) {
  .layer3-grid {
    margin-top: 100px;
  }
}
</style>
