<script>
import AppH1 from '../components/AppH1.vue';
import MainButton from '../components/MainButton.vue';


export default {
    name: 'Login',
    components: {MainButton, AppH1 },
}
</script>

<template>
    <AppH1>Ingresar a mi cuenta</AppH1>
    <form action="#">
        <div class="mb-4">
            <label for="email" class="block mb-2">Email</label>
            <input type="email" id="email" class="w-full p-2 border border-violet-400">
        </div>
        <div class="mb-4">
            <label for="password" class="block mb-2">Contraseña</label>
            <input type="password" id="password" class="w-full p-2 border border-violet-400 rounded">
        </div>
        <MainButton />
    </form>
</template>