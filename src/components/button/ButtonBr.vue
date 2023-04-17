<template>
    <button
    class="group h-[4rem] items-center relative flex w-full justify-center rounded-[34px] border-2 border-[#0A2640] bg-white px-3 py-2 text-2xl font-semibold text-[#0A2640] hover:bg-white focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">
    {{ title }}
  </button>
</template>
\
<script lang="ts">
import { defineComponent,  } from 'vue'

export default defineComponent({
   props: {
    title: {
      required:true,
      type: String
    }
   }
})
</script>