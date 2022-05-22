<template>
  <div>
    <NavBar/>
    <HomeComponent/>
    <FooterComponent/>
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue';
import HomeComponent from './components/Home.vue';
import FooterComponent from './components/Footer.vue';
export default {
  name: "App",
  components: { NavBar, HomeComponent, FooterComponent },
};
</script>

<style lang="scss" >
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500&family=Ubuntu:wght@300;400;500&display=swap");

$primaryBrandColor:#2290E8;
$secondaryBrandColor:#F34336;
* {
  padding: 0;
  margin: 0;
  font-family: "Roboto", sans-serif;
  color: #36454f ;
}
</style>
