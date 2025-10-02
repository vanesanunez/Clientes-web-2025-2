<script>
import { RouterLink, RouterView } from 'vue-router';
import Home from './pages/Home.vue';
import AppNavbar from './components/AppNavbar.vue';
import AppFooter from './components/AppFooter.vue';

export default {
    name: 'App',
    components: { AppNavbar, AppFooter },

}
</script>

<template>
    <AppNavbar />
    <main>
        <RouterView />
    </main>
    <AppFooter />
</template>