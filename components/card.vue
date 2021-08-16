<template>
  <div class="columns my-2 mb-5">
    <div v-for="(card, i) in 4" :key="i" class="card">
      <div class="colum px-3">
        <div class="card-image ">
          <figure class="image is-2by1 ">
            <img :src="cardImage(i + 1)" alt="Placeholder image" />
          </figure>
        </div>
        <div class="card-content">
          <div class="content">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus
            nec iaculis mauris. <a>@bulmaio</a>. <a href="#">#css</a>
            <a href="#">#responsive</a>
            <br />
            <time datetime="2016-1-1">11:09 PM - 1 Jan 2016</time>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    cardImage(value) {
      return `https://venus.acatlan.unam.mx/retos/imagenes/card_${value}.jpeg`;
    }
  }
};
</script>

<style></style>
