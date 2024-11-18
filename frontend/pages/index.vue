<template>
  <MyHeader />
  <Hero />
  <MovingText />
  <ProductRow
    title="SUNTAN"
    subtitle="Natural, organic oils for super tan and glowing skin"
    :products="suntans"
  />
  <ProductRow
    class="bg-[#FBF1EB]"
    title="SHIMMER"
    subtitle="Natural products for elegant glow and skincare"
    :products="shimmers"
  />
  <Newsletter />
</template>

<script setup>
onMounted(() => {
  const header = document.getElementById("header");
  window.addEventListener("scroll", () => {
    if (window.scrollY > 0) {
      header?.classList.add("scrolling");
    } else {
      header?.classList.remove("scrolling");
    }
  });
});

const suntans = [
  {
    title: "WATERMELON",
    subtitle: "Suntan & Body Oil",
    image: "/watermelon-500x500-min.png",
    priceOptions: [{ price: "€32.00", size: "110ml" }],
    stars: 5,
    reviews: 232,
    description:
      "For a fast, deep tan and radiant skin. With juicy watermelon aroma.",
  },
  {
    title: "CHOCO",
    subtitle: "Suntan & Body Oil",
    image: "/choco-thumb-500x500-min.png",
    priceOptions: [
      { price: "€32.00", size: "110ml" },
      { price: "€45.00", size: "200ml" },
    ],
    stars: 5,
    reviews: 3088,
    description:
      "Get a quick and deep chocolate tan with this organic body oil. Suitable for everyday use.",
  },
  {
    title: "COOL",
    subtitle: "After Sun Oil",
    image: "/cool-thumb-500x500-min.png",
    priceOptions: [
      { price: "€32.00", size: "110ml" },
      { price: "€45.00", size: "200ml" },
    ],
    stars: 5,
    reviews: 531,
    description:
      "Replenish your skin after sun exposure with this organic body oil. Suitable for everyday use.",
  },
];

const shimmers = [
  {
    title: "AURA",
    subtitle: "Peptide Shimmer Spray",
    image: "/aura-thumb-500x500-min-shadow.png",
    priceOptions: [{ price: "€36.00", size: "110ml" }],
    stars: 5,
    reviews: 60,
    description:
      "Natural shimmer spray with peptides for face, body & hair. Illuminates, hydrates, rejuvenates.",
  },
  {
    title: "GLOW",
    subtitle: "Shimmer Oil",
    image: "/glow-thumb-500x500-min.png",
    priceOptions: [{ price: "€34.00", size: "110ml" }],
    stars: 5,
    reviews: 914,
    description: "Natural glowing and hydrating dry oil with shiny particles.",
  },
  {
    title: "NOUGAT",
    subtitle: "Sparkling Body Butter",
    image: "/nougat-thumb-500x500-min.png",
    priceOptions: [{ price: "€70.00", size: "110ml" }],
    stars: 5,
    reviews: 155,
    description:
      "Premium skincare. Melting organic mousse. Evens the tan and makes the skin radiant. With aroma of a delicious gourmet dessert.",
  },
];
</script>
