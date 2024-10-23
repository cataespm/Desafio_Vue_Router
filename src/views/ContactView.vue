<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
  <section class="container px-5">
    <div class="row">
      <div class="col pt-5">
        <h1 class="text-center pb-3">Contactame</h1>
        <p class="d-none d-md-block text-center">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates
          sunt quia nobis tempora aliquam, labore similique sapiente ut
          praesentium veniam fuga quae vitae error. Facilis commodi repellat eum
          nesciunt quas?
        </p>

        <div class="mb-3">
          <label for="exampleFormControlInput1" class="form-label"
            >Nombre</label
          >
          <input
            type="text"
            class="form-control"
            id="exampleFormControlInput1"
            placeholder="Nombre"
          />
        </div>
        <div class="mb-3">
          <label for="exampleFormControlInput1" class="form-label"
            >Correo Electrónico</label
          >
          <input
            type="email"
            class="form-control"
            id="exampleFormControlInput1"
            placeholder="name@example.com"
          />
        </div>
        <div class="mb-3">
          <label for="exampleFormControlTextarea1" class="form-label"
            >Mensaje</label
          >
          <textarea
            class="form-control"
            id="exampleFormControlTextarea1"
            rows="3"
          ></textarea>
        </div>
        <div class="mb-5">
          <button
            type="button"
            class="ms-auto text-end btn btn-info text-white"
          >
            Enviar
          </button>
        </div>
      </div>
    </div>
    <button @click="VolverAlInicio" class="btn btn-primary">Ir a Inicio</button>
  </section>
</template>
<script>
export default {
  methods: {
    VolverAlInicio() {
      this.$router.push({ name: "inicio" });
    },
  },
};
</script>
