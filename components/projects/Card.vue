<template v-if="href !== '#'">
    <a .href="href">
        <div class="max-w-sm bg-zinc-900 px-4 pt-4 pb-2 rounded-xl shadow-lg transform hover:scale-105 transition duration-500">
          <div class="relative">
            <img class="w-full rounded-xl" .src="coverImage" alt="Colors" />
            <div class="overlay rounded-xl flex items-center justify-center">
                <svg width="64px" height="64px" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M14 7H16C18.7614 7 21 9.23858 21 12C21 14.7614 18.7614 17 16 17H14M10 7H8C5.23858 7 3 9.23858 3 12C3 14.7614 5.23858 17 8 17H10M8 12H16" stroke="#ffffff" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path> </g></svg>



            </div>
            <p :class="color" class="absolute top-0 text-white-800 font-semibold py-1 px-3 rounded-br-lg rounded-tl-lg">{{language}}</p>
          </div>
          <h1 class="mt-4 text-white-800 text-2xl font-bold cursor-pointer">{{title}}</h1>
          <div class="my-4">
            <div class="flex space-x-1 items-center">
              <span>
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-sky-600 mb-1.5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 4v12l-4-2-4 2V4M6 20h12a2 2 0 002-2V6a2 2 0 00-2-2H6a2 2 0 00-2 2v12a2 2 0 002 2z" />
                </svg>
              </span>
              <p>{{info}}</p>
            </div>
          </div>
        </div>
    </a>
  </template>
  
  <style scoped>
    .overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.5); /* Just adjust the alpha value for transparency */
      z-index: 1;
      opacity: 0;
      transition: opacity 0.3s ease;
    }
  
    .max-w-sm:hover .overlay {
      opacity: 1;
    }
  </style>
  
  <script lang="ts" setup>
  const { title, info, href, coverImage, language, color } = defineProps<{
    title: string,
    info: string,
    href: string,
    coverImage: string
    language: string
    color: string
  }>()
  </script>