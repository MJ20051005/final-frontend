<template>
    <div class="timeline">
      <h2>Timeline</h2>
      <div v-if="eventos.length > 0">
        <ul>
          <li v-for="(evento, index) in eventos" :key="index">
            <div class="evento">
              <div class="fecha">{{ evento.fecha }}</div>
              <div class="contenido">
                <h3>{{ evento.titulo }}</h3>
                <p>{{ evento.descripcion }}</p>
              </div>
            </div>
          </li>
        </ul>
      </div>
      <div v-else>
        <p>No hay eventos en la línea de tiempo.</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        eventos: [
          { fecha: '1 de enero de 2024', titulo: 'Evento 1', descripcion: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.' },
          { fecha: '15 de marzo de 2024', titulo: 'Evento 2', descripcion: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.' },
          { fecha: '30 de abril de 2024', titulo: 'Evento 3', descripcion: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.' }
        ]
      };
    }
  };
  </script>
  
  <style scoped>
  .timeline {
    margin: 20px;
  }
  
  .evento {
    display: flex;
    margin-bottom: 20px;
  }
  
  .fecha {
    font-weight: bold;
    margin-right: 10px;
  }
  
  .contenido {
    flex: 1;
  }
  </style>
  


































































































































































































