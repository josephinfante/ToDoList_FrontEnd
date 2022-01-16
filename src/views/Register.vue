<template>
    <div class="register">
        <Titles name="Registrate"/>
        <div v-for="i in inputs" :key="i.placeholder">
            <Input :type="i.type" :placeholder="i.placeholder"/>
        </div>
        <Button btn_link="ConfirmEmail" btn_text="Registrarme"/>
    </div>
</template>

<script>
import Titles from '@/components/Titles';
import Input from '@/components/Input';
import Button from '@/components/Button';

export default {
    name: 'Register',
    components : {
        Titles,
        Input,
        Button
    },
    data() {
        return {
            inputs: [
                 {
                    type: 'text',
                    placeholder: 'Nombre'
                },
                {
                    type: 'email',
                    placeholder: 'Correo electrónico'
                },
                {
                    type: 'password',
                    placeholder: 'Contraseña'
                },
                {
                    type: 'password',
                    placeholder: 'Confirmar contraseña'
                },
            ]
        }
    }
}
</script>

<style lang="css">
    
</style>