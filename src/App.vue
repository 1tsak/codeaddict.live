<template>
  <div>
    <NavBar />
    <HomeComponent />
    <FooterComponent />
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import HomeComponent from "./components/Home.vue";
import FooterComponent from "./components/Footer.vue";
export default {
  name: "App",
  components: { NavBar, HomeComponent, FooterComponent },
};
</script>

<style lang="scss" >
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500&family=Ubuntu:wght@300;400;500&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;500;600&display=swap");

$primaryBrandColor: #2290e8;
$secondaryBrandColor: #f34336;
* {
  padding: 0;
  margin: 0;
  font-family: "Open Sans", sans-serif;
  font-size: 18px;
  color: #36454f;
}
html,body{
  height: 100%;
}

#app {
  display: flex;
  flex-direction: column;
  height: 100%;
  // background: url(./assets/bg.svg);
  margin: 0 auto;
  // background: rgb(240, 243, 255);
  // background: radial-gradient(
  //   circle,
  //   rgba(240, 243, 255, 1) 0%,
  //   rgba(255, 244, 246, 1) 100%
  // );
}
</style>
