<script>
import MainButton from '../components/MainButton.vue';
import MainLoader from '../components/MainLoader.vue';

export default {
    name: 'Login',
    components: {MainButton, MainLoader},
}
</script>

<template>
    <h1>Ingresar a mi cuenta</h1>

    <div v-if="loading" class="flex justify-center items-center h-40">
    <MainLoader />
    </div>

    <form v-else
        action="#"
        @submit.prevent="handleSubmit"
    >
        <div class="mb-4">
            <label for="email" class="block mb-2">Email</label>
            <input 
                type="email"
                id="email"
                class="w-full p-2 border border-violet-400"
                v-model="user.email"
            >
        </div>
        <div class="mb-4">
            <label for="password" class="block mb-2">Contraseña</label>
            <input 
                type="password"
                id="password"
                class="w-full p-2 border border-violet-400 rounded"
                v-model="user.password"
            >
        </div>
        <MainButton 
            type="submit" >
                <template v-if="!updating">Ingresar</template>
                <MainLoader v-else />
            </MainButton>
    </form>
</template>