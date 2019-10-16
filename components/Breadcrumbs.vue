<template>
  <nav class="my-4" v-if="$route.name !== 'index'">
    <ol class="list-reset flex text-grey-dark">
      <li><a href="/" class="text-teal-600 font-bold capitalize">Home</a></li>
      <li><span class="mx-2 text-gray-500">/</span></li>
      <li class="text-gray-500 capitalize">{{$route.name}}</li>
    </ol>
  </nav>
</template>

<script>
export default {

}
</script>

<style>

</style>
