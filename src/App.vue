<template>
  <div id="app  container">
    <Header class="header"></Header>
    <router-view/>
    <Footer class="mt-5"></Footer>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "app",
  components: {
    Header,
    Footer
  }
};
</script>

<style>



</style>
