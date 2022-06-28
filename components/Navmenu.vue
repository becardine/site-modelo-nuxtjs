<template>
  <b-navbar toggleable="lg" class="navMenu">
    <b-navbar-brand href="#">
        <img src="~/assets/img/techend-logo.png" alt="Logo com o nome da nossa empresa TechEnd e o ícone de um foguete">
    </b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav class="mx-auto link">
        <b-nav-item v-for="item in links" :key="item" :href="item.link" class="text-white">{{
          item.name
        }}</b-nav-item>
      </b-navbar-nav>
      <b-button class="btnToSchedule rounded-pill border-0 px-4">Agende seu horário</b-button>
    </b-collapse>
  </b-navbar>
</template>
<style scoped>
.navMenu {
  background: var(--color-medium);
  color: var(--color-light);
}

.link {
    color: var(--color-light);
}
.btnToSchedule {
    background: var(--color-contrast);
    transition: background .2s;
}
.btnToSchedule:hover {
    background: var(--color-hover);
}
</style>
<script>
export default {
  data() {
    return {
      links: [
        {
          name: "Início",
          link: "#inicio",
        },
        {
          name: "Sobre",
          link: "#sobre",
        },
        {
          name: "Profissionais",
          link: "#profissionais",
        },
        {
          name: "Contato",
          link: "#contato",
        },
      ],
    };
  },
};
</script>