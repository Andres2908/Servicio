<template>
  <div>
    <section class="my-5">
      <Carrusel />
    </section>

    <section>
      <QuickLinks />
    </section>

    <div>
      <Card />
    </div>

    <figure class="image is-3by1 my-5">
      <img
        src="https://www.techadvisor.com/cmsdata/features/3499097/ms_surface_laptop_13_5_review14_thumb1200_16-9.jpg"
      />
      <h2 class="is-size-4 has-text-white">
        <b>Actualización de Windows 10</b>
      </h2>
      <p class="texto is-size-6 has-text-white">
        Nuevas características que te ayudarán a dedicarte a lo que te apasiona,
        aconectarte más y a devolver un poco de tu tiempo
        <br />
      </p>
    </figure>

    <div>
      <Card />
    </div>

    <div class="has-text-centered covid py-5">
      <p style="font-size: 30px">
        <b>La respuesta de Microsoft a la COVID-19</b>
      </p>
      <p>
        Lee cómo estamos respondiendo al brote de COVID-19 y encuentra recursos
        para ayudarte.
      </p>
      <a href="#">Más información</a>
    </div>
    <br />
  </div>
</template>

<script>
import Carrusel from "../components/carrusel.vue";
import Card from "../components/card.vue";
import QuickLinks from "../components/quickLinks.vue";

export default {
  components: { Carrusel, Card, QuickLinks },
  methods: {
    methods: {
      carouselImage(value) {
        return `https://9c6368703316.ngrok.io/imagenes/card_1.jpeg`;
      }
    }
  }
};
</script>

<style>
h2 {
  position: absolute;
  top: 35%;
  left: 71%;
  transform: translate(-65%, -29%);
}
.texto {
  position: absolute;
  top: 50%;
  left: 70%;
  transform: translate(-50%, -30%);
}
.covid {
  background: #e6e6e6;
}
</style>
