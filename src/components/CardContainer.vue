<script>
import CardComponent from './CardComponent.vue';
    export default {
        components:{
            CardComponent
        }
    }
</script>

<template>
    <div class="card_container p-5 mt-4">
        <div class="chara_numbers text-white p-3 fw-bold">
            Found 62 characters
        </div>
        <CardComponent/>
    </div>
</template>

<style lang="scss" scoped>
    .card_container{
        background-color: white;
        .chara_numbers{
            background-color: var(--secondary-color);

        }
    }
</style>