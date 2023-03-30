<template>
  <div class="About">
    <h1 class="about">{{ About }}</h1>
  </div>
  <div class="ABOUT">
    <div class="Aboutimg"></div>
    <div class="textabout">
      <h1 class="abouttitle">{{ About }}</h1>
      <h2 class="abouttext">{{ aboutText }}</h2>
    </div>
  </div>
</template>
<script>
export default {
  name: "aboutTravel",
  el: ".About",
  data() {
    return {
      About: "About Us",
      aboutText: `Travel Services, travel agency, operating in Rome, Italy, since 2020.
        We are able to offer a variety of solutions to travelers in some countries such as Spain, Turkey, Egypt...
        Offers hotel and golf reservations, airport transfers, tours, and much more. From individual travelers to tour operators, we have the right solution for your requirements.`,
    };
  },
};
</script>
