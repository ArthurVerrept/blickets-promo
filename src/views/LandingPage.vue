<template>
  <div>
    <div class="mx-36 grid grid-cols-2">
      <div class="flex justify-center pt-24">
        <div class="flex flex-col">
          <h1
            class="font-['Paytone_One'] max-w-xl text-8xl pt-10"
          >
            Get more out of each
          </h1>
          <h1 class="font-['Paytone_One'] max-w-xl text-8xl pb-8">
            {{ word }}
          </h1>
          <p
            class="max-w-md font-['Lato']"
          >
            By putting your tickets to the blockchain using our service,
            you provide both yourself and the customer
            a huge set of benefits that you could not get otherwise.
          </p>
        </div>
      </div>
      <div>
        <img
          class="max-w-md ml-24"
          src="../assets/aaa.png"
          alt="image of phone with app"
        >
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'LandingPage',
  data() {
    return {
      word: '',
      words: [
        'ticket.',
        'purchase.',
        'event.',
        'experience.',
        'sale.',
      ],
    };
  },
  mounted() {
    [this.word] = this.words;
    let i = 0;
    window.setInterval(() => {
      this.word = this.words[i];
      i += 1;
      if (i >= this.words.length) {
        i = 0;
      }
    }, 1200);
  },
});

</script>
