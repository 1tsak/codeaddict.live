<template>
  <div class="portfolio flex flex-col items-center justify-center">
    <h2 class="m-5 hover:ease-linear underline">OUR WORK</h2>
    <div class="projects flex flex-row space-x-5 m-5">
        
        <ProjectItem/>
        <ProjectItem/>
        <ProjectItem/>
        <ProjectItem/>
    </div>
  </div>
</template>

<script>
import ProjectItem from './ProjectItem.vue';
export default {
    name: "PortFolio",
    components: { ProjectItem }
};
</script>

<style lang="scss" scoped>

</style>