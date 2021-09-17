<template>
  <div class="error-layout">
    <div>
      <img src="@/assets/img/404.svg" alt="Erro 404" />

      <p class="error-text">
        A página que você está procurando<br />
        não existe ou foi removida
      </p>

      <vs-button to="/" flat> Home </vs-button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.error-layout {
  display: grid;
  place-items: center;
  height: 100vh;
  div {
    text-align: center;
    display: flex;
    flex-direction: column;
    gap: 30px;
  }
  .error-text {
    color: #e3e5e8;
    font-size: 24px;
    font-weight: bold;
  }
}

@media (max-width: 1300px) {
  .error-layout {
    img {
      max-width: 500px;
    }
  }
}

@media (max-width: 900px) {
  .error-layout {
    img {
      max-width: 400px;
    }
  }
}

@media (max-width: 700px) {
  .error-layout {
    img {
      max-width: 300px;
    }
  }
}
</style>
