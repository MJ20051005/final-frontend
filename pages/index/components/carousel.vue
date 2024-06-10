<template>
    <v-carousel class="custom-carousel">
        <v-carousel-item
            class="carousel-item"
            src="../../../public/carrusel1.jpg"
            cover
        ></v-carousel-item>

        <v-carousel-item
            class="carousel-item"
            src="../../../public/carrusel2.jpg"
            cover
        ></v-carousel-item>

        <v-carousel-item
            class="carousel-item"
            src="../../../public/carrusel3.jpg"
            cover
        ></v-carousel-item>
    </v-carousel>
</template>

<script setup>
const items = ref([
    {
        public: "carrusel1.jpg"
    },
    {
        public: "carrusel2.jpg"
    },
    {
        public:"carrusel3.jpg"
    }
])
</script>

<style scoped>
.custom-carousel {
    max-width: 800px; /* Ajusta el ancho máximo del carrusel */
    margin: auto; /* Centra el carrusel horizontalmente */
}

.carousel-item img {
    max-width: 100%; /* Ajusta el ancho máximo de las imágenes dentro del carrusel */
    height: auto; /* Ajusta la altura automáticamente para mantener la proporción */
    object-fit: cover; /* Escala las imágenes para que cubran completamente el contenedor */
}
</style>
