<template>
  <div class="bg-[#0f977f]">
    <div
      class="flex items-center justify-center min-h-screen"
      v-for="image in images"
    >
      <div class="space-y-3">
        <div class="flex justify-center">
          <div class="text-xl font-bold text-white">Halo.</div>
        </div>
        <div class="w-[230px] h-[130px]">
          <img
            :src="image.src"
            alt=""
            class="w-full h-full"
            ref="storeImages"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const storeImages = ref([]);

const images = [
  {
    src: "/public/baseball-svgrepo-com.svg",
    alt: "",
  },
];
</script>

<style lang="scss" scoped></style>
