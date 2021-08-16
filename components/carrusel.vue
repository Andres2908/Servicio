<template>
  <div>
    <b-carousel>
      <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
        <section :class="`hero is-large`">
          <div class="hero-body has-text-centered">
            <h1 class="is-size-3">{{ carousel.title }}</h1>
            <p class="is-size-5 ">{{ carousel.text }}</p>
            <b-button type="is-dark">{{ carousel.button }}</b-button>
            <div></div>
            <figure class="image is-3by1">
              <img :src="carouselImage(i + 1)" alt="imagen" />
            </figure>
          </div>
        </section>
      </b-carousel-item>
    </b-carousel>
  </div>
</template>

<script>
export default {
  data() {
    return {
      carousels: [
        {
          title: "Aprende a tu manera",
          text:
            "Regresa a clases con Microsoft 365 y disfruta de aplicaciones prémium de Office, almacenamiento en la nube, seguridad avanzada y más.",
          button: "Elige el plan ideal"
        },
        {
          title: "Surface Laptop Go",
          text:
            "Aprovecha al máximo cada día con nuestro dispositivo Surface Laptop más ligero",
          button: "Compra ahora"
        }
      ],
      dataImage: ""
    };
  },
  methods: {
    carouselImage(value) {
      return `https://venus.acatlan.unam.mx/retos/imagenes/carrusel_${value}.jpeg`;
    }
  },
  created() {
    // console.log(carouselImage());
  }
};
</script>

<style>
.hero-body {
  padding: 0rem 0rem !important;
}
.containerC {
  position: relative;
  display: inline-block;
  text-align: center;
}
.over-text {
  position: absolute;
  top: 600px;
  left: 30px;
}
</style>
