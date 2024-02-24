<template>
  <main class="grid lg:grid-cols-2 place-items-center pt-56 pb-56 md:pt-56" >
    <div class="p-4 md:order-1 hidden md:block rounded-full rotate-border">
      <div class="image-container">
        <img
          class="rounded-full"
          src="../../assets/nicolai.png"
          loading="eager"
          format="avif"
          width="450"
          height="450"
        />
      </div>
    </div>

    <div>
      <h1 class="text-5xl lg:text-6xl xl:text-7xl font-bold lg:tracking-tight">
        Hi! My name is
        <span
        class="bg-gradient-to-r from-teal-400 via-blue-300 to-violet-400 text-transparent bg-clip-text animate-gradient"
        >
          Nicolai
        </span>
      </h1>
      <p class="text-lg mt-4 max-w-xl">
        I am a product-oriented         <span
        class="bg-gradient-to-r font-bold from-violet-400 via-blue-300 to-teal-400 text-transparent bg-clip-text animate-gradient"
        >
          Software Developer
        </span> with a business mindset from
        bringing the latest tech to launching successful startups!
      </p>
    </div>
  </main>
</template>

<style>
.animate-gradient {
  background-size: 300%;
  -webkit-animation: animatedgradient 5s ease infinite alternate;
  -moz-animation: animatedgradient 5s ease infinite alternate;
  animation: animatedgradient 5s ease infinite alternate;
}

.rotate-border {
  position: relative;
  overflow: hidden;
}

.rotate-border::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  border: 8px dashed #659bff; /* Adjust border properties as needed */
  border-radius: 50%;
  animation: spin 40s infinite reverse linear;
}

@keyframes spin {
  100% {
    transform: rotate(1turn);
  }
}

.image-container {
  overflow: hidden;
  border-radius: 50%;
}

.grid {
  animation: fadeInAnimation ease 2s;
  animation-iteration-count: 1;
  animation-fill-mode: forwards;
}

@keyframes fadeInAnimation {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
</style>