<template>
  <div class="layout-default">
    <header>
      <menu>
        <NuxtLink to="/">Miniblog</NuxtLink>
        <a href="http://isaacgroisman.surge.sh/" target="_blank">About me</a>
      </menu>
    </header>
    <Nuxt />
    <footer>
      <div class="flex mt-8 md:my-8 text-center justify-center">Developed by  <a class="ml-1 underline" href="http://isaacgroisman.surge.sh/" target="_blank"> Isaac Groisman.</a></div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'LayoutDefaul',
}
</script>

<style lang="scss" scoped>
.layout-default {
  @apply min-h-full;
  header {
    @apply sticky absolute top-0 bg-white z-10;
    menu {
      @apply m-auto flex justify-between items-center w-full max-w-5xl px-4 py-6;
    }
    .brand {
      @apply font-bold text-2xl;
    }
  }

  footer div{
    padding-top: 2rem;
    padding-bottom: 2rem;
    background-color: rgba(229, 231, 235, 3);
    margin-bottom: 0;
  }
}
</style>
