<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>
    <svg class="main_svg">
      <text x="50%" y="50%" dy=".35em" text-anchor="middle">Anmeldung</text>
    </svg>
  </header>

  <RouterView />
</template>

<style scoped>svg text {
    animation: stroke 6s alternate;
    stroke-width: 2;
  fill: rgba(72,138,204,1); 
  stroke: rgba(54,95,160,0);
    stroke-dashoffset: -25%; 
  stroke-dasharray: 50% 0; 
  stroke-width: 0;
    font-size: 100px;
}
@keyframes stroke {
    0%   {
        fill: rgba(72,138,204,0); stroke: rgba(54,95,160,1);
        stroke-dashoffset: 25%; stroke-dasharray: 0 50%; stroke-width: 2;
    }
    70%  {fill: rgba(72,138,204,0); stroke: rgba(54,95,160,1); }
    80%  {fill: rgba(72,138,204,0); stroke: rgba(54,95,160,1); stroke-width: 3; }
    100% {
        fill: rgba(72,138,204,1); stroke: rgba(54,95,160,0);
        stroke-dashoffset: -25%; stroke-dasharray: 50% 0; stroke-width: 0;
    }
}
</style>
