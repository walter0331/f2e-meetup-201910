<template>
  <div>
    <Panel>
      <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
        Simple
      </button>
    </Panel>

    <Panel>
      <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded-full">
        Pill
      </button>
    </Panel>

    <Panel>
      <button class="bg-transparent hover:bg-blue-500 text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
        Outline
      </button>
    </Panel>

    <Panel>
      <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 border border-blue-700 rounded">
        Bordered Button
      </button>
    </Panel>

    <Panel>
      <button class="bg-blue-500 hover:bg-blue-400 text-white font-bold py-2 px-4 border-b-4 border-blue-700 hover:border-blue-500 rounded">
        3D Button
      </button>
    </Panel>

    <Panel title="Button with counter" link="https://tailwindcomponents.com/component/button-with-counter">
      <div class="mt-4">
        <button class='relative bg-blue-500 text-white p-6 rounded text-2xl font-bold overflow-visible'>
          Example button
          <div class="absolute top-0 right-0 -mt-4 -mr-4 px-4 py-1 bg-red-500 rounded-full">2000</div>
        </button>
      </div>
    </Panel>
    
    <Panel title="Nice looking button" link="https://tailwindcomponents.com/component/nice-looking-button">
      <div class="inline-flex">
        <button class="bg-gray-400 hover:bg-gray-500 text-gray-800 font-bold py-2 px-4 rounded-l">
          Prev
        </button>
        <button class="bg-gray-400 hover:bg-gray-500 text-gray-800 font-bold py-2 px-4 rounded-r">
          Next
        </button>
      </div>
    </Panel>

  </div>
</template>

<script>
import Panel from '~/components/Panel';

export default {
  components: {
    Panel
  }
}
</script>

<style>

</style>
