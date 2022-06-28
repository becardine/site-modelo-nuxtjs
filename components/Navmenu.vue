<template>
  <b-navbar toggleable="lg" type="light" class="navMenu">
    <b-navbar-brand href="#">
      <img
        src="~/assets/img/techend-logo.png"
        alt="Logo com o nome da nossa empresa TechEnd e o ícone de um foguete"
      />
    </b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav class="mx-auto" type="light">
        <b-nav-item v-for="item in links" :key="item" :href="item.link">{{
          item.name
        }}</b-nav-item>
      </b-navbar-nav>
      <BtnContact />
    </b-collapse>
  </b-navbar>
</template>
<style scoped>
.navMenu {
  background: var(--color-medium);
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
          name: "Nossos Profissionais",
          link: "#nossos-profissionais",
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