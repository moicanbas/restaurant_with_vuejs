<template>
  <div class="wrapper">
    <side-bar>
      <template slot="links">
        <sidebar-link to="/" name="Inicio" icon="tim-icons icon-chart-pie-36"/>
        <sidebar-link to="/carrito-compras" name="Carrito" icon="tim-icons icon-cart"/>
        <sidebar-link to="/historial-pedidos" name="Histórico pedidos" icon="tim-icons icon-single-copy-04"/>
        <sidebar-link to="/profile" name="Datos de facturación" icon="tim-icons icon-delivery-fast"/>
      </template>
    </side-bar>
    <div class="main-panel">
      <top-navbar></top-navbar>

      <dashboard-content @click.native="toggleSidebar">

      </dashboard-content>

      <content-footer></content-footer>
    </div>
  </div>
</template>
<style lang="scss">
</style>
<script>
import TopNavbar from "./TopNavbar.vue";
import ContentFooter from "./ContentFooter.vue";
import DashboardContent from "./Content.vue";
import MobileMenu from "./MobileMenu";
export default {
  components: {
    TopNavbar,
    ContentFooter,
    DashboardContent,
    MobileMenu
  },
  methods: {
    toggleSidebar() {
      if (this.$sidebar.showSidebar) {
        this.$sidebar.displaySidebar(false);
      }
    }
  }
};
</script>
