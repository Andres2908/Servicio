<template>
  <div>
    <nav
      class="navbar header has-shadow "
      role="navigation"
      aria-label="main navigation"
    >
      <div class="navbar-brand">
        <a class="navbar-item" href="/">
          <img
            src="data:image/png;base64,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"
            alt="Buefy"
            height="28"
          />
        </a>

        <b-navbar-item href="#">
          Microsoft 365
        </b-navbar-item>

        <b-navbar-item href="#">
          Office
        </b-navbar-item>

        <b-navbar-item href="#">
          Windows
        </b-navbar-item>

        <b-navbar-item href="#">
          Surface
        </b-navbar-item>

        <b-navbar-item href="#">
          Xbox
        </b-navbar-item>

        <b-navbar-item href="#">
          Soporte
        </b-navbar-item>
      </div>

      <div class="=navbar-menu">
        <div class="navbar-end">
          <b-dropdown
            append-to-body
            aria-role="menu"
            scrollable
            max-height="200"
            trap-focus
          >
            <template #trigger>
              <a class="navbar-item" role="button">
                <span>Todo Microsoft</span>
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
    </nav>
    <Nuxt />
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
