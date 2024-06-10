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
          text: "Por minuto: Bs. 0,20 -Pase diario: Bs. 10 al dia -Pase mensual: Bs. 50 al mes",
          url: "https://media.istockphoto.com/id/1439808962/es/foto/bicicleta-el%C3%A9ctrica-negra-aislada-sobre-fondo-blanco.jpg?s=612x612&w=0&k=20&c=Xjh2Lozm0qD8EuHuZVLxFWuhKU-BFFMGgANDD-vIF1I="
        },
        {
          titulo: "Mid-range bike",
          subtitlo: "Categoria b",
          text: "Por minuto: Bs. 0,50 -Pase diario: Bs. 15 al dia -Pase mensual: Bs. 100 al mes",
          url: "https://media.istockphoto.com/id/1415317051/es/foto/bicicleta-el%C3%A9ctrica-negra-aislada-sobre-fondo-blanco.jpg?s=612x612&w=0&k=20&c=jVoxQEiR2r_47f8tGWskxZ8cdZvv7c04kiRixkAXEls="
        },
        {
          titulo: "Premium bike",
          subtitlo: "Categoria c",
          text: "Por minuto: Bs. 1,00 -Pase diario: Bs. 20 al dia -Pase mensual: Bs. 150 al mes",
          url: "https://media.istockphoto.com/id/1135938388/es/foto/bicicleta-el%C3%A9ctrica-gen%C3%A9rica-e-bike-aislado-sobre-fondo-blanco-ilustraci%C3%B3n-3d.jpg?s=612x612&w=0&k=20&c=ysxa6k52X9VoWzXUurL0e0A0n9vahOQsngtBe4GyO-E="
        }
      ])
      
      </script>
      