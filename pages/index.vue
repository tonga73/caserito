<template>
  <div class="container">
    <div>
      <Logo />
      <div class="p-5">
        <!-- <nuxt-link class="button--grey" to="/">¿quienes somos?</nuxt-link>
        <nuxt-link class="button--green" to="/">productos</nuxt-link> -->
        <nuxt-link class="button--green" to="/perfil-nutricional"
          >PERFIL NUTRICIONAL</nuxt-link
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
</style>
