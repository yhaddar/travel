<template>
  <div class="Package">
    <h1 class="OurPackage">{{ OurPackage }}</h1>
    <div class="pkg">
      <div class="package" v-for="packages in Packages" :key="packages.id">
        <div class="PackageImg">
          <img :src="packages.packageimg" alt="" class="packageimg" />
        </div>
        <div class="PackageText">
          <h1 class="packagetitle">{{ packages.packagetitle }}</h1>
          <div class="Packagetext">
            <h1 class="packagetext">{{ packages.packagetext }}</h1>
          </div>
        </div>
        <div class="btn">
          <a href="" class="link-4">
            <button class="btn-readmore">{{ ReadMore }}</button>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "packageTravel",
  el: ".Package",
  data() {
    return {
      OurPackage: "Our Package",
      ReadMore: "Read More",
      Packages: [
        {
          id: 1,
          packageimg: require("../assets/qatar.jpg"),
          packagetitle: "Qatar Doha,",
          packagetext:
            "A multicultural city, Doha is Qatar's glittering jewel and is home to most of the country's residents as well as the expatriate population of a range of different origins. The city offers plenty of great shopping experiences with its plentiful malls, while the Corniche area dazzles visitors with its stunning architecture and dazzling views of the harbour. Doha boasts a lot of cultural facilities, including the 'Education City' and the 'National Museum', which have a bright futuristic glow.",
          packagelink:
            "https://ar.tripadvisor.com/Tourism-g294009-Doha-Vacations.html",
        },
        {
          id: 2,
          packageimg: require("../assets/Istanbul.jpg"),
          packagetitle: "Turkey Istanbul,",
          packagetext:
            "Tourism in Istanbul is characterized by the presence of the best and most beautiful tourist and recreational places such as parks, museums and beaches, which also makes Istanbul one of the best tourist cities in Turkey. The wonderful city of Istanbul is rich in the presence of the most important tourist places. Istanbul spans two continents and is one of the most visited Turkish cities. The city has many great museums, parks, beaches and hotels.",
          packagelink: "https://www.travellwd.com/tourism-in-istanbul/",
        },
        {
          id: 3,
          packageimg: require("../assets/madrid.jpg"),
          packagetitle: "Spain Madrid,",
          packagetext:
            "Madrid is considered one of the most important cities in Europe strategically, culturally and economically. It is the fourth largest city in terms of the number of tourists in Europe and the first in Spain, Madrid has a modern infrastructure, and Madrid includes the best hotels and accommodations that are located in the whole of Spain, due to its great entertainment and amenities for the convenience of its guests.",
          packagelink: "https://www.travellwd.com/tourism-in-madrid/",
        },
        {
          id: 4,
          packageimg: require("../assets/marakesh.jpg"),
          packagetitle: "Morocco Marrakesh,",
          packagetext:
            "The colorful souks, the magnificent Moroccan architecture, the distinctive gardens and the luxurious boutique hotels are all factors that allow you to have an unforgettable experience in Marrakesh. Spend the day exploring the peaceful courtyards and winding alleys of this historic city, strolling through the tranquil Majorelle Garden or admiring the beauty of the medina's mosques, before ending up in the evening in a one-of-a-kind riad.",
          packagelink:
            "https://ar.tripadvisor.com/Tourism-g293734-Marrakech_Marrakech_Safi-Vacations.html",
        },
        {
          id: 5,
          packageimg: require("../assets/cairo.jpg"),
          packagetitle: "Egypt Cairo,",
          packagetext:
            "Cairo is an ancient city that has evolved into a modern metropolis. It is considered one of the largest cities in the Middle East and has traffic and noise problems to prove it. But as long as you're not looking for solitude, Cairo - the city of a thousand minarets - is a great place to explore Egyptian history and civilization.",
          packagelink:
            "https://ar.tripadvisor.com/Tourism-g294201-Cairo_Cairo_Governorate-Vacations.html",
        },
        {
          id: 6,
          packageimg: require("../assets/paris.jpg"),
          packagetitle: "France Paris,",
          packagetext:
            "Paris is one of the world's leading tourist destinations as it is the headquarters of most French companies. Paris has a variety of museums, theaters and monuments built over the centuries, such as the Eiffel Tower, the Arc de Triomphe, the Louvre and the Palace of Versailles. Paris is one of the largest art centers in the world, with a large number of museums that include paintings by the most prominent international artists.",
          packagelink: "https://www.travellwd.com/tourism-in-paris/",
        },
      ],
    };
  },
};
</script>
