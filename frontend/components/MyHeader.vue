<template>
  <header id="header">
    <div
      class="bg-[#DEBAA7] w-full text-lg leading-9 px-1 uppercase text-center"
    >
      <p class="text-white">DELIVERY WITHIN 2-3 BUSINESS DAYS</p>
    </div>

    <nav class="bg-white border-b border-gray-200">
      <div
        class="container mx-auto flex items-center justify-center px-4 lg:px-8 h-20"
      >
        <img src="/logo.svg" alt="Logo" class="h-10 mx-5" />

        <div
          class="hidden md:flex items-center space-x-8 uppercase text-sm font-medium text-gray-700"
        >
          <a href="#" class="hover:text-gray-900">Home</a>
          <a href="#" class="hover:text-gray-900">Products</a>
          <a href="#" class="hover:text-gray-900">About us</a>
          <a href="#" class="hover:text-gray-900">Contacts</a>
        </div>

        <div class="flex items-center space-x-6 mx-5">
          <a href="#" class="text-gray-500 hover:text-gray-800">
            <i class="fa fa-bars"></i>
          </a>
          <a href="#" class="text-gray-500 hover:text-gray-800">
            <i class="fa fa-search"></i>
          </a>

          <a href="#" class="relative text-gray-500 hover:text-gray-800">
            <i class="fa fa-shopping-cart"></i>
            <span
              class="absolute top-0 right-0 bg-orange-300 text-white text-xs rounded-full px-1 -translate-y-2 translate-x-2"
              >1</span
            >
          </a>

          <a
            href="#"
            class="text-gray-500 hover:text-gray-800 flex items-center"
          >
            <i class="fa fa-user"></i>
            <span class="ml-2 hidden md:inline">Sign In</span>
          </a>
        </div>

        <button class="block md:hidden text-gray-500 hover:text-gray-800">
          <i class="fa fa-bars"></i>
        </button>
      </div>
    </nav>
  </header>
</template>
