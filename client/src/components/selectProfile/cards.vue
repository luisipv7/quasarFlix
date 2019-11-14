<template>
  <q-card
    class="my-card"
    @click.native="$router.push('https://github.com/')"
  >
    <img
      clickable
      src="http://lorempixel.com/150/150/"
    >
    <q-item-section class="flex-center text-h5 relative-bottom">
      <q-item-label>Nome</q-item-label>
    </q-item-section>
  </q-card>
</template>

<script>
export default {

}
</script>

<style>
</style>
