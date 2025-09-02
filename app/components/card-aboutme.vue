<template>
  <div v-for="data in infosCard" :key="data.id" class=" w-[290px] h-[212px] p-6 gap-5 shadow-xs hover:shadow-lg transition ease-in-out duration-300 border border-gray-200 hover:border-gray-300 rounded-2xl bg-gradient-to-r from-white to-gray-50">
    <div class="w-12 h-12 bg-gray-200 rounded-2xl flex items-center justify-center">
      <Icon :name="data.icon" size="25" class="text-gray-800"/>
    </div>
    <div class="flex flex-col gap-2 py-4">
      <p class="font-medium text-gray-900">{{ data.title }}</p>
      <p class="text-sm text-gray-500">{{ data.description }}</p>
    </div>
  </div>
</template>

<script setup>
defineProps({
  infosCard: Array
})
</script>
