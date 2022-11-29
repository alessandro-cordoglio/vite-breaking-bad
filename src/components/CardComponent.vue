<script>
    export default {
        props:{
            info: Object,
        }
    }
</script>

<template>
        <div class="my_card p-3">
            <div class="card_img text-center">
                <img :src="info.img" alt="">
            </div>
            <div class="card_name text-white text-center">
                {{info.name}}
            </div>
            <div class="card_series text-center">
                {{info.category}}
            </div>
            <div class="card_status text-center">
                {{info.status}}
            </div>
        </div>
</template>

<style lang="scss" scoped>
    .my_card{
        background-color: var(--primary-color);
        width: calc((100%/5) - 20px);
        margin-right:20px ;
        margin-bottom: 20px;
        img{
            max-width: 100%;
        }
        .card_name{
            font-weight: bold;
        }
        .card_series{
            font-size: 18px ;
            color: gray;
        }
        .card_status{
            color: gray;
        }
    }
</style>