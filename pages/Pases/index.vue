<template>

    <div class="d-flex flex-wrap">
        <card v-for="item in items" :item="item"></card>
   
    </div>
        
      </template>
      <script setup>
      import card from "./components/card.vue"
      import appBar from "../index/components/app-bar.vue"
     

      
      const items = ref([
        {
          titulo: "Budget-friendly bike ",
          subtitlo: "Categoria a",
          text: "Por un viaje (45 min): Bs.5 -Por un dia: Bs.30 -Por 3 dias: Bs.80  -Por 7 dias: Bs.150",
          url: "https://media.istockphoto.com/id/1439808962/es/foto/bicicleta-el%C3%A9ctrica-negra-aislada-sobre-fondo-blanco.jpg?s=612x612&w=0&k=20&c=Xjh2Lozm0qD8EuHuZVLxFWuhKU-BFFMGgANDD-vIF1I="
        },
        {
          titulo: "Mid-range bike",
          subtitlo: "Categoria b",
          text: "Por un viaje (45 min): Bs.5 -Por un dia: Bs.30  -Por 3 dias: Bs.90  -Por 7 dias: Bs.150",
          url: "https://media.istockphoto.com/id/1415317051/es/foto/bicicleta-el%C3%A9ctrica-negra-aislada-sobre-fondo-blanco.jpg?s=612x612&w=0&k=20&c=jVoxQEiR2r_47f8tGWskxZ8cdZvv7c04kiRixkAXEls="
        },
        {
          titulo: "Premium bike",
          subtitlo: "Categoria c",
          text: "Por un viaje (45 min): Bs.15 -Por un dia: Bs.90 -Por 3 dias: Bs.200 -Por 7 dias: Bs.300",
          url: "https://media.istockphoto.com/id/1135938388/es/foto/bicicleta-el%C3%A9ctrica-gen%C3%A9rica-e-bike-aislado-sobre-fondo-blanco-ilustraci%C3%B3n-3d.jpg?s=612x612&w=0&k=20&c=ysxa6k52X9VoWzXUurL0e0A0n9vahOQsngtBe4GyO-E="
        }
      ])
      
      </script>
      