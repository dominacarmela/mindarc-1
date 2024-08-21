<script setup lang="ts">

</script>

<template>
  <div class="desktop-banner">
    <div class="desktop-banner__container">
      <h1>Hello Developer!</h1>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
    </div>
  </div>
</template>

<style scoped>
.desktop-banner {
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  background-image: url(../assets/mobile-banner.png);
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 400px;
  width: 100%;

}
.desktop-banner__container {
  text-align: center;
  padding: 0 20px;
}
.desktop-banner__container p {
  font-size: 24px;
}

@media (min-width: 1024px) {
  .desktop-banner {
    min-height: 650px;
    background-image: url(../assets/desktop-banner.png);
  }
  
}
</style>
