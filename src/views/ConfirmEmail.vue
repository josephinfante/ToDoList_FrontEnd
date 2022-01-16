<template>
    <div class="confirmEmail">
        <Titles name="Confirma tu correo"/>
        <InputDigits />
        <Button btn_text="Confirmar correo"/>
    </div>
</template>

<script>
import Titles from '@/components/Titles';
import Button from '@/components/Button';
import InputDigits from '@/components/InputDigits';

export default {
    name: 'ConfirmEmail',
    components : {
        Titles,
        Button,
        InputDigits
    },
}
</script>

<style lang="css">
    
</style>