<template>
    <h1 class="title">{{ name }}</h1>
</template>

<script>
export default {
    name: 'Titles',
    props:  {
        name: String
    }
}
</script>

<style lang="css">
    .title {
        font-size: 40px;
    }
</style>