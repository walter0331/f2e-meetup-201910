<template>
  <nav class="flex items-center justify-between flex-wrap bg-teal-500 p-6">
    <div class="flex items-center flex-shrink-0 text-white mr-6">
      <a href="/">
        <span class="font-semibold text-xl tracking-tight">F2E&RGBA Meetup</span>
      </a>
    </div>
    <!-- desktop menu -->
    <div class="w-auto flex-auto flex litems-center hidden lg:block">
      <div class="text-sm flex">
        <a href="/cards" class="block text-teal-200 hover:text-white mr-4">
          Cards
        </a>
        <a href="/buttons" class="block text-teal-200 hover:text-white mr-4">
          Buttons
        </a>
        <a href="/forms" class="block text-teal-200 hover:text-white mr-4">
          Forms
        </a>
        <a href="/colors" class="block text-teal-200 hover:text-white">
          Colors
        </a>
      </div>
    </div>

    <!-- mobile menu -->
    <div class="block lg:hidden">
      <button
        @click="onToggleMenu()"
        class="flex items-center px-3 py-2 border rounded text-teal-200 border-teal-400 hover:text-white hover:border-white">
        <svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/></svg>
      </button>
    </div>
    <div v-if="openMenu" class="w-full block flex-grow lg:flex lg:items-center lg:w-auto">
      <div class="text-sm lg:flex-grow">
        <a href="/cards" class="block mt-4 lg:inline-block lg:mt-0 text-teal-200 hover:text-white mr-4">
          Cards
        </a>
        <a href="/buttons" class="block mt-4 lg:inline-block lg:mt-0 text-teal-200 hover:text-white mr-4">
          Buttons
        </a>
        <a href="/forms" class="block mt-4 lg:inline-block lg:mt-0 text-teal-200 hover:text-white">
          Forms
        </a>
        <a href="/forms" class="block mt-4 lg:inline-block lg:mt-0 text-teal-200 hover:text-white">
          Colors
        </a>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      openMenu: false
    }
  },
  methods: {
    onToggleMenu() {
      this.openMenu = !this.openMenu;
    }
  }
}
</script>

<style>

</style>
