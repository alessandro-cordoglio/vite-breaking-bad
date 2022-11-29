<script>
import CardContainer from './CardContainer.vue';
    export default {
    components: { 
        CardContainer
     }
}
</script>

<template>
    <div>
        <main>
            <div class="my_container">
                <div class="form ms-2">
                    <select class="form-select w-auto" name="category" id="">
                        <option value="">Select category</option>
                        <option value="">1</option>
                        <option value="">2</option>
                        <option value="">3</option>
                    </select>
                </div>
                <CardContainer/>
            </div>
        </main>
    </div>
</template>

<style lang="scss" scoped>

</style>