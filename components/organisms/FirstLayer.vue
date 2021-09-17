<template>
  <section class="layer1-grid">
    <div>
      <Title text="Victor Jansen" />
      <GreenSubtitle
        text="UI/UX Designer and fullstack Developer </>"
        class="green-subtitle"
      />
      <div class="button">
        <vs-button size="large" class="primaryButton" @click="goToSection">
          Saber Mais
          <template #animate>
            <i class="fas fa-rocket"></i>
          </template>
        </vs-button>
        <vs-button
          dark
          class="darkButton"
          color="#141417"
          size="large"
          href="https://www.instagram.com/victorjansenf/"
          blank
        >
          Instagram

          <template #animate>
            <i class="fab fa-instagram"></i>
          </template>
        </vs-button>
      </div>
    </div>
    <div class="img">
      <img src="@/assets/img/ICONS.svg" alt="ICONS" />
    </div>
  </section>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  methods: {
    goToSection() {
      window.scrollTo(0, 690)
    },
  },
})
</script>

<style scoped lang="scss">
.layer1-grid {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  height: 450px;
  align-items: center;
  margin-top: 200px;
  div {
    margin: 0 auto;
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
    font-family: Poppins;
    font-size: 12px;
  }
  .primaryButton {
    font-family: Poppins;
    font-size: 12px;
  }
}

@media (max-width: 1300px) {
  .layer1-grid {
    margin-top: 200px;
    div {
      margin: 0;
    }
  }
  .img {
    position: absolute;
    right: 0;
    z-index: -1;
    opacity: 0.4;
  }
}

@media (max-width: 700px) {
  .button {
    margin-top: 10px;
    .darkButton,
    .primaryButton {
      font-size: 10px;
    }
  }

  .img {
    display: none;
  }
}
</style>
