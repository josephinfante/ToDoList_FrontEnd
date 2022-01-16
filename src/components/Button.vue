<template>
    <button class="button">
        {{ btn_text }}
    </button>
</template>

<script>
export default {
    name: 'Button',
    props: {
        btn_text: String,
        btn_link: String,
    }
}
</script>

<style lang="css">
    .button {
        min-width: 150px;
        height: 50px;
        border-radius: 50px;
        background: #FCFC62;
        box-shadow: 0px 5px 10px rgba(0, 0, 0, 0.4);
        font-family: 'Poppins-semibold';
        font-size: 15px;
        cursor: pointer;
        transition: 0.1s;
    }
    .button:hover {
        background-color: #FFFF32;
    }
    .button:active {
        transform: translateY(3px);
    }
</style>