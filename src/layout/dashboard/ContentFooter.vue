<template>
  <footer class="footer">
    <div class="container-fluid">
      <div class="copyright">
        © {{year}} hecho con el <i class="tim-icons icon-heart-2"></i> by
        <a href="https://github.com/moicanbas" target="_blank" rel="noopener">Moisés cantillo,</a> Eder Castro &nbsp;&
        <a href="https://github.com/isradeveloper" target="_blank" rel="noopener">Israel trujillo</a> para desarrollo web II.
      </div>
    </div>
  </footer>
</template>
<script>
  export default {
    data() {
      return {
        year: new Date().getFullYear()
      }
    }
  };
</script>
<style>
</style>
