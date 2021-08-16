<template>
  <div>
    <div class="container">
      <NavBar />
      <Nuxt />
    </div>

    <Footer />
  </div>
</template>

<script>
import NavBar from "../components/navBar.vue";
import Footer from "../components/Footer.vue";
export default {
  components: { NavBar, Footer }
};
</script>
