<template>
  <div class="UptoOff">
    <h1 class="uptooff">{{ title }}</h1>
    <h1 class="uptoofftext">{{ text }}</h1>
    <div class="link-5">
      <button class="btn-reservation">{{ textbtn }}</button>
    </div>
  </div>
</template>
<script>
export default {
  name: "uptooffTravel",
  el: "UptoOff",
  data() {
    return {
      title: "Upto 30% Off",
      text: "30% discount for two or more people with the right to a room for each one",
      textbtn: "Book Now",
    };
  },
};
</script>
