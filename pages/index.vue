<script setup>
definePageMeta({
  layout: "landing",
  title: 'Nicolai Dybro | Portfolio',
});
useHead({
        title: 'Nicolai Dybro | Portfolio',
    });
</script>

<script setup lang="ts">
useHead({
  title: 'Nicolai Dybro | Portfolio',
  meta: [
    { name: 'description', content: 'Nicolai Dybro Portfolio.' }
  ],
})
</script>

<template>
    <ContainersContainer>
    <div>
        <Profile/>
    </div>
    </ContainersContainer>
    <ContainersBagcontainer>
        <div>
            <Projects/>
        </div>
      </ContainersBagcontainer>
      <ContainersContainer>
    <div>
        <Expertise/>
    </div>
    </ContainersContainer>
    <!---->

      <Footer/>
</template>


<style>
html {
    scroll-behavior: smooth;
}
</style>