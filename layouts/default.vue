<template>
  <div>
    <nav
      class="navbar header has-shadow "
      role="navigation"
      aria-label="main navigation"
    >
      <div class="navbar-brand">
        <a class="navbar-item" href="/">
          <img src="~assets/buefy.png" alt="Buefy" height="28" />
        </a>

        <div class="=navbar-menu">
          <div class="navbar">
            <b-navbar-item href="#">
              Surface
            </b-navbar-item>

            <b-dropdown
              append-to-body
              aria-role="menu"
              scrollable
              max-height="200"
              trap-focus
            >
              <template #trigger>
                <a class="navbar-item" role="button">
                  <span>Equipos</span>
                  <b-icon icon="menu-down"></b-icon>
                </a>
              </template>

              <b-dropdown-item
                v-for="item of equipos"
                :key="item"
                aria-role="listitem"
                >{{ item }}</b-dropdown-item
              >
            </b-dropdown>

            <b-dropdown
              append-to-body
              aria-role="menu"
              scrollable
              max-height="200"
              trap-focus
            >
              <template #trigger>
                <a class="navbar-item" role="button">
                  <span>Equipos para empresas</span>
                  <b-icon icon="menu-down"></b-icon>
                </a>
              </template>

              <b-dropdown-item
                v-for="item of equipos"
                :key="item"
                aria-role="listitem"
                >{{ item }}</b-dropdown-item
              >
            </b-dropdown>

            <b-navbar-item href="#">
              Comprar ahora
            </b-navbar-item>

            <b-navbar-item href="#">
              Soporte técnico
            </b-navbar-item>
          </div>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  data() {
    return {
      equipos: [
        "Angular",
        "Angular 2",
        "Aurelia",
        "Backbone",
        "Ember",
        "jQuery",
        "Meteor",
        "Node.js",
        "Polymer",
        "React",
        "RxJS",
        "Vue.js"
      ]
    };
  }
};
</script>
