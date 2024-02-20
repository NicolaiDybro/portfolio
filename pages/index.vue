<script setup>
definePageMeta({
  layout: "landing",
});
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