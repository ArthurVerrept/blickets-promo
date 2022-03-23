<template>
  <main
    ref="home"
    class="relative h-screen"
  >
    <Header @goto="(n: string) => goto(n)" />
    <LandingPage />
    <Info id="info" />
    <AppDemo id="demo" />
    <Roadmap id="roadmap"/>
    <Contact />
  </main>
</template>

<script lang='ts'>
import Header from '../components/Header.vue';
import LandingPage from './LandingPage.vue';
import Info from './Info.vue';
import AppDemo from './AppDemo.vue';
import Roadmap from './Roadmap.vue';
import Contact from './Contact.vue';

export default {
  name: 'Home',
  components: {
    Header,
    LandingPage,
    Info,
    AppDemo,
    Roadmap,
    Contact,
  },

  methods: {
    goto(refName: string) {
      console.log(refName);
      const element = document.getElementById(refName);
      console.log(element);
      const { top } = element!.getBoundingClientRect();
      console.log(top);
      window.scrollTo(0, top);
    },
  },
};
</script>
