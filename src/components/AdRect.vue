<script setup>
defineProps({
  title: String,
  imageSrc: String,
  imageAlt: String,
  buttonText: String,
});
</script>

<template>
  <div class="w-[300px] h-auto bg-white shadow-2xl pt-6">
    <p class="text-xl text-center font-semibold font-open-sans">
      {{ title }}
    </p>
    <figure class="w-full px-6 my-6">
      <img
        :src="imageSrc"
        :alt="imageAlt"
        class="w-full h-full object-contain"
      />
    </figure>
    <button class="text-center text-white bg-[#FEA300] py-2 text-lg w-full">
      {{ buttonText }}
    </button>
  </div>
</template>
