<template>
  <section id="products" class="py-16 px-4">
    <div class="text-center mb-10">
      <h2 class="text-3xl font-light text-gray-800">{{ title }}</h2>
      <p class="text-lg font-medium text-gray-600 mt-2">{{ subtitle }}</p>
    </div>

    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
      <ProductItem
        v-for="(product, index) in products"
        :key="index"
        :product="product"
      />
    </div>
  </section>
</template>

<script setup>
defineProps({
  title: {
    type: String,
    required: true,
  },
  subtitle: {
    type: String,
    required: true,
  },
  products: {
    type: Array,
    required: true,
  },
});
</script>
