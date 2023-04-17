<template>
    <div class="max-w-xs rounded overflow-hidden">
        <img
          class="w-full rounded-xl"
          :src="image"
          alt="Sunset in the mountains"
        />
        <div class="pt-6">
          <div class="font-bold text-2xl mb-2 text-white">{{name}}</div>
          <p class="text-white text-xl">{{position}}</p>
        </div>
      </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    image:{
        required: true,
        type: String
    },
    name:{
        required: true,
        type: String
    },
    position:{
        required: true,
        type: String
    }
  }
})
</script>
