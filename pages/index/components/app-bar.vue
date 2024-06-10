<template>

<v-app-bar app color="rgb(15, 165, 65)">
    <v-col cols="2000" md="0">
           <img src="/biciverde.jpeg" alt="image" width="100px" height="100px">
        </v-col>
    <v-toolbar-title> Green Ride</v-toolbar-title>
    <v-btn text @click="goTo ('/')">Home</v-btn>
    <v-btn text @click="goTo('/products')">Productos</v-btn>
    <v-btn text @click="goTo('/contact')">Contact</v-btn>
    <v-btn text @click="goTo('/pases')">Pases turisticos</v-btn>
    


</v-app-bar>

</template>

<script>
export default {
    methods: {
        goTo(route) {
            this.$router.push(route);
        }
    }
}
</script>