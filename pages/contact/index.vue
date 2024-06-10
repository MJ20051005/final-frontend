<template>
    <v-card class="mx-auto" width="256">
      <v-layout>
        <v-navigation-drawer absolute permanent>
          <v-list>
            <v-list-item
              v-for="(contact, index) in contacts"
              :key="index"
              :prepend="contact"
              :subtitle="contact.email"
              :title="contact.name"
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
  
        <v-main style="height: 454px;"></v-main>
      </v-layout>
    </v-card>
  </template>
  
  <script>
  export default {
    data() {
      return {
        contacts: [
          { name: 'Maria Jose Castro', email: 'majo@google.com'},
          { name: 'Fabian Espinoza', email: 'fabian@google.com'},
          { name: 'Camila Gallo', email: 'camigallo@google.com'},
        ],
        items: [
          { text: 'Home', icon: 'mdi-home' },
          { text: 'Profile', icon: 'mdi-account' },
          { text: 'Messages', icon: 'mdi-message' },
          { text: 'Settings', icon: 'mdi-settings' }
        ]
      };
    }
  };
  </script>