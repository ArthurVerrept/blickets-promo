<template>
  <main class="relative h-screen ">
    <Header />
    <LandingPage />
    <Info />
    <AppDemo />
    <Roadmap />
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
};
</script>
