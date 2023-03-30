<template>
  <div class="div">
    <h1 class="OurService">{{ text }}</h1>
    <div class="Activities">
      <div
        class="activities"
        v-for="activitie in activities"
        :key="activitie.id"
      >
        <img :src="activitie.img" alt="" class="imglogo" />
        <h1 class="servicetext">{{ activitie.text }}</h1>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "serviceTravel",
  el: ".div",
  data() {
    return {
      text: "Our Service",
      activities: [
        {
          id: 1,
          img: require("../assets/adventure.png"),
          text: "Adventure",
        },
        {
          id: 2,
          img: require("../assets/tourguid.png"),
          text: "Tour Guid",
        },
        {
          id: 3,
          img: require("../assets/trekking.png"),
          text: "Trekking",
        },
        {
          id: 4,
          img: require("../assets/campfire.png"),
          text: "Camp Fire",
        },
        {
          id: 5,
          img: require("../assets/offroad.png"),
          text: "Off Road",
        },
        {
          id: 6,
          img: require("../assets/camping.png"),
          text: "Camping",
        },
      ],
    };
  },
};
</script>
