<template>
  <section id="secondLayer" class="grid-second-layer">
    <p>
      Faço o possível para desenvolver
      <span class="bold">sem que o cliente tenha alguma preocupação!</span>
    </p>
    <div class="cards">
      <BlackCard
        title="UI & UX"
        text="Design desenvolvido para melhor 
experiência do usuário.
Sem complicações e dificuldades"
      />
      <BlackCard
        title="Responsividade"
        text="Interface Programada e Modelada para se adaptar a qualquer tipo de tela!"
      />
      <BlackCard
        title="Iteratividade"
        text="Animações e motion Design para sua plataforma. "
      />
    </div>
  </section>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style scoped lang="scss">
.grid-second-layer {
  width: 100%;
  margin: 130px auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-content: center;
  font-family: Poppins;
  color: #e3e5e8;
  font-size: 16px;
  P {
    margin: 0 auto;
    text-align: center;

    .bold {
      color: #ffffff;
      font-weight: bold;
    }
  }
  .cards {
    display: flex;
    flex-wrap: wrap;
    gap: 40px;
    margin-top: 140px;
  }
}

@media (max-width: 700px) {
  .grid-second-layer {
    margin-top: 20px;
  }
}
</style>
