<script setup lang="ts">

const movie = {
       title:"Big Buck Bunny",
       description:"Three rodents amuse themselves by harassing creatures of the forest. However, when they mess with a bunny, he decides to teach them a lesson.",
       videoUrl:"http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4",
       thumbnailUrl:"https://upload.wikimedia.org/wikipedia/commons/7/70/Big.Buck.Bunny.-.Opening.Screen.png",
       genre:"Comedy",
       duration:"10 minutes"
    };
</script>

<template>
    <div class="relative h-[56.25vw]">
      <video :src=movie.videoUrl poster='https://www.youtube.com/watch?v=ft0KVQ-Tas4' class="w-full h-[56.25vw] object-cover brightness-[60%] transition duration-500" autoPlay muted loop></video>
      <div class="absolute top-[30%] md:top-[40%] ml-4 md:ml-16">
        <p class="text-white text-1xl md:text-5xl h-full w-[50%] lg:text-6xl font-bold drop-shadow-xl">
          Arterning
        </p>
        <p class="text-white text-[8px] md:text-lg mt-3 md:mt-8 w-[90%] md:w-[80%] lg:w-[50%] drop-shadow-xl">
          cute
        </p>
        <div class="flex flex-row items-center mt-3 md:mt-4 gap-3">
          <button
            onClick={handleOpenModal}
            class="
            bg-white
            text-white
              bg-opacity-30 
              rounded-md 
              py-1 md:py-2 
              px-2 md:px-4
              w-auto 
              text-xs lg:text-lg 
              font-semibold
              flex
              flex-row
              items-center
              hover:bg-opacity-20
              transition
            "
            >
              More Info
          </button>
        </div>
      </div>
    </div>
</template>