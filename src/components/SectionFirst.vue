<template>
  <div class="bg-[#0A2640] p-24">
    <div class="grid grid-rows-2 gap-4">
      <div class="flex justify-center">
        <a class="text-[#F1F1F1] text-2xl"> Our Team </a>
      </div>
      <div class="flex justify-center">
        <a class="text-white text-4xl">
          Handshake infographic mass market crowdfunding iteration.
        </a>
      </div>
    </div>
    <div class="gap-10 flex justify-center columns-3 mt-20 p-12">
      <div v-for="item in items" v-bind:key="item.id">
        <CardImage
          v-bind:image="item.image"
          v-bind:name="item.name"
          v-bind:position="item.position"
        />
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import CardImage from "./card/CardImage.vue";

export default defineComponent({
  components: { CardImage },
  setup() {
    const items = [
      {
        id: 1,
        name: "Michael Scott",
        position: "General Manager",
        image:
          "https://img.freepik.com/premium-photo/generative-ai-adorable-boy-astronaut-outer-space-standing-planet-bright-colorful-asteroids-galaxies-moonlight-shining-down-chibi-style-emblem-space-travel-technology-cuteness_620624-6177.jpg",
      },
      {
        id: 2,
        name: "Dwight Schrute",
        position: "General Manager",
        image:
          "https://img.freepik.com/premium-photo/generative-ai-adorable-boy-astronaut-outer-space-standing-planet-bright-colorful-asteroids-galaxies-moonlight-shining-down-chibi-style-emblem-space-travel-technology-cuteness_620624-6177.jpg",
      },
      {
        id: 3,
        name: "Pam Beetsley",
        position: "General Manager",
        image:
          "https://img.freepik.com/premium-photo/generative-ai-adorable-boy-astronaut-outer-space-standing-planet-bright-colorful-asteroids-galaxies-moonlight-shining-down-chibi-style-emblem-space-travel-technology-cuteness_620624-6177.jpg",
      },
    ];
    return { items };
  },
});
</script>
