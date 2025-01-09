<template>
    <v-app-bar :elevation="2">
    <v-app-bar-title>Application Bar</v-app-bar-title>
          <v-toolbar-items>
              <v-btn v-for="(item, i) in menuTabs" :key=item.id :to="item.route" text>{{item.name}} <v-icon class="pl-1">{{item.icon}}</v-icon></v-btn>
              <!-- <v-btn v-if="isUserAuthenticated" to="/profile" text>{{userName}}
                <v-avatar size="36" class="ml-2"><v-img :src="userPhoto"/></v-avatar> </v-btn> -->
          </v-toolbar-items>
    </v-app-bar>
</template>

<script setup>
import { ref } from 'vue';

const menuTabs = ref([ 
    {
        id: 0,
        name: 'Главная',
        icon: 'mdi-access-point',
        route: '/'
    },
    {
        id: 1,
        name: 'Домашняя',
        icon: 'mdi-house',
        route: '/auth/login'
    },
    {
        id: 2,
        name: 'Профиль',
        icon: 'mdi-house',
        route: '/profile'
    }
]);
</script>