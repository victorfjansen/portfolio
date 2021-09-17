<template>
  <header class="center examplex">
    <vs-navbar
      v-model="active"
      vs-theme="dark"
      target-scroll="#padding-scroll-content"
      padding-scroll
      square
    >
      <template #left>
        <p class="jansen" @click="goToTop">Jansen</p>
      </template>

      <vs-navbar-item
        id="sobre"
        :active="active == 'sobre'"
        class="marginitems"
      >
        Sobre
      </vs-navbar-item>

      <vs-navbar-group class="nav-bar-group">
        <p>Contate-me</p>
        <template #items>
          <h5 class="title">Social</h5>

          <vs-navbar-item id="Instagram">
            <a href="https://www.instagram.com/victorjansenf/" target="_blank">
              Instagram
            </a>
          </vs-navbar-item>
          <vs-navbar-item id="Discord">
            <a
              href="https://api.whatsapp.com/send?phone=5527992415328"
              target="_blank"
            >
              Whatsapp
            </a>
          </vs-navbar-item>
          <vs-navbar-item id="GitHub">
            <a href="https://github.com/victorfjansen" target="_blank">
              Meu GitHub
            </a>
          </vs-navbar-item>
        </template>
      </vs-navbar-group>

      <template #right>
        <div class="marginright">
          <a href="https://www.instagram.com/victorjansenf/" target="_blank">
            <img src="@/assets/img/instagram.svg" alt="Instagram" />
          </a>
          <a href="https://github.com/victorfjansen" target="_blank">
            <img src="@/assets/img/github.svg" alt="Github Icon" />
          </a>
        </div>
      </template>
    </vs-navbar>
  </header>
</template>
<script>
export default {
  data: () => ({
    active: 'sobre',
  }),
  methods: {
    goToTop() {
      window.scrollTo(0, 0)
    },
  },
}
</script>

<style scoped lang="scss">
.jansen {
  font-size: 24px;
  font-weight: bold;
  margin-left: 100px;
}

.marginright {
  margin-right: 100px;
  a {
    margin-right: 40px;
    width: 18px;
    height: 18px;
  }
}

.marginitems {
  margin-right: 53px;
}

a {
  text-decoration: none;
  color: #fff;
}

* {
  font-family: Poppins;
}

.nav-bar-group {
  font-family: Poppins;
}

@media (max-width: 1300px) {
  .jansen {
    margin-left: 0px;
  }
  .marginright {
    margin-right: 0px;
    a {
      margin-right: 10px;
    }
  }
}

@media (max-width: 700px) {
  .marginright {
    display: none;
  }
  .marginitems {
    margin-right: 10px;
  }
}
</style>
