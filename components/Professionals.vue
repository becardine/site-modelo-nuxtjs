<template>
  <section class="wrapper text-center mt-5">
    
    <h4>Nossos Profissionais</h4>
    <h2 class="fs-5">Conheça quem faz seu negócio decolar</h2>

    <div class="d-flex my-5 justify-content-around">
      <b-card
        v-for="professional in professionals"
        :key="professional"
        :title="professional.name"
        :img-src="professional.photo"
        :img-alt="professional.alt"
        img-top
        tag="article"
        style="max-width: 20rem"
        class="mb-2"
      >
        <b-card-text>
          {{ professional.description }}
        </b-card-text>

        <b-button href="#" class="btnInfo border-0 rounded-pill">{{
          professional.cargo
        }}</b-button>
      </b-card>
    </div>
  </section>
</template>
<style scoped>
.btnInfo {
  background: var(--color-medium);
}
</style>
<script>
export default {
  data() {
    return {
      professionals: [
        {
          name: "Maria",
          photo: require("~/assets/img/maria.jpg"),
          alt: "Foto de um de nossos profissionais",
          description: "Atua na área há mais de 10 anos, ama livros e gatos.",
          cargo: "Desenvolvedora Back-end",
        },
        {
          name: "Jorge",
          photo: require("~/assets/img/jorge.jpg"),
          alt: "Foto de um de nossos profissionais",
          description: "Atua na área há mais de 10 anos, ama livros e gatos.",
          cargo: "Desenvolvedor Front-end",
        },
        {
          name: "Helena",
          photo: require("~/assets/img/helena.jpg"),
          alt: "Foto de um de nossos profissionais",
          description: "Atua na área há mais de 10 anos, ama livros e gatos.",
          cargo: "Analista",
        },
      ],
    };
  },
};
</script>