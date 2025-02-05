<script setup>
import { ref } from 'vue';

const isActive = ref(false);
const toggleInsulto = () => {
  isActive.value = !isActive.value;
  console.log(isActive.value);

  // Después de 2 segundos, cambia isActive a false
  setTimeout(() => {
    isActive.value = false;
    console.log(isActive.value); // Verificar el cambio
  }, 2000);
};

import { defineEmits } from 'vue'

const emit = defineEmits(['pause-audio'])

const triggerPause = (audioNumber) => {
  emit('pause-audio', audioNumber)
}

</script>
<template>

    <body>

        <div class="night"></div>

        <div class="bubbles">
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
            <div class="bubble"><svg class="heart" viewBox="0 0 32 32">
                    <title>heart22</title>
                    <path
                        d="M23.6 2c-3.363 0-6.258 2.736-7.599 5.594-1.342-2.858-4.237-5.594-7.601-5.594-4.637 0-8.4 3.764-8.4 8.401 0 9.433 9.516 11.906 16.001 21.232 6.13-9.268 15.999-12.1 15.999-21.232 0-4.637-3.763-8.401-8.4-8.401z">
                    </path>
                </svg>
            </div>
        </div>

        <!-- partial -->
        
        <div class="fixed inset-0 flex items-center justify-center z-50">
            <div class="w-full max-w-md bg-white shadow-xl rounded-lg overflow-hidden">
                <div class="relative h-60 bg-cover bg-center"
                    style="background-image: url('https://res.cloudinary.com/djfokdod6/image/upload/v1738712685/IMG_0814_npt4fx.jpg')">
                    <div class="absolute inset-0 bg-black opacity-30"></div>
                    <div class="absolute inset-0 flex items-center justify-center">
                        <h2 class="text-3xl font-bold text-white text-center px-4">Noche de películas</h2>
                    </div>
                </div>
                <div class="p-6">
                    <div class="space-y-4">
                        <div class="flex items-center gap-3">
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                                stroke="currentColor" class="size-6">
                                <path stroke-linecap="round" stroke-linejoin="round"
                                    d="M6.75 3v2.25M17.25 3v2.25M3 18.75V7.5a2.25 2.25 0 0 1 2.25-2.25h13.5A2.25 2.25 0 0 1 21 7.5v11.25m-18 0A2.25 2.25 0 0 0 5.25 21h13.5A2.25 2.25 0 0 0 21 18.75m-18 0v-7.5A2.25 2.25 0 0 1 5.25 9h13.5A2.25 2.25 0 0 1 21 11.25v7.5" />
                            </svg>
                            <span class="text-gray-700">Viernes 14 de Julio</span>
                        </div>
                        <div class="flex items-center gap-3">
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                                stroke="currentColor" class="size-6">
                                <path stroke-linecap="round" stroke-linejoin="round"
                                    d="M12 6v6h4.5m4.5 0a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z" />
                            </svg>
                            <span class="text-gray-700">Decidiremos</span>
                        </div>
                        <div class="flex items-center gap-3">
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                                stroke="currentColor" class="size-6">
                                <path stroke-linecap="round" stroke-linejoin="round"
                                    d="M3.375 19.5h17.25m-17.25 0a1.125 1.125 0 0 1-1.125-1.125M3.375 19.5h1.5C5.496 19.5 6 18.996 6 18.375m-3.75 0V5.625m0 12.75v-1.5c0-.621.504-1.125 1.125-1.125m18.375 2.625V5.625m0 12.75c0 .621-.504 1.125-1.125 1.125m1.125-1.125v-1.5c0-.621-.504-1.125-1.125-1.125m0 3.75h-1.5A1.125 1.125 0 0 1 18 18.375M20.625 4.5H3.375m17.25 0c.621 0 1.125.504 1.125 1.125M20.625 4.5h-1.5C18.504 4.5 18 5.004 18 5.625m3.75 0v1.5c0 .621-.504 1.125-1.125 1.125M3.375 4.5c-.621 0-1.125.504-1.125 1.125M3.375 4.5h1.5C5.496 4.5 6 5.004 6 5.625m-3.75 0v1.5c0 .621.504 1.125 1.125 1.125m0 0h1.5m-1.5 0c-.621 0-1.125.504-1.125 1.125v1.5c0 .621.504 1.125 1.125 1.125m1.5-3.75C5.496 8.25 6 7.746 6 7.125v-1.5M4.875 8.25C5.496 8.25 6 8.754 6 9.375v1.5m0-5.25v5.25m0-5.25C6 5.004 6.504 4.5 7.125 4.5h9.75c.621 0 1.125.504 1.125 1.125m1.125 2.625h1.5m-1.5 0A1.125 1.125 0 0 1 18 7.125v-1.5m1.125 2.625c-.621 0-1.125.504-1.125 1.125v1.5m2.625-2.625c.621 0 1.125.504 1.125 1.125v1.5c0 .621-.504 1.125-1.125 1.125M18 5.625v5.25M7.125 12h9.75m-9.75 0A1.125 1.125 0 0 1 6 10.875M7.125 12C6.504 12 6 12.504 6 13.125m0-2.25C6 11.496 5.496 12 4.875 12M18 10.875c0 .621-.504 1.125-1.125 1.125M18 10.875c0 .621.504 1.125 1.125 1.125m-2.25 0c.621 0 1.125.504 1.125 1.125m-12 5.25v-5.25m0 5.25c0 .621.504 1.125 1.125 1.125h9.75c.621 0 1.125-.504 1.125-1.125m-12 0v-1.5c0-.621-.504-1.125-1.125-1.125M18 18.375v-5.25m0 5.25v-1.5c0-.621.504-1.125 1.125-1.125M18 13.125v1.5c0 .621.504 1.125 1.125 1.125M18 13.125c0-.621.504-1.125 1.125-1.125M6 13.125v1.5c0 .621-.504 1.125-1.125 1.125M6 13.125C6 12.504 5.496 12 4.875 12m-1.5 0h1.5m-1.5 0c-.621 0-1.125.504-1.125 1.125v1.5c0 .621.504 1.125 1.125 1.125M19.125 12h1.5m0 0c.621 0 1.125.504 1.125 1.125v1.5c0 .621-.504 1.125-1.125 1.125m-17.25 0h1.5m14.25 0h1.5" />
                            </svg>

                            <span class="text-gray-700">Star Wars 3</span>
                        </div>
                    </div>
                    <div class="mt-8 flex justify-center items-center flex-col">
                        <button
                        @click="toggleInsulto"
                            class="bg-red-500 text-white font-semibold py-2 px-6 rounded-full hover:bg-red-600 transition duration-300 ease-in-out transform hover:-translate-y-1 hover:scale-105 focus:outline-none focus:ring-2 focus:ring-red-500 focus:ring-opacity-50">
                            Confirmar Asistencia
                        </button>
                        <button class="mt-1" @click="triggerPause(2)">Pausar</button>
                    </div>
                </div>
                <div class="bg-gray-50 px-6 py-4">
                    <p class="text-gray-600 text-sm text-center italic">
                        Are you a tamal? because es ta mal that you're not with me
                    </p>
                </div>
            </div>
        </div>
        <div :class="isActive ? 'insulto' : 'hidden'"
            class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 z-50">
            <svg width="48px" height="48px" viewBox="0 0 80 80" fill="none" xmlns="http://www.w3.org/2000/svg">
                <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
                <g id="SVGRepo_iconCarrier">
                    <path
                        d="M55.8624 68.7922C55.8624 65.8071 56.1166 61.5245 56.1166 59.5125C56.1166 57.5005 58.7774 55.0808 58.7774 45.6433C58.7774 36.2058 55.4679 34.2727 53.0483 34.3516C50.6286 34.4305 50.3305 32.5457 47.718 32.0416C45.7104 31.6515 45.3203 32.6333 44.0316 32.6333C42.7428 32.6333 42.0722 30.7222 39.898 30.7222C37.7238 30.7222 35.9485 32.4142 35.9485 32.4142C35.9485 32.4142 35.2384 31.3709 31.5914 31.498C26.8749 31.6602 27.4359 37.3061 27.4359 40.392C27.4359 43.4779 27.357 36.6749 27.357 36.6749C27.357 36.6749 19.9622 34.1763 21.1238 45.0779C21.2597 46.3578 19.857 56.1066 32.078 60.81C32.078 60.81 33.3974 61.2132 31.8544 69.9056C31.8544 69.9056 32.5163 73.9997 42.8656 73.9997C53.9907 73.9953 55.8624 68.7922 55.8624 68.7922Z"
                        fill="url(#paint0_linear)"></path>
                    <path
                        d="M35.9487 32.4145C35.9487 32.4145 37.1979 31.2266 38.8812 30.8408C38.0483 31.1214 36.4484 33.0588 35.7689 34.1109C35.7689 34.1109 33.2485 31.4194 31.5872 31.4983C35.129 31.3405 35.9487 32.4145 35.9487 32.4145Z"
                        fill="url(#paint1_linear)"></path>
                    <path
                        d="M47.3982 31.989C46.8459 31.9496 46.9818 33.3479 44.343 33.4882C44.343 33.4882 42.7387 32.6334 44.0274 32.6334C45.2504 32.629 45.6668 31.7567 47.3982 31.989Z"
                        fill="url(#paint2_linear)"></path>
                    <path
                        d="M54.7665 65.4653C54.3413 58.2677 48.8971 63.4007 54.7051 55.664C58.0234 51.2411 57.1861 42.9608 56.8223 39.6952C56.4585 36.4295 53.675 35.7632 51.7375 35.2811C50.0587 34.8603 49.4231 32.6905 48.0686 32.125C50.3611 32.7255 50.7425 34.4307 53.0482 34.3518C55.4678 34.2729 58.7773 36.206 58.7773 45.6435C58.7773 55.081 56.1166 57.5006 56.1166 59.5126C56.1166 61.5246 55.8623 65.8072 55.8623 68.7923C55.8623 68.7923 55.218 70.5807 52.4389 72.0623C52.9474 70.3528 54.9155 68.0734 54.7665 65.4653Z"
                        fill="url(#paint3_radial)"></path>
                    <path
                        d="M32.078 60.8104C25.6957 58.3557 23.4514 53.4244 22.0137 48.4404C24.898 56.2648 32.5032 58.816 33.5903 60.4466C34.5941 61.9545 35.3437 66.5483 32.6961 71.2912C31.9553 70.5285 31.8545 69.9017 31.8545 69.9017C33.3974 61.2093 32.078 60.8104 32.078 60.8104Z"
                        fill="url(#paint4_radial)"></path>
                    <path
                        d="M43.5581 73.9913C42.6946 68.626 46.6309 63.642 46.6309 55.4363C46.6309 46.424 52.5047 41.6942 49.261 32.603C50.5935 33.3438 51.2116 34.4134 53.0482 34.352C55.4679 34.2731 58.7774 36.2062 58.7774 45.6437C58.7774 55.0812 56.1166 57.5009 56.1166 59.5128C56.1166 61.5248 55.8624 65.8074 55.8624 68.7925C55.8624 68.7925 54.0652 73.7765 43.5581 73.9913Z"
                        fill="url(#paint5_radial)"></path>
                    <path
                        d="M34.252 35.3997C36.7944 35.3997 38.2453 34.5537 40.3011 34.5537C42.3569 34.5537 49.011 35.7986 49.011 40.239C49.011 44.6794 45.3815 53.6917 41.3882 54.8314C37.3949 55.9667 30.2981 50.5137 29.6932 46.8799C29.0883 43.246 30.2587 35.3997 34.252 35.3997Z"
                        fill="url(#paint6_radial)"></path>
                    <path
                        d="M44.3428 34.0101C44.3428 34.0101 44.3735 20.1541 44.3735 15.8013C44.3735 11.4442 44.7373 6 40.0164 6C35.2954 6 35.8609 11.808 35.8609 14.894C35.8609 17.9799 35.782 36.6752 35.782 36.6752"
                        fill="url(#paint7_linear)"></path>
                    <path
                        d="M44.3428 33.484C43.7203 33.5323 42.9971 32.98 42.9971 29.9948C42.9971 27.0097 42.756 15.4901 42.756 10.8393C42.756 8.05582 41.6777 6 40.0164 6C44.7329 6 44.3735 11.4442 44.3735 15.8013C44.3735 20.1584 44.3472 32.6117 44.3472 32.6117V33.484H44.3428Z"
                        fill="url(#paint8_linear)"></path>
                    <path
                        d="M40.0163 34.1989C36.5315 34.1989 38.2498 21.1451 38.2498 19.1199C38.2498 17.0948 36.7331 9.60791 39.5648 9.60791C40.9807 9.60791 42.1949 12.9481 41.2831 19.5232C40.3757 26.1027 43.5011 34.1989 40.0163 34.1989Z"
                        fill="url(#paint9_radial)"></path>
                    <path
                        d="M23.7493 36.8152C25.3931 39.8047 26.787 43.5613 27.5015 47.8308V42.3909L27.2867 36.6487C26.9316 36.5435 25.2747 36.1226 23.7493 36.8152Z"
                        fill="url(#paint10_radial)"></path>
                    <path
                        d="M27.471 36.7193L27.3614 36.6755C27.3614 36.6755 26.5812 36.4125 25.5686 36.43C25.7308 37.1095 25.836 37.8152 25.8711 38.5472C26.0639 42.6939 27.6463 48.0461 27.6463 48.0461L27.471 36.7193Z"
                        fill="url(#paint11_radial)"></path>
                    <path
                        d="M27.6814 48.3437C27.6814 48.3437 27.471 36.7977 27.471 36.7188C27.471 36.7188 27.3132 36.5566 26.8924 36.5566C26.7565 36.5566 26.6293 45.0298 27.6814 48.3437Z"
                        fill="#975500"></path>
                    <defs>
                        <linearGradient id="paint0_linear" x1="51.8136" y1="68.5334" x2="33.3908" y2="32.089"
                            gradientUnits="userSpaceOnUse">
                            <stop offset="0.00132565" stop-color="#FFCB4B"></stop>
                            <stop offset="1" stop-color="#FFD748"></stop>
                        </linearGradient>
                        <linearGradient id="paint1_linear" x1="42.018" y1="30.6739" x2="26.9398" y2="34.5313"
                            gradientUnits="userSpaceOnUse">
                            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
                            <stop offset="1" stop-color="#E68E43"></stop>
                        </linearGradient>
                        <linearGradient id="paint2_linear" x1="50.9527" y1="31.3841" x2="40.0245" y2="34.1162"
                            gradientUnits="userSpaceOnUse">
                            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
                            <stop offset="1" stop-color="#E68E43"></stop>
                        </linearGradient>
                        <radialGradient id="paint3_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
                            gradientTransform="translate(49.3832 48.0607) rotate(180) scale(28.9435)">
                            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
                            <stop offset="1" stop-color="#FF8900"></stop>
                        </radialGradient>
                        <radialGradient id="paint4_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
                            gradientTransform="translate(29.7592 46.5552) rotate(180) scale(30.0741)">
                            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
                            <stop offset="1" stop-color="#FF8900"></stop>
                        </radialGradient>
                        <radialGradient id="paint5_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
                            gradientTransform="translate(45.7416 46.361) rotate(180) scale(25.0939 103.181)">
                            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
                            <stop offset="1" stop-color="#FF8900"></stop>
                        </radialGradient>
                        <radialGradient id="paint6_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
                            gradientTransform="translate(39.3416 39.4088) rotate(180) scale(10.3566 5.25668)">
                            <stop stop-color="#FBE07A"></stop>
                            <stop offset="0.2654" stop-color="#FCDF73" stop-opacity="0.7346"></stop>
                            <stop offset="0.6548" stop-color="#FDDB5F" stop-opacity="0.3452"></stop>
                            <stop offset="1" stop-color="#FFD748" stop-opacity="0"></stop>
                        </radialGradient>
                        <linearGradient id="paint7_linear" x1="54.7889" y1="76.0956" x2="41.6346" y2="29.2459"
                            gradientUnits="userSpaceOnUse">
                            <stop offset="0.00132565" stop-color="#FFCB4B"></stop>
                            <stop offset="1" stop-color="#FFD748"></stop>
                        </linearGradient>
                        <linearGradient id="paint8_linear" x1="47.6973" y1="18.3635" x2="36.7691" y2="21.0956"
                            gradientUnits="userSpaceOnUse">
                            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
                            <stop offset="1" stop-color="#E68E43"></stop>
                        </linearGradient>
                        <radialGradient id="paint9_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
                            gradientTransform="translate(39.7674 21.9024) rotate(91.5882) scale(12.7006 1.48173)">
                            <stop stop-color="#FBE07A"></stop>
                            <stop offset="0.2654" stop-color="#FCDF73" stop-opacity="0.7346"></stop>
                            <stop offset="0.6548" stop-color="#FDDB5F" stop-opacity="0.3452"></stop>
                            <stop offset="1" stop-color="#FFD748" stop-opacity="0"></stop>
                        </radialGradient>
                        <radialGradient id="paint10_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
                            gradientTransform="translate(27.2065 31.241) scale(29.355)">
                            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
                            <stop offset="1" stop-color="#FF8900"></stop>
                        </radialGradient>
                        <radialGradient id="paint11_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse"
                            gradientTransform="translate(26.1122 30.6449) rotate(92.9961) scale(17.4604 3.67741)">
                            <stop stop-color="#FFBC47" stop-opacity="0"></stop>
                            <stop offset="1" stop-color="#FF8900"></stop>
                        </radialGradient>
                    </defs>
                </g>
            </svg>
        </div>
    </body>

</template>


<style scoped>

.insulto {
  animation: insultoAnimation 1s  2;
}


@keyframes insultoAnimation {
  0% {
    transform: scale(100%);
    opacity: 1;
  }

  10% {
    transform: scale(500%);
    opacity: 1;
  }

  20% {
    transform: scale(100%);
    opacity: 1;
  }

  30% {
    transform: scale(500%);
    opacity: 1;
  }

  40% {
    transform: scale(100%);
    opacity: 1;
  }

  50% {
    transform: scale(500%);
    opacity: 1;
  }

  60% {
    transform: scale(100%);
    opacity: 1;
  }

  70% {
    transform: scale(500%);
    opacity: 1;
  }

  80% {
    transform: scale(100%);
    opacity: 1;
  }

  90% {
    transform: scale(500%);
    opacity: 1;
  }

  100% {
    transform: scale(100%);
    opacity: 0;
  }
}
body {
    display: flex;
    align-items: flex-end;
    justify-content: center;
    min-height: 100vh;
    background-color: var(--dark-color);
    overflow: hidden;
    perspective: 1000px;
}

.night {
    position: fixed;
    left: 50%;
    z-index: 50;
    top: 0;
    transform: translateX(-50%);
    width: 100%;
    height: 100%;
    filter: blur(0.1vmin);
    background-image: radial-gradient(ellipse at top,
            transparent 0%,
            var(--dark-color)),
        radial-gradient(ellipse at bottom,
            var(--dark-color),
            rgba(145, 233, 255, 0.2)),
        repeating-linear-gradient(220deg,
            rgb(0, 0, 0) 0px,
            rgb(0, 0, 0) 19px,
            transparent 19px,
            transparent 22px),
        repeating-linear-gradient(189deg,
            rgb(0, 0, 0) 0px,
            rgb(0, 0, 0) 19px,
            transparent 19px,
            transparent 22px),
        repeating-linear-gradient(148deg,
            rgb(0, 0, 0) 0px,
            rgb(0, 0, 0) 19px,
            transparent 19px,
            transparent 22px),
        linear-gradient(90deg, rgb(255, 94, 0), rgb(240, 240, 240));
}

.container * {
    -webkit-animation-play-state: paused !important;
    animation-play-state: paused !important;
}

/*# sourceMappingURL=main.css.map */
.bubbles {
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    pointer-events: none;
}

.bubble {
    position: absolute;
    z-index: 200;
    border-radius: 50%;
}

.bubble:nth-child(1) {
    top: 8%;
    left: 60%;

    height: 11vmin;
    width: 11vmin;
    -webkit-animation: love-burst 3s infinite 0s;
    animation: love-burst 3s infinite 0s;
    box-shadow: inset 0 0 0 5.5vmin transparent;
    -webkit-transform: translate(0, 0.05em) scale(0);
    transform: translate(0, 0.05em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(2) {
    top: 83%;
    left: 14%;
    height: 20vmin;
    width: 20vmin;
    -webkit-animation: love-burst 3s infinite 0.15s;
    animation: love-burst 3s infinite 0.15s;
    box-shadow: inset 0 0 0 10vmin transparent;
    -webkit-transform: translate(0, 0.75em) scale(0);
    transform: translate(0, 0.75em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(3) {
    top: 25%;
    left: 49%;
    height: 4vmin;
    width: 4vmin;
    -webkit-animation: love-burst 3s infinite 0.3s;
    animation: love-burst 3s infinite 0.3s;
    box-shadow: inset 0 0 0 2vmin transparent;
    -webkit-transform: translate(0, 0.5em) scale(0);
    transform: translate(0, 0.5em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(4) {
    top: 63%;
    left: 93%;
    height: 3vmin;
    width: 3vmin;
    -webkit-animation: love-burst 3s infinite 0.45s;
    animation: love-burst 3s infinite 0.45s;
    box-shadow: inset 0 0 0 1.5vmin transparent;
    -webkit-transform: translate(0, 0.35em) scale(0);
    transform: translate(0, 0.35em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(5) {
    top: 7%;
    left: 56%;
    height: 18vmin;
    width: 18vmin;
    -webkit-animation: love-burst 3s infinite 0.6s;
    animation: love-burst 3s infinite 0.6s;
    box-shadow: inset 0 0 0 9vmin transparent;
    -webkit-transform: translate(0, 0.3em) scale(0);
    transform: translate(0, 0.3em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(6) {
    top: 10%;
    left: 68%;
    height: 5vmin;
    width: 5vmin;
    -webkit-animation: love-burst 3s infinite 0.75s;
    animation: love-burst 3s infinite 0.75s;
    box-shadow: inset 0 0 0 2.5vmin transparent;
    -webkit-transform: translate(0, 1.1em) scale(0);
    transform: translate(0, 1.1em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(7) {
    top: 68%;
    left: 1%;
    height: 5vmin;
    width: 5vmin;
    -webkit-animation: love-burst 3s infinite 0.9s;
    animation: love-burst 3s infinite 0.9s;
    box-shadow: inset 0 0 0 2.5vmin transparent;
    -webkit-transform: translate(0, 0.15em) scale(0);
    transform: translate(0, 0.15em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(8) {
    top: 61%;
    left: 51%;
    height: 11vmin;
    width: 11vmin;
    -webkit-animation: love-burst 3s infinite 1.05s;
    animation: love-burst 3s infinite 1.05s;
    box-shadow: inset 0 0 0 5.5vmin transparent;
    -webkit-transform: translate(0, 1.05em) scale(0);
    transform: translate(0, 1.05em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(9) {
    top: 24%;
    left: 45%;
    height: 11vmin;
    width: 11vmin;
    -webkit-animation: love-burst 3s infinite 1.2s;
    animation: love-burst 3s infinite 1.2s;
    box-shadow: inset 0 0 0 5.5vmin transparent;
    -webkit-transform: translate(0, 1em) scale(0);
    transform: translate(0, 1em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(10) {
    top: 13%;
    left: 10%;
    height: 19vmin;
    width: 19vmin;
    -webkit-animation: love-burst 3s infinite 1.35s;
    animation: love-burst 3s infinite 1.35s;
    box-shadow: inset 0 0 0 9.5vmin transparent;
    -webkit-transform: translate(0, 1em) scale(0);
    transform: translate(0, 1em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(11) {
    top: 76%;
    left: 7%;
    height: 14vmin;
    width: 14vmin;
    -webkit-animation: love-burst 3s infinite 1.5s;
    animation: love-burst 3s infinite 1.5s;
    box-shadow: inset 0 0 0 7vmin transparent;
    -webkit-transform: translate(0, 0.1em) scale(0);
    transform: translate(0, 0.1em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(12) {
    top: 22%;
    left: 8%;
    height: 17vmin;
    width: 17vmin;
    -webkit-animation: love-burst 3s infinite 1.65s;
    animation: love-burst 3s infinite 1.65s;
    box-shadow: inset 0 0 0 8.5vmin transparent;
    -webkit-transform: translate(0, 0.2em) scale(0);
    transform: translate(0, 0.2em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(13) {
    top: 23%;
    left: 81%;
    height: 16vmin;
    width: 16vmin;
    -webkit-animation: love-burst 3s infinite 1.8s;
    animation: love-burst 3s infinite 1.8s;
    box-shadow: inset 0 0 0 8vmin transparent;
    -webkit-transform: translate(0, 0.1em) scale(0);
    transform: translate(0, 0.1em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(14) {
    top: 77%;
    left: 88%;
    height: 3vmin;
    width: 3vmin;
    -webkit-animation: love-burst 3s infinite 1.95s;
    animation: love-burst 3s infinite 1.95s;
    box-shadow: inset 0 0 0 1.5vmin transparent;
    -webkit-transform: translate(0, 0.45em) scale(0);
    transform: translate(0, 0.45em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(15) {
    top: 41%;
    left: 1%;
    height: 9vmin;
    width: 9vmin;
    -webkit-animation: love-burst 3s infinite 2.1s;
    animation: love-burst 3s infinite 2.1s;
    box-shadow: inset 0 0 0 4.5vmin transparent;
    -webkit-transform: translate(0, 0.05em) scale(0);
    transform: translate(0, 0.05em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(16) {
    top: 51%;
    left: 51%;
    height: 8vmin;
    width: 8vmin;
    -webkit-animation: love-burst 3s infinite 2.25s;
    animation: love-burst 3s infinite 2.25s;
    box-shadow: inset 0 0 0 4vmin transparent;
    -webkit-transform: translate(0, 1.15em) scale(0);
    transform: translate(0, 1.15em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(17) {
    top: 37%;
    left: 65%;
    height: 11vmin;
    width: 11vmin;
    -webkit-animation: love-burst 3s infinite 2.4s;
    animation: love-burst 3s infinite 2.4s;
    box-shadow: inset 0 0 0 5.5vmin transparent;
    -webkit-transform: translate(0, 0.2em) scale(0);
    transform: translate(0, 0.2em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(18) {
    top: 11%;
    left: 83%;
    height: 18vmin;
    width: 18vmin;
    -webkit-animation: love-burst 3s infinite 2.55s;
    animation: love-burst 3s infinite 2.55s;
    box-shadow: inset 0 0 0 9vmin transparent;
    -webkit-transform: translate(0, 0.9em) scale(0);
    transform: translate(0, 0.9em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(19) {
    top: 64%;
    left: 86%;
    height: 12vmin;
    width: 12vmin;
    -webkit-animation: love-burst 3s infinite 2.7s;
    animation: love-burst 3s infinite 2.7s;
    box-shadow: inset 0 0 0 6vmin transparent;
    -webkit-transform: translate(0, 0.65em) scale(0);
    transform: translate(0, 0.65em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

.bubble:nth-child(20) {
    top: 39%;
    left: 24%;
    height: 19vmin;
    width: 19vmin;
    -webkit-animation: love-burst 3s infinite 2.85s;
    animation: love-burst 3s infinite 2.85s;
    box-shadow: inset 0 0 0 9.5vmin transparent;
    -webkit-transform: translate(0, 0.2em) scale(0);
    transform: translate(0, 0.2em) scale(0);
    -webkit-transform-origin: center bottom;
    transform-origin: center bottom;
}

@-webkit-keyframes love-burst {

    50%,
    100% {
        box-shadow: inset 0 0 0 0 rgb(1, 175, 73);
        -webkit-transform: translate(0, 0) scale(1);
        transform: translate(0, 0) scale(1);
    }
}

@keyframes love-burst {

    50%,
    100% {
        box-shadow: inset 0 0 0 0 rgb(18, 226, 129);
        -webkit-transform: translate(0, 0) scale(1);
        transform: translate(0, 0) scale(1);
    }
}

.heart {
    fill: transparent;
    opacity: 0;
}

.bubble:nth-child(1) .heart {
    -webkit-animation: love 3s forwards infinite 0s;
    animation: love 3s forwards infinite 0s;
    -webkit-transform: scale(0.5) rotate(-4deg);
    transform: scale(0.5) rotate(-4deg);
}

.bubble:nth-child(2) .heart {
    -webkit-animation: love 3s forwards infinite 0.15s;
    animation: love 3s forwards infinite 0.15s;
    -webkit-transform: scale(0.5) rotate(22deg);
    transform: scale(0.5) rotate(22deg);
}

.bubble:nth-child(3) .heart {
    -webkit-animation: love 3s forwards infinite 0.3s;
    animation: love 3s forwards infinite 0.3s;
    -webkit-transform: scale(0.5) rotate(-5deg);
    transform: scale(0.5) rotate(-5deg);
}

.bubble:nth-child(4) .heart {
    -webkit-animation: love 3s forwards infinite 0.45s;
    animation: love 3s forwards infinite 0.45s;
    -webkit-transform: scale(0.5) rotate(50deg);
    transform: scale(0.5) rotate(50deg);
}

.bubble:nth-child(5) .heart {
    -webkit-animation: love 3s forwards infinite 0.6s;
    animation: love 3s forwards infinite 0.6s;
    -webkit-transform: scale(0.5) rotate(-29deg);
    transform: scale(0.5) rotate(-29deg);
}

.bubble:nth-child(6) .heart {
    -webkit-animation: love 3s forwards infinite 0.75s;
    animation: love 3s forwards infinite 0.75s;
    -webkit-transform: scale(0.5) rotate(35deg);
    transform: scale(0.5) rotate(35deg);
}

.bubble:nth-child(7) .heart {
    -webkit-animation: love 3s forwards infinite 0.9s;
    animation: love 3s forwards infinite 0.9s;
    -webkit-transform: scale(0.5) rotate(-5deg);
    transform: scale(0.5) rotate(-5deg);
}

.bubble:nth-child(8) .heart {
    -webkit-animation: love 3s forwards infinite 1.05s;
    animation: love 3s forwards infinite 1.05s;
    -webkit-transform: scale(0.5) rotate(40deg);
    transform: scale(0.5) rotate(40deg);
}

.bubble:nth-child(9) .heart {
    -webkit-animation: love 3s forwards infinite 1.2s;
    animation: love 3s forwards infinite 1.2s;
    -webkit-transform: scale(0.5) rotate(-35deg);
    transform: scale(0.5) rotate(-35deg);
}

.bubble:nth-child(10) .heart {
    -webkit-animation: love 3s forwards infinite 1.35s;
    animation: love 3s forwards infinite 1.35s;
    -webkit-transform: scale(0.5) rotate(28deg);
    transform: scale(0.5) rotate(28deg);
}

.bubble:nth-child(11) .heart {
    -webkit-animation: love 3s forwards infinite 1.5s;
    animation: love 3s forwards infinite 1.5s;
    -webkit-transform: scale(0.5) rotate(-3deg);
    transform: scale(0.5) rotate(-3deg);
}

.bubble:nth-child(12) .heart {
    -webkit-animation: love 3s forwards infinite 1.65s;
    animation: love 3s forwards infinite 1.65s;
    -webkit-transform: scale(0.5) rotate(48deg);
    transform: scale(0.5) rotate(48deg);
}

.bubble:nth-child(13) .heart {
    -webkit-animation: love 3s forwards infinite 1.8s;
    animation: love 3s forwards infinite 1.8s;
    -webkit-transform: scale(0.5) rotate(-33deg);
    transform: scale(0.5) rotate(-33deg);
}

.bubble:nth-child(14) .heart {
    -webkit-animation: love 3s forwards infinite 1.95s;
    animation: love 3s forwards infinite 1.95s;
    -webkit-transform: scale(0.5) rotate(40deg);
    transform: scale(0.5) rotate(40deg);
}

.bubble:nth-child(15) .heart {
    -webkit-animation: love 3s forwards infinite 2.1s;
    animation: love 3s forwards infinite 2.1s;
    -webkit-transform: scale(0.5) rotate(-29deg);
    transform: scale(0.5) rotate(-29deg);
}

.bubble:nth-child(16) .heart {
    -webkit-animation: love 3s forwards infinite 2.25s;
    animation: love 3s forwards infinite 2.25s;
    -webkit-transform: scale(0.5) rotate(19deg);
    transform: scale(0.5) rotate(19deg);
}

.bubble:nth-child(17) .heart {
    -webkit-animation: love 3s forwards infinite 2.4s;
    animation: love 3s forwards infinite 2.4s;
    -webkit-transform: scale(0.5) rotate(-29deg);
    transform: scale(0.5) rotate(-29deg);
}

.bubble:nth-child(18) .heart {
    -webkit-animation: love 3s forwards infinite 2.55s;
    animation: love 3s forwards infinite 2.55s;
    -webkit-transform: scale(0.5) rotate(14deg);
    transform: scale(0.5) rotate(14deg);
}

.bubble:nth-child(19) .heart {
    -webkit-animation: love 3s forwards infinite 2.7s;
    animation: love 3s forwards infinite 2.7s;
    -webkit-transform: scale(0.5) rotate(-10deg);
    transform: scale(0.5) rotate(-10deg);
}

.bubble:nth-child(20) .heart {
    -webkit-animation: love 3s forwards infinite 2.85s;
    animation: love 3s forwards infinite 2.85s;
    -webkit-transform: scale(0.5) rotate(46deg);
    transform: scale(0.5) rotate(46deg);
}

@-webkit-keyframes love {
    50% {
        fill: rgb(253, 66, 19);
        opacity: 1;
    }
}

@keyframes love {
    50% {
        fill: rgb(253, 93, 19);
        opacity: 1;
    }
}
</style>