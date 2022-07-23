<template>
  <div>
    <div
      class="
        hover:scale-105
        transition-all
        cursor-pointer
        project-item
        w-[350px]
        h-[250px]
        flex flex-col
        shadow-sm shadow-slate-300
        border border-slate-100
        relative
        p-5
        rounded-lg
      "
    >
      <img
        class="
          absolute
          top-0
          left-0
          right-0
          bottom-0
          w-[100%]
          h-[100%]
          rounded-lg
          z-10
        "
        src="./../assets/project_bg.jpg"
        alt=""
      />
      <h1 class="z-20 backdrop-blur-sm text-3xl mt-5 text-white">ODT</h1>
      <p class="z-20 backdrop-blur-sm text-sm text-slate-100">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Id rem, quidem
        hic esse aliquid ea inventore voluptate illo veniam natus!
      </p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
</style>