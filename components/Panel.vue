<template>
  <div class="bg-orange-100 mb-4 rounded rounded-t-lg overflow-hidden border border-gray-400 p-4 lg:p-10">
    <div v-if="title && link" class="mb-4">
      <a :href="link" target="_blank" class="text-teal-500 hover:text-teal-600">
        <h2 class="text-2xl inline-block">
          {{ title }} <small class="text-gray-500">(link to doc)</small>
        </h2>
      </a>
    </div>
    <slot />
  </div>
</template>

<script>
export default {
  props: ['link', 'title']
}
</script>

<style>

</style>