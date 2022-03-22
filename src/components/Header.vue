<template>
  <header class="h-24 flex items-center mx-36">
    <div class="container flex items-center grid grid-cols-2">
      <div class="text-[#E43C4A] font-['Shrikhand'] text-3xl">
        Blickets
      </div>
      <div class="w-full flex justify-end">
        <div
          class="text-black font-['Lato'] text-lg ml-16 cursor-pointer"
          @click="$emit('goto', 'info')"
        >
          Info
        </div>
        <div
          class="text-black font-['Lato'] text-lg ml-16 cursor-pointer"
          @click="$emit('goto', 'demo')"
        >
          Demo
        </div>
        <div
          class="text-black font-['Lato'] text-lg ml-16 cursor-pointer"
          @click="$emit('goto', 'roadmap')"
        >
          Roadmap
        </div>
      </div>
    </div>
  </header>
</template>

<script lang="ts">
export default {
  name: 'Header',
};
</script>
