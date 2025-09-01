    <template>
        <div class="relative w-full min-h-[100dvh] flex flex-col items-center justify-center overflow-hidden">

            <div class="absolute inset-0 bg-gradient-to-br from-gray-400/40 via-white to-sky-300/30"></div>

            <div class="absolute top-20 left-20 w-32 h-32 bg-gray-900/30 rounded-full blur-3xl opacity-60 animate-float">
            </div>

            <div
                class="absolute bottom-20 right-20 w-40 h-60 bg-sky-300/70 rounded-full blur-3xl opacity-60 animate-float [animation-delay:1s]">
            </div>

            <div class="relative z-10 text-center space-y-6 flex flex-col items-center justify-center px-1 md:px-0">
                <p
                    class="text-center text-[12px] px-3 py-0.5 rounded-xl bg-blue-100 text-blue-500 font-medium border border-blue-400">
                    ✨ Disponível para novos projetos</p>
                <h1 class="md:w-4/6 text-center text-[45px] text-base/12 md:text-7xl font-bold ">
                    Tire sua ideia do papel e
                    <span class="bg-gradient-to-r from-[#0F1A41] to-sky-400 bg-clip-text text-transparent">conquiste a
                        internet</span>
                </h1>
                <p class="md:w-3/6 text-center text-lg text-gray-600 md:text-gray-500">
                    Desenvolvimento web moderno e inovador. Criando experiências digitais únicas que
                    transformam ideias em realidade digital impactante.
                </p>

                <div class="flex gap-4 justify-center py-1">
                    <button
                        class="cursor-pointer flex items-center gap-3 text-white font-medium text-sm bg-blue-900 hover:bg-[#0F1A41] px-5 md:px-8 py-3 rounded-xl outline-0 transition-colors duration-300 ease-in-out">
                        <Icon name="lucide:mail" size="18" />
                        Vamos conversar
                    </button>
                    <button
                        class="cursor-pointer flex items-center gap-2 text-gray-800 font-medium border border-gray-400 text-sm bg-white hover:bg-gray-100 hover:text-gray-900 px-5 md:px-8 py-3 rounded-xl outline-0 transition-colors duration-300 ease-in-out">Ver
                        meus projetos</button>
                </div>

                <div class="flex gap-6 justify-center py-2 ">
                    <Icon name="lucide:github" size="24"
                        class="text-gray-600 cursor-pointer transform hover:scale-105 transition-transform duration-200 ease-in-out" />
                    <Icon name="mdi:instagram" size="24"
                        class="text-gray-600 cursor-pointer transform hover:scale-105 transition-transform duration-200 ease-in-out" />
                    <Icon name="lucide:mail" size="24"
                        class="text-gray-600 cursor-pointer transform hover:scale-105 transition-transform duration-200 ease-in-out" />
                </div>

            </div>
            <div class="absolute bottom-4 left-1/2 transform -translate-x-1/2">
                <Icon name="lucide:arrow-down" size="24" class="text-gray-600 animate-bounce" />
            </div>
        </div>
    </template>

    <style>
    @keyframes float {

        0%,
        100% {
            transform: translateY(0);
        }

        50% {
            transform: translateY(-40px);
            transform: translateX(-40px);
        }
    }

    .animate-float {
        animation: float 4s ease-in-out infinite;
    }
    </style>
