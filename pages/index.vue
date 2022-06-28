<template>
  <div>
    <Navmenu />
    <header class="wrapper d-flex py-5 align-items-center gap-2">
      <div class="col-lg-8">
        <h1 class="fw-bold">
          Ajudamos sua empresa se destacar no meio digital.
        </h1>
        <p class="text-secondary my-4 mb-5">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Incidunt
          voluptate quidem iusto quia suscipit commodi sit illum minus cum,
          facilis itaque repudiandae doloremque tempore labore laboriosam at
          illo dicta molestiae facilis itaque repudiandae doloremque tempore
          labore laboriosam at illo dicta molestiae!
        </p>

        <BtnContact />
      </div>

      <div class="col-lg-4">
        <img
          src="~/assets/img/office-work.jpg"
          width="300px"
          alt="Pessoas sentadas conversando e sorrindo, mostrando algumas informações"
          class="rounded"
        />
      </div>
    </header>

    <main>
      <Professionals />

      <section
        class="wrapper d-flex py-5 align-items-center"
      >
        <div class="col-lg-7">
          <img
            src="~/assets/img/time-reunido.jpg"
            alt="Pessoas sentadas conversando e sorrindo, mostrando algumas informações"
            class="rounded"
          />
        </div>
        <div class="col-lg-5">
          <h4 class="text-end">Sobre nós</h4>
          <h2 class="fs-5">De onde viemos e para onde queremos ir</h2>
          <p class="text-secondary my-4 mb-5">
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Incidunt
            voluptate quidem iusto quia suscipit commodi sit illum minus cum,
            facilis itaque repudiandae doloremque tempore labore laboriosam at
            illo dicta molestiae facilis itaque repudiandae doloremque tempore
            labore laboriosam at illo dicta molestiae!
          </p>
        </div>
      </section>
    </main>

    <footer class="d-flex align-items-center justify-content-around py-2 footerBg">
      <span>@techend</span>
      <span>(48) 9999-9999</span>
      <span>Rua dos Morros, 21</span>
    </footer>
  </div>
</template>
<style scoped>
img {
  box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
}

.footerBg {
  background: var(--color-medium);
  color: var(--color-light);
}
</style>
<script>
</script>
