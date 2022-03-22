<template>
  <div class="bg-black mt-20">
    <div class="mx-36 py-10 flex gap-4">
      <div class="flex flex-col">
        <span
          class="font-['Lato'] transition py-1 ease-in-out duration-300 font-bold
        text-white rounded cursor-pointer"
          @click="openEmail()"
        >Contact</span>
        <span
          class="font-['Lato'] transition ease-in-out duration-300
        text-neutral-500 rounded cursor-default"
        >Download</span>
      </div>
      <div class="grow flex justify-center">
        <span
          class="font-['Lato'] transition ease-in-out duration-300 font-bold
         text-neutral-700 rounded cursor-pointer pt-7"
        >Blickets, All rights reserved</span>
      </div>
      <div class="flex flex-col justify-center">
        <span
          class="font-['Lato'] transition ease-in-out duration-300
        text-neutral-500 rounded cursor-default"
        >View online experience</span>
        <span
          class="font-['Lato'] transition ease-in-out duration-300
        text-black rounded cursor-default"
        >A</span>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: 'Contact',
  methods: {
    openEmail() {
      window.location.href = 'mailto:arthur-verrept@hotmail.co.uk?subject=Blickets Enquiry&body=';
    },
  },
};
</script>
