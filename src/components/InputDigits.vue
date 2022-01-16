<template>
    <div class="inputDigits flex justify-center my-10">
        <input maxlength="1" type="text" class="digits mx-2">
        <input maxlength="1" type="text" class="digits mx-2">
        <input maxlength="1" type="text" class="digits mx-2">
        <input maxlength="1" type="text" class="digits mx-2">
        <input maxlength="1" type="text" class="digits mx-2">
        <input maxlength="1" type="text" class="digits mx-2">
    </div>
</template>

<script>
export default {
    name: 'InputDigits',
    method: {
    },
}
</script>

<style lang="css">
    .digits {
        width: 45px;
        border-bottom: 4px solid #E5E5E5;
        text-align: center;
        color: #747474;
    }
    .digits:focus-visible {
        outline: none;
    }
</style>