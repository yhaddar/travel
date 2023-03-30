<template>
  <div class="text">
    <h1 class="text-1">{{ text1 }}</h1>
    <h1 class="text-2">{{ text2 }}</h1>
    <div class="link-2">
      <button class="btn-1">{{ textbtn }}</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  el: ".text",
  data() {
    return {
      text1: "Wherever You Want",
      text2: "Don't miss the chance",
      textbtn: "Fill out The form here",
    };
  },
};
// document.querySelector(".btn-1").addEventListener("click", () => {
//   alert("hello");
// });
</script>
