<template>
  <nav class="nav">
    <div class="logo">
      <h1 class="logo-txt">{{ logo }}</h1>
    </div>
    <ul class="ul">
      <li class="li" v-for="link in links" :key="link.id">
        <a v-bind:href="link.link" class="link">{{ link.name }}</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "headerTravel",
  data() {
    return {
      links: [
        {
          id: 1,
          link: "#Home",
          name: "Home",
        },
        {
          id: 2,
          link: "#Service",
          name: "Service",
        },
        {
          id: 3,
          link: "#About",
          name: "About",
        },
        {
          id: 4,
          link: "#Package",
          name: "Package",
        },
        {
          id: 5,
          link: "#Contact",
          name: "Contact",
        },
      ],
      logo: "TRAVEl",
    };
  },
};
</script>
