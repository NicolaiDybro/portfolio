<template>
  <div id="projects" class="flex items-center justify-center mt-12">
    <h1 class="xl:text-4xl font-bold lg:tracking-tight">Showcase of my Projects</h1>
  </div>

  <div class="flex items-center justify-center mt-1">
    <h1 class="xl:text-1xl lg:tracking-tight">What I have worked on before</h1>
  </div>
  <div class="flex flex-wrap items-center justify-center gap-10 mt-12 mb-24">
    <div class="">
      <ProjectsCard
        title="Splocus"
        info="Server Software"
        href="https://splocus.dk"
        cover-image="../../images/splocuswebp.png"
        language="JAVA"
        color="bg-yellow-400"
      />
    </div>
    <div class="flex justify-center">
      <ProjectsCard
        title="JP Grønt"
        info="JavaFX Application for handling Data"
        href="https://www.jpgroent.dk/"
        cover-image="../../images/jpgrontwebp.png"
        language="JAVA"
        color="bg-yellow-400"
      />
    </div>
    <div class="flex justify-center">
      <ProjectsCard
        title="Bar Software"
        info="A Bar APP using bluetooth to mix drinks"
        href="https://github.com/NicolaiDybro/BarAPP"
        cover-image="../../images/barbotwebp.png"
        language="ANDROID APP"
        color="bg-green-400"
      />
    </div>


  </div>
</template>