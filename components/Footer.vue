<template>
  <footer class="py-4">
    <div class="container is-flex is-justify-content-between is-size-6 py-4">
      <div>
        <div class="columns">
          <div class="column">
            <div class="columns is-mobile">
              <div class="column">
                <p class="bd-notification is-info ">
                  <b>Novedades</b>
                </p>
                <br />
                <a href="#" class="bd-notification is-info py-5">
                  Microsoft 365 </a
                ><br />
                <a href="#" class="bd-notification is-info">
                  Aplicaciones de Windows 10
                </a>
              </div>
              <div class="column">
                <p class="bd-notification is-info"><b> Microsoft store</b></p>
                <br />
                <a href="#">Perfil de la cuenta</a><br />
                <a href="#">Centro de descargas</a><br />
                <a href="#">Soporte de Microsoft Store</a><br />
                <a href="#">Devoluciones y reembolsos</a><br />
                <a href="#">Devoluciones y reembolsos</a>
              </div>
              <div class="column">
                <p class="bd-notification is-info"><b>Educación</b></p>
                <br />
                <a href="#">Office 365 para escuelas</a><br />
                <a href="#">Office 365 para escuelas</a>
              </div>
            </div>
          </div>

          <div class="column">
            <div class="columns is-mobile">
              <div class="column is-4">
                <p class="bd-notification is-info"><b>Grandes empresas</b></p>
                <br />
                <a href="#">Azure</a><br />
                <a href="#">AppSource</a><br />
                <a href="#">Automotriz</a><br />
                <a href="#">Gobierno</a><br />
                <a href="#">Atención para la salud</a><br />
                <a href="#">Manufactura</a><br />
                <a href="#">Servicios financieros</a><br />
                <a href="#">Comercio directo</a>
              </div>
              <div class="column is-4">
                <p class="bd-notification is-info"><b>Desarrollador</b></p>
                <br />
                <a href="#">Microsoft Visual Studio</a><br />
                <a href="#">Centro de desarrollo</a><br />
                <a href="#">Channel 9</a><br />
                <a href="#">Centro para desarrolladores de Microsoft 365</a
                ><br />
                <a href="#">Programa para desarrolladores de Microsoft 365</a>
              </div>
              <div class="column is-4">
                <p class="bd-notification is-info"><b>Compañía</b></p>
                <br />
                <a href="#">Trabajos</a><br />
                <a href="#">Acerca de Microsoft</a><br />
                <a href="#">Privacidad en Microsoft</a><br />
                <a href="#">Inversionistas</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style scoped>
footer {
  background-color: #e6e6e6;
  /* position: fixed;
  bottom: 0px;
  left: 0px;
  right: 0px; */
}
a {
  color: #2a2b2e;
  text-decoration: none;
  background-image: linear-gradient(currentColor, currentColor);
  background-position: 0% 100%;
  background-repeat: no-repeat;
  background-size: 0% 2px;
  transition: background-size 0.3s;
}
a:hover,
a:focus {
  background-size: 100% 1px;
}
</style>
