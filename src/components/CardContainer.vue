<script>
import axios from "axios";
import CardComponent from './CardComponent.vue';
    export default {
        components:{
            CardComponent,
        },
        data(){
            return{
                characters:[]
            }
        },
        created() {
            axios.get("https://www.breakingbadapi.com/api/characters").then((resp)=>{
                this.characters= resp.data
            })
        },
    }
</script>

<template>
    <div class="card_container p-5 mt-4">
        <div class="chara_numbers text-white p-3 fw-bold">
            Found {{characters.length}} characters
        </div>
        <div class="card_container p-3 row">
            <CardComponent v-for="char in characters"
                :info="char"/>
        </div>
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