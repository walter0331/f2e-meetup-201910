<template>
  <div class="bg-gray-200">
    <Header />
    <div class="flex flex-col container mx-auto min-h-screen">
      <div class="flex-auto p-4">
        <Breadcrumbs />
        <nuxt />
      </div>
    </div>
  </div>
</template>
<script>
import Header from '~/components/Header';
import Breadcrumbs from '~/components/Breadcrumbs';

export default {
  components: {
    Header,
    Breadcrumbs
  }
}
</script>
