<script setup>
defineProps({
  title: String,
  imageSrc: String,
  imageAlt: String,
  buttonText: String,
});
</script>

<template>
  <a
    href="https://tincan.ch/digital"
    target="_blank"
    rel="noopener noreferrer"
    class="cursor-pointer"
  >
    <div
      class="w-[300px] max-w-full h-auto bg-white shadow-2xl pt-6 hover:scale-105 hover:-translate-y-2 transition-all duration-500"
    >
      <h2 class="text-xl text-center font-semibold font-open-sans">
        {{ title }}
      </h2>
      <figure class="w-full my-6 px-6">
        <img
          :src="imageSrc"
          :alt="imageAlt"
          class="w-full h-full object-contain"
        />
      </figure>
      <div class="text-center text-white bg-[#FEA300] py-2 text-lg w-full">
        {{ buttonText }}
      </div>
    </div>
  </a>
</template>
