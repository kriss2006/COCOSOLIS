<template>
  <div class="flex flex-col items-center text-center p-6">
    <a href="#" class="mb-6">
      <img :src="product.image" :alt="product.title" class="h-40 mx-auto" />
    </a>

    <div class="mb-4">
      <p class="text-lg font-bold text-[#816c65]">{{ product.title }}</p>
      <p class="text-sm text-[#816c65]">{{ product.subtitle }}</p>
    </div>

    <div class="flex items-center justify-center mb-4">
      <img
        v-for=" in product.stars"
        src="/star.png"
        alt="Rating Stars"
        class="h-4 mr-2"
      />
      <span class="text-sm text-[#816c65]">{{ product.reviews }} reviews</span>
    </div>

    <div class="mb-6 text-sm text-[#816c65]">
      <p>{{ product.description }}</p>
    </div>

    <div class="w-full flex flex-wrap gap-4 justify-center">
      <div
        v-for="(option, index) in product.priceOptions"
        :key="index"
        class="w-full sm:w-[48%] flex flex-col items-center border-t pt-4"
      >
        <div class="mb-2">
          <span class="text-lg font-medium text-[#816c65]">{{
            option.price
          }}</span>
          <span class="text-sm text-[#816c65]">/ {{ option.size }}</span>
        </div>

        <a
          href="#"
          class="bg-[#816c65] text-white text-xs font-medium uppercase py-2 px-6 transition w-full text-center"
        >
          Add
        </a>
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps({
  product: {
    type: Object,
    required: true,
  },
});
</script>
