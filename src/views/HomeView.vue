<template>
  <main v-if="isMainActive">
    <div class="flex justify-center items-center h-screen bg-black">
      <div class="wrapper">
        <div class="lid one"></div>
        <div class="lid two"></div>
        <div class="envelope"></div>
        <div @click="openModal(), playAudio(1)" 
          class="letter flex items-center justify-center absolute top-0 w-4/5 h-4/5 bg-white rounded-lg z-2 transition-all duration-500 cursor-pointer">
          <p>Para Chloe</p>
        </div>
      </div>
    </div>
    <div class="fixed inset-0 flex items-center justify-center z-50 bg-black bg-opacity-50" :class="{
      'opacity-0 pointer-events-none': !isModalOpen,
      'opacity-100': isModalOpen
    }">
      <div
        class="bg-black w-7xl h-11/12 p-6 rounded-lg shadow-lg opacity-0 scale-50 transition-all duration-300 flex flex-col bg-[url('https://res.cloudinary.com/djfokdod6/image/upload/q_auto,f_auto/v1738645821/1605f65a-c4ef-4f72-b51f-894bcf294ea0.png')]"
        :class="{
          'opacity-100 scale-100': isModalOpen,
          'opacity-0 scale-50': !isModalOpen
        }" @click.stop>
        <div
          class="flex-1 flex justify-center items-center ">
          <div
            class="relative w-full max-w-sm md:max-w-md lg:max-w-lg aspect-square bg-[url('https://res.cloudinary.com/djfokdod6/image/upload/q_auto,f_auto/v1738644155/SanValentinpng_npgzuz.png')] bg-cover bg-center">

            <!-- Imagen izquierda -->
            <img
              src="https://res.cloudinary.com/djfokdod6/image/upload/q_auto,f_auto/v1738641878/1f850362-b9c8-44d6-8d98-3ae7ce62d6ba-removebg-preview_g9fsyg.png"
              alt="" class="absolute md:bottom-0 md:-rotate-90  -rotate-30 bottom-80
             h-36 sm:h-36 md:h-44 lg:h-56 xl:h-72 
             -left-12 sm:-left-16 md:-left-36 lg:-left-48 xl:-left-56">

            <!-- Imagen derecha -->
            <img src="https://res.cloudinary.com/djfokdod6/image/upload/q_auto,f_auto/v1738641642/image_ymqnxp.png"
              alt="" class="absolute bottom-0 
             h-36 sm:h-36 md:h-44 lg:h-56 xl:h-72 
             -right-10 sm:-right-16 md:-right-16 lg:-right-24">
          </div>
        </div>


        <div class="flex justify-center space-x-3 p-4">
          <button @click="toggleMain(), pauseAudio(1), playAudio(2)"
            class="bg-red-500 text-white font-semibold py-2 px-6 rounded-full hover:bg-red-600 transition duration-300 ease-in-out transform   focus:outline-none focus:ring-2 focus:ring-red-500 focus:ring-opacity-50">
            Si
          </button>
          <RocketButton />
        </div>

      </div>
    </div>
  </main>
  <main v-else>
    <FlowersView @pause-audio="pauseAudio"/>
  </main>

  <div>
    <div class="hidden">
      <audio ref="audioPlayer1" :src="audioSrc1" controls></audio>
      <button @click="playAudio(1)">Reproducir Audio 1</button>
      <button @click="pauseAudio(1)">Pausar Audio 1</button>
      <button @click="stopAudio(1)">Detener Audio 1</button>
    </div>

    <div class="hidden">
      <audio ref="audioPlayer2" :src="audioSrc2" controls></audio>
      <button @click="playAudio(2)">Reproducir Audio 2</button>
      <button @click="pauseAudio(2)">Pausar Audio 2</button>
      <button @click="stopAudio(2)">Detener Audio 2</button>
    </div>
  </div>
</template>

<script setup>
import RocketButton from '@/components/RocketButton.vue';
import { ref } from 'vue';
import FlowersView from './FlowersView.vue';

const isModalOpen = ref(false);

const isMainActive = ref(true);
const toggleMain = () =>{
  isMainActive.value = !isMainActive.value
}

const openModal = () => {
  isModalOpen.value = true;
  
};

const closeModal = () => {
  isModalOpen.value = false;
};



const audioSrc1 = ref('/ChillGuy.mp3');
const audioSrc2 = ref('/OjitosLindos.mp3');

// Referencias a los elementos de audio
const audioPlayer1 = ref(null);
const audioPlayer2 = ref(null);

// Función para reproducir audio
const playAudio = (audioNumber) => {
  if (audioNumber === 1) {
    audioPlayer1.value.play();
  } else {
    audioPlayer2.value.play();
  }
};

// Función para pausar audio
const pauseAudio = (audioNumber) => {
  if (audioNumber === 1) {
    audioPlayer1.value.pause();
  } else {
    audioPlayer2.value.pause();
  }
};

// Función para detener audio
const stopAudio = (audioNumber) => {
  if (audioNumber === 1) {
    audioPlayer1.value.pause();
    audioPlayer1.value.currentTime = 0;
  } else {
    audioPlayer2.value.pause();
    audioPlayer2.value.currentTime = 0;
  }
};
</script>

<style scoped></style>