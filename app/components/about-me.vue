<template>
    <div class="w-full flex flex-col md:flex-row px-10 items-center justify-center py-8">
        <div class="w-full md:w-1/2 flex flex-col gap-5 items-center justify-center">
            <div class="w-full flex flex-col gap-6 text-center md:text-start items-center md:items-start">
                <span class="text-xs font-medium text-gray-800 border border-gray-300 rounded-xl px-2 py-0.5">Sobre mim</span>
                <h2 class="text-4xl font-bold">Transformando ideias em <span class="bg-gradient-to-r from-[#0F1A41] to-sky-400 bg-clip-text text-transparent">soluções digitais inovadoras</span></h2>
                <p class="text-gray-600 text-md md:pr-1"><span class="font-bold">Desenvolvedor Front-end especializado em Nuxt.js e TailwindCSS</span>, com vasta experiência em criar aplicações web modernas e performáticas. Atualmente trabalho como <span class="font-bold">desenvolvedor autônomo</span>, criando soluções personalizadas para diversos clientes.</p>
                <p class="text-gray-600 text-md md:pr-1">Meu compromisso é entregar um código limpo e eficiente, otimizando para uma excelente performance e experiência do usuário. Utilizo as mais modernas práticas de desenvolvimento,<span class="font-bold">responsividade</span> e <span class="font-bold">acessibilidade.</span></p>
            </div>
            <ul class="w-full flex flex-row justify-center md:justify-start flex-wrap gap-10 py-3 text-center">
                <li class="flex flex-col gap-1">
                    <h3 class="text-3xl font-bold text-gray-800">50+</h3>
                    <p class="text-sm text-gray-600">Projetos Entregues</p>
                </li>
                <li class="flex flex-col gap-1">
                    <h3 class="text-3xl font-bold text-gray-800">5+</h3>
                    <p class="text-sm text-gray-600">Anos de Experiência</p>
                </li>
                <li class="flex flex-col gap-1">
                    <h3 class="text-3xl font-bold text-gray-800">100%</h3>
                    <p class="text-sm text-gray-600">Clientes Satisfeitos</p>
                </li>
                <li class="flex flex-col gap-1">
                    <h3 class="text-3xl font-bold text-gray-800">24/7</h3>
                    <p class="text-sm text-gray-600">Suporte Dedicado</p>
                </li>
            </ul>
        </div>
        <div class="w-full md:w-1/2 h-auto flex flex-row flex-wrap px-3 py-10 items-center gap-5">
            <CardAboutme :infosCard="infosCard" />
        </div>
    </div>
</template>
<script setup>
const infosCard = ref([
    {id:1, icon: 'lucide:code-xml', title: 'Código Limpo', description: 'Sigo as melhores práticas de desenvolvimento, garantindo código maintível e escalável.'},
    {id:2, icon: 'lucide:rocket', title: 'Performance', description: 'Otimização constante para entregar aplicações rápidas e eficientes.'},
    {id:3, icon: 'lucide:users', title: 'UX Focado', description: 'Design centrado no usuário para criar experiências intuitivas e envolventes.'},
    {id:4, icon: 'lucide:zap', title: 'Entrega Rápida', description: 'Metodologias ágeis para entregar projetos dentro do prazo e orçamento.'}
])
</script>