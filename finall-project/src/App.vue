<template>
  <div class="container">
    <headerCompornet></headerCompornet>
    <Category></Category>
    <productsrecommend></productsrecommend>
    <footerComponent></footerComponent>
  </div>
</template>

<script>
import headerCompornet from "./components/header-component.vue";
import productsrecommend from "./components/productsre-component.vue";
import footerComponent from "./components/footer-component.vue";
import Category from "./components/Category-component.vue";
export default {
  name: "App",
  components: {
    headerCompornet,
    productsrecommend,
    footerComponent,
    Category
  },
};
</script>

<style >
/* .container{
  overflow: hidden;
  width: 8000px;
  height: 3725px;
  background-color: #3d4380;
  display: flex;
  flex-direction: column;
  /* align-items: center; */
/* }  */
.container{
  overflow: hidden;
  /* width: 8000px;
  height: 3725px; */
  background-color: #3d4380;
  display: flex;
  flex-direction: column;
}
</style>
