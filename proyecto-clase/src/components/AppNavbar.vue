<script>
export default {
    name: 'AppNavbar',
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
</template>