<template>
    <v-card class="mx-auto" width="256">
      <v-layout>
        <v-navigation-drawer absolute permanent>
          <v-list>
            <v-list-item
              prepend-avatar="https://cdn.vuetifyjs.com/images/john.png"
              subtitle="john@google.com"
              title="John Leider"
            >
              <template v-slot:append>
                <v-btn icon="mdi-menu-down" size="small" variant="text"></v-btn>
              </template>
            </v-list-item>
          </v-list>
  
          <v-divider></v-divider>
  
          <v-list density="compact" nav>
            <v-list-item
              v-for="(item, i) in items"
              :key="i"
              color="primary"
            >
              <template v-slot:prepend>
                <v-icon :icon="item.icon"></v-icon>
              </template>
              <v-list-item-title>{{ item.text }}</v-list-item-title>
            </v-list-item>
          </v-list>
        </v-navigation-drawer>
  
        <v-main style="height: 354px;"></v-main>
      </v-layout>
    </v-card>
  </template>
  
  <script>
  export default {
    data() {
      return {
        items: [
          { text: 'Fabian', icon: 'mdi-folder' },
          { text: 'Espinoza', icon: 'mdi-account-multiple' },
          { text: '15451511', icon: 'mdi-star' },
          { text: 'fabzzzzzz', icon: 'mdi-history' },
        ],
      };
    },
  };
  </script>
  