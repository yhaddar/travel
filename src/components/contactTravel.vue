<template>
  <div class="Contact">
    <h1 class="contactUS">{{ title }}</h1>
  </div>
  <div class="contact">
    <div class="contacts" v-for="Contact in Contacts" :key="Contact.id">
      <h1 class="title-contact">{{ Contact.titles }}</h1>
      <ul class="ul-contact">
        <li class="li-contact">
          <a :href="Contact.link1" class="link-contact">{{ Contact.li1 }}</a>
        </li>
        <li class="li-contact">
          <a :href="Contact.link2" class="link-contact">{{ Contact.li2 }}</a>
        </li>
        <li class="li-contact">
          <a :href="Contact.link3" class="link-contact">{{ Contact.li3 }}</a>
        </li>
        <li class="li-contact">
          <a :href="Contact.link4" class="link-contact">{{ Contact.li4 }}</a>
        </li>
      </ul>
    </div>
  </div>
  <hr class="hr" />
  <div class="textfinal">
    <h3 class="copyright">© 2022 Copyright: Travel.com</h3>
  </div>
</template>
<script>
export default {
  name: "contactTravel",
  el: ".contact",
  data() {
    return {
      title: "Contact Us",
      Contacts: [
        {
          titles: "Quick links",
          id: 1,
          li1: "> Home",
          li2: "> Service",
          li3: "> About",
          li4: "> Package",
          link1: "#Home",
          link2: "#Service",
          link3: "#About",
          link4: "#Package",
        },
        {
          titles: "Extra Links",
          id: 2,
          li1: "> Need Help ?",
          li2: "> About Us",
          li3: "> Privacy Policy",
          li4: "> Terms Of Use",
          link1: "#",
          link2: "#",
          link3: "#",
          link4: "#",
        },
        {
          titles: "Contact Info",
          id: 3,
          li1: " > +39 612 304 560 ",
          li2: " > +39 614 789 526",
          li3: " > xyzexemple@gmail.com",
          li4: "> Via Laurentina, 865, 00143 Roma RM, Italie",
          link1: "#",
          link2: "#",
          link3: "#",
          link4: "#",
        },
        {
          titles: "Contact Info",
          id: 4,
          li1: "> Facebook",
          li2: "> Twitter",
          li3: "> Instagram",
          li4: "> Linkedin",
          link1: "#",
          link2: "#",
          link3: "#",
          link4: "#",
        },
      ],
    };
  },
};
</script>
