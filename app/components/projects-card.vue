<template>
  <div 
  v-for="product in products" 
  :key="product.id"
  class="cursor-pointer transform transition-transform duration-300 hover:-translate-y-2 hover:shadow-lg relative min-h-[395px] w-full md:w-[400px] border rounded-2xl border-gray-200 bg-gray-50 group overflow-hidden">
    
    <span class="absolute top-3 left-3 bg-[#191747] text-white text-xs font-semibold px-3 py-1 rounded-full z-10">
      {{ product.category }}
    </span>

    <div class="h-[192px] w-full relative overflow-hidden">
      <img 
        class="h-[192px] w-full object-cover rounded-t-2xl transition-transform duration-300 group-hover:scale-105" 
        :src="product.image"
      >
      <div class="absolute inset-0 bg-violet-900/60 bg-opacity-50 flex items-center justify-center opacity-0 transition-opacity duration-300 group-hover:opacity-100">
        <button class="bg-white text-violet-900 font-semibold px-4 py-2 rounded-md hover:bg-gray-100 cursor-pointer">
          Ver Demo
        </button>
      </div>
    </div>

    <div class="w-full px-6 py-7 flex flex-col gap-3">
      <h3 class="text-xl font-medium text-gray-900">{{ product.title }}</h3>
      <p class="text-gray-500">{{ product.description }}</p>
    </div>

    <ul class="flex flex-row gap-2 px-6 pb-5">
      <li class="text-white text-xs font-medium bg-violet-900 px-2 py-0.5 rounded-xl">Nuxt.js</li>
      <li class="text-white text-xs font-medium bg-violet-900 px-2 py-0.5 rounded-xl">Javascript</li>
      <li class="text-white text-xs font-medium bg-violet-900 px-2 py-0.5 rounded-xl">TailwindCSS</li>
      <li class="text-white text-xs font-medium bg-violet-900 px-2 py-0.5 rounded-xl">Supabase</li>
    </ul>

  </div>
</template>

<script setup>
defineProps({
  products: {
    type: Array,
    required: true
  }
})
</script>
