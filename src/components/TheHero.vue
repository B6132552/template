<template>
  <div class="grid grid-flow-row auto-rows-max grid-cols-2 gap-4">
    <div class="p-38 md:p-12  ml-10 mt-20 md:p-10 sm:p-10">
      <div class="grid grid-flow-row auto-rows-max">
        <div>
          <a class="text-3xl xl:text-6xl lg:text-5xl md:text-4xl">Save time by building fast with Boldo Template</a>
        </div>
        <div class="mt-14">
          <a class="text-lg mt-20  md:text-2xl">Funding handshake buyer business-to-business metrics iPad
            partnership. First mover advantage innovator success deployment
            non-disclosure.</a>
        </div>
        <div class="mt-20">
          <div class="grid grid-flow-row auto-rows-max grid-cols-3 gap-6">
           <ButtonBgFull v-bind:title="title"/>
           <ButtonBr v-bind:title="titleBr"/>
          </div>

        </div>
      </div>
    </div>
    <div class="text-center p-32 md:p-16 sm:p-12 2xl:p-16">
      <img transition src="../assets/image/HeroGraphics.png" alt="bg" />
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent, } from "vue"
import ButtonBgFull from "./button/ButtonBgFull.vue"
import ButtonBr from "./button/ButtonBr.vue"
export default defineComponent({
  components: {ButtonBgFull, ButtonBr},
  setup(){
    const title = "Buy template"
    const titleBr = "Explore"
    return {title, titleBr}
  }
})
</script>
<style></style>
