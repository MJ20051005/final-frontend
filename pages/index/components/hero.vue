<template>
  <div class="hero-image">
    <div class="hero-text">
      <h1 style="font-size:100px">Green Ride</h1>
      <p>Cuida el planeta</p>
    </div>
  </div>
</template>

<script setup>
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Courier+New:wght@400&display=swap');

  body, html {
    height: 100%;
    margin: 0;
    font-family: 'Courier New', Courier, monospace;
  }

  .hero-image {
    background-image: linear-gradient(rgba(58, 238, 88, 0.5), rgba(112, 240, 144, 0.5)), url("photographer.jpg");
    height: 100vh;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
  }

  .hero-text {
    text-align: center;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: rgb(15, 165, 65);
  }
</style>

