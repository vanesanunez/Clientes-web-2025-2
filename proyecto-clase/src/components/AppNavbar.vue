<script>
import { RouterLink } from 'vue-router';

export default {
    name: 'AppNavbar',
}
</script>

<template>
    <nav class="flex items-center p-4 gap-8 bg-violet-700 text-white">
        <RouterLink class="text-xl" to="/">Red social</RouterLink>
        <div>
            <ul class="flex gap-4">
                <li>
                    <RouterLink class="nav-link" to="/">Inicio</RouterLink>
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
</template>