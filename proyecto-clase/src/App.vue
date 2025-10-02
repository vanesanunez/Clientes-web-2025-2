<script>
import { RouterLink, RouterView } from 'vue-router';
import Home from './pages/Home.vue';

export default {
    name: 'App', 
    components: { Home }, 

}
</script>

<template>
<nav>
    <div>
        <ul>
            <li>
                <RouterLink class="nav-link" to="/">Home</RouterLink>
            </li>
            <li>
                <RouterLink class="nav-link" to="/chat">Chat general</RouterLink>
            </li>
            <li>
                <RouterLink class="nav-link" to="/ingresar">Ingresar</RouterLink>
            </li>
            <li>
                <RouterLink class="nav-link" to="/crear-cuenta">Registrarse</RouterLink>
            </li>
        </ul>
    </div>
</nav>
<main>
    <RouterView />
</main>

</template>