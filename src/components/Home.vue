<template>
  <div class="home">
    <HeroComponent/>
    <PortFolio/>
  </div>
</template>

<script>
import HeroComponent from './Hero.vue';
import PortFolio from './Portfolio.vue';

export default {
    name: "HomeComponent",
    setup() {
        return {};
    },
    components: { HeroComponent, PortFolio }
};
</script>

<style lang="scss" scoped>
.home {
  padding: 35px;
  margin: 0 auto;

}
</style>