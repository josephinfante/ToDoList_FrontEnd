<template>
    <div class="login">
        <Titles name="Inicia sesión"/>
        <div v-for="i in inputs" :key="i.placeholder">
            <Input :type="i.type" :placeholder="i.placeholder"/>
        </div>
        <div class="mt-8 mb-10 text-right link mx-auto">
            <router-link :to="{ name: 'Home' }">Olvidaste tu contraseña?</router-link>
        </div>
        <Button btn_link="/" btn_text="Iniciar sesión" />
    </div>
</template>

<script>
import Titles from '@/components/Titles';
import Input from '@/components/Input';
import Button from '@/components/Button';

export default {
    name: 'Login',
    components : {
        Titles,
        Input,
        Button
    },
    data() {
        return {
            inputs: [
                {
                    type: 'email',
                    placeholder: 'Correo electrónico'
                },
                {
                    type: 'password',
                    placeholder: 'Contraseña'
                }
            ]
        }
    }
}
</script>

<style lang="css">
    .link {
        width: 300px;
    }
</style>