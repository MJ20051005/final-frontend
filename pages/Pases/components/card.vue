<template>

  <v-card
    class="mx-auto"
    max-width="344"
  >
    <v-img
      height="200px"
      :src="item.url"
      cover
    ></v-img>

    <v-card-title>
      {{ item.titulo }}
    </v-card-title>

    <v-card-subtitle>
      {{ item.subtitulo }}
    </v-card-subtitle>

    <v-card-actions>
      <v-btn
        color="green-lighten-2"
        text="Explorar"
      ></v-btn>

      <v-spacer></v-spacer>

      <v-btn
        :icon="show ? 'mdi-chevron-up' : 'mdi-chevron-down'"
        @click="show = !show"
      ></v-btn>
    </v-card-actions>

    <v-expand-transition>
      <div v-show="show">
        <v-divider></v-divider>

        <v-card-text>
          {{ item.text }}  
        </v-card-text>
      </div>
    </v-expand-transition>
  </v-card>
</template>

<script>
  export default {
    props: {
      item:{
        type: Object,
        required: true
      }
    },
  
    data: () => ({
      show: false,
    }),
  }
</script>
