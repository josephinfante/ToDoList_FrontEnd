<template>
    <div class="card py-5 px-5" :id="id">
        <div class="flex justify-between">
            <div class="img">  
                <img src="../assets/icons/home-solid.svg" alt="">
            </div>
            <div class="custom_checkbox">
                <input type="checkbox" :id="task_name" />
                <label :for="task_name"></label>
            </div>
        </div>
        <div class="text-left mt-5 card_text">
            <p>{{ task_name }}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'TaskCard',
    props: {
        id: Number,
        task_name: String
    }
}
</script>

<style lang="css">
    .card {
        background: #FEFFEA;
        width: 200px;
        height: 200px;
        border-radius: 30px;
        box-shadow: 0px 5px 10px rgba(0, 0, 0, 0.4);
    }
    .img {
        width: 30px;
        height: 30px;
    }
    .card input[type="checkbox"] {
        display: none;
    }
    .card label {
        position: relative;
    }
    .card label::before {
        content: "";
        background: url("../assets/icons/check-circle-solid.svg");
        background-position: center;
        background-size: contain;
        width: 30px;
        height: 30px;
        position: absolute;
        left: -25px;
        top: -2px;
        transform: scale(0) rotateZ(180deg);
        transition: 0.4s cubic-bezier(0.54, 0.1, 0, 1.49);
    }
    .card input[type="checkbox"]:checked + label::before {
        transform: scale(1) rotateZ(0deg);
    }
    .card label::after {
        content: "";
        width: 30px;
        height: 30px;
        position: absolute;
        left: -25px;
        top: -2px;
        border-radius: 50%;
        box-shadow: 0px 5px 10px rgba(0, 0, 0, 0.5);
    }
    .card_text {
        font-size: 15px;
        max-height: 110px;
        overflow: auto;
    }
</style>