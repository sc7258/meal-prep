<!--
<template>
    <v-app>
        <v-toolbar app>
            <v-toolbar-title class="headline text-uppercase">
                <span>Vuetify</span>
                <span class="font-weight-light">MATERIAL DESIGN</span>
            </v-toolbar-title>
            <v-spacer></v-spacer>
            <v-btn
                flat
                href="https://github.com/vuetifyjs/vuetify/releases/latest"
                target="_blank"
            >
                <span class="mr-2">Latest Release</span>
            </v-btn>
        </v-toolbar>

        <v-content>
            <HelloWorld />
        </v-content>
    </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
    name: 'App',
    components: {
        HelloWorld
    },
    data() {
        return {
            //
        };
    }
};
</script>
-->

<template>
    <v-app>
        <app-navigation></app-navigation>

        <!-- <v-content transition="slide-x-transition"> -->
        <v-content >
            <router-view></router-view>
        </v-content>
    </v-app>
</template>

<script>
import AppNavigation from '@/components/AppNavigation';
export default {
    name: 'App',
    components: {
        AppNavigation
    }    
};
</script>

<style>
</style>