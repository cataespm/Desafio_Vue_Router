<template>
  <section class="container" id="productos">
    <h1 class="text-center">Productos</h1>
    <div class="row">
      <div class="col-sm-4 col-12 px-5 mb-4">
        <SingleCard
          :nombre="nombre"
          :descripcion="descripcion"
          :precio="precio"
          :cantidad="cantidad"
          :imagen="imagen"
        />
      </div>
    </div>

    <div>
      <button @click="VolverAlInicio" class="btn btn-primary">
        Ir a Inicio
      </button>
    </div>
  </section>
</template>
<script>
import SingleCard from "../components/SingleCard.vue";

export default {
  methods: {
    VolverAlInicio() {
      this.$router.push({ name: "inicio" });
    },
  },
  components: {
    SingleCard,
  },
  props: {
    // productos: Array,
    require: true,
    nombre: {
      type: String,
      required: true,
    },
    descripcion: {
      type: String,
      required: true,
    },
    precio: {
      type: Number,
      required: true,
    },
    cantidad: {
      type: String,
      required: true,
    },
    imagen: {
      type: String,
      required: true,
    },
  },
};
</script>
