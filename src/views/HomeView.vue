<template>
  <header class="header">
    <headerTravel />
  </header>
  <main id="Home">
    <HomeTravel />
  </main>
  <section id="Service">
    <serviceTravel />
  </section>
  <section id="About">
    <aboutTravel />
  </section>
  <section id="Package">
    <packageTravel />
  </section>
  <section id="UptoOff">
    <uptooffTravel />
  </section>
  <footer id="Contact">
    <contactTravel />
  </footer>
</template>

<script>
// import components file :
import headerTravel from "../components/headerTravel.vue";
import HomeTravel from "../components/HomeTravel.vue";
import serviceTravel from "../components/serviceTravel.vue";
import aboutTravel from "../components/aboutTravel.vue";
import packageTravel from "../components/packageTravel.vue";
import uptooffTravel from "../components/uptooffTravel.vue";
import contactTravel from "../components/contactTravel.vue";

// import sass file :
import "../scss/travel.scss";

export default {
  name: "HomeView",
  components: {
    headerTravel,
    HomeTravel,
    serviceTravel,
    aboutTravel,
    packageTravel,
    uptooffTravel,
    contactTravel,
  },
};
</script>
