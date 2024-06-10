<template>
  <v-app>
    <v-main>
      <v-container>
        <!-- Sección de ¿Quiénes somos? -->
        <v-row justify="center">
          <v-col cols="12" md="8" lg="5">
            <h1 class="title">¿Quiénes somos?</h1>
            <v-row>
              <v-col cols="12" md="8" sm="12" xs="12">
                <p class="description">
                  Somos un emprendimiento innovador sobre el alquiler de bicicletas, podrás alquilarlas para pasear por la ciudad y además, ayudar al medio ambiente.
                </p>
              </v-col>
              <v-col cols="12" md="4" sm="12" xs="12">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQQlmyx4zFjKG-NOBY3_cjePX7RxSGg5U28kg&s" alt="Descripción de la imagen" class="side-image">
              </v-col>
            </v-row>
          </v-col>
        </v-row>

        <!-- Sección de Descubre una nueva forma de moverte -->
        <v-row justify="center" class="mt-5">
          <v-col cols="12" md="8" lg="5">
            <v-card class="mx-auto" max-width="600" outlined>
              <v-img src="../../../public/biciverde.jpeg" height="300px"></v-img>
              <v-card-title class="text-h4">
                Descubre una nueva forma de moverte!
              </v-card-title>
              <v-card-text class="text-h6">
                <p>Descarga la app y creá tu cuenta.</p>
              </v-card-text>
              <v-card-actions>
                <v-btn color="primary" outlined href="https://play.google.com/store">
                  <v-icon left>mdi-google-play</v-icon> Google Play
                </v-btn>
                <v-btn color="primary" outlined href="https://www.apple.com/app-store">
                  <v-icon left>mdi-apple</v-icon> App Store
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
          <v-col cols="12" md="8" lg="4" class="d-flex align-center justify-center">
            <div class="instructions text-center">
              <h2 class="text-h5">Instrucciones:</h2>
              <ol class="text-h6">
                <li>Crea tu cuenta</li>
                <li>Elige tu pase</li>
                <li>Desbloquea una bici</li>
                <li>Devuelve la bici</li>
              </ol>
            </div>
          </v-col>
        </v-row>

        <!-- Sección de Nuestras bicis -->
        <v-row justify="center" class="mt-5">
          <h1 class="title">Nuestras bicis</h1>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style scoped>
.v-application {
  background-color: #ffffff;
}

.v-btn {
  margin: 8px;
}

.v-card-title {
  font-size: 1.75rem;
  font-weight: bold;
}

.v-card-text {
  font-size: 1.25rem;
}

.instructions {
  background-color: #dcedc8; /* Verde claro */
  padding: 16px;
  border-radius: 8px;
}

.instructions h2 {
  font-size: 1.75rem;
  font-weight: bold;
  margin-bottom: 16px;
  font-family: 'Roboto', sans-serif; /* Cambia la fuente a Roboto */
}

.instructions ol {
  font-size: 1.25rem;
  padding-left: 20px;
  font-family: 'Roboto', sans-serif; /* Cambia la fuente a Roboto */
}

.title {
  font-size: 3rem;
  text-align: center;
  margin-bottom: 20px;
}

.side-image {
  width: 100%;
  height: auto;
  max-width: 100%;
  border-radius: 8px;
  margin-bottom: 20px;
}

.description {
  font-size: 1.5rem;
  text-align: justify;
  margin: 20px 0;
}

.call-to-action {
  font-size: 2rem;
  text-align: center;
  margin: 20px 0;
}
</style>