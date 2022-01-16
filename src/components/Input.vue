<template>
    <input class="input my-4" :type="type" :placeholder="placeholder">
</template>

<script>
export default {
    name: 'Input',
    props: {
        type: String,
        placeholder: String
    }
}
</script>

<style lang="css">
    .input {
        background: #E5E5E5;
        width: 300px;
        height: 50px;
        border-radius: 50px;
        color: #747474;
        padding: 0px 25px;
        font-size: 12px;
    }
    .input:focus-visible {
        outline: none;
    }
</style>