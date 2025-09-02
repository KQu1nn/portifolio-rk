<template>
  <div class="w-full min-h-[100dvh] flex flex-col gap-10 bg-white py-10 md:py-20 md:px-5">
    <div class="flex flex-col items-center gap-5 py-5">
      <p class="text-xs font-medium text-gray-800 border border-gray-300 rounded-xl px-2 py-0.5">Meus Projetos</p>
      <h3 class="text-4xl text-center font-bold">Projetos que fazem a <span class="bg-gradient-to-r from-[#0F1A41] to-sky-400 bg-clip-text text-transparent">diferença</span></h3>
      <p class="md:w-3/6 w-5/6 text-center text-gray-600 md:text-gray-500 py-2">Cada projeto é uma oportunidade de criar algo excepcional. Confira alguns dos trabalhos que trouxeram resultados reais para meus clientes.</p>
    </div>

    <div class="flex flex-col md:flex-row gap-10 justify-center md:py-10 px-5">
      <ProjectsCard :products="products" />
    </div>

    <div class="w-full flex justify-center ">
      <button class="border border-gray-300 rounded-xl text-sm font-medium text-gray-900 px-8 py-2 cursor-pointer outline-0 hover:bg-gray-100 hover:scale-102 transition-colors duration-300 ease-in-out ">Ver todos os projetos</button>
    </div>
  </div>
</template>

<script setup>
  import image1 from '@/assets/images/image1.jpg'
  import image2 from '@/assets/images/image2.jpg'
  import image3 from '@/assets/images/image3.jpg'

  const products = ref([
    {id: 1, title: 'Plataforma SaaS Completa', description: 'Sistema completo de gestão empresarial com dashboard analytics, autenticação avançada e integração com APIs externas.', image: image1, category: 'Full Stack', url: '#' },
    {id: 2, title: 'E-commerce Moderno', description: 'Loja virtual responsiva com carrinho de compras, sistema de pagamento integrado e painel administrativo.', image: image2, category: 'E-commerce', url: '#' },
    {id: 3, title: 'App Mobile Financeiro', description: 'Aplicativo de controle financeiro com gráficos interativos, sincronização em tempo real e notificações push.', image: image3, category: 'Mobile', url: '#' },
  ])
</script>