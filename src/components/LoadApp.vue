<template>
    <div id="load-animate" v-if="state.load_status">
        <div class="load">
            <div class="img">
                <img src="../../assets/Load/2.webp" alt="">
            </div>
        </div>
    </div>
</template>
<script>
    import { reactive , onMounted} from 'vue';
export default {
    setup() {
        const state = reactive({
            load_status:true
        })

        

        onMounted(() => {
            const body = document.querySelector('body');
            body.style.overflow = "auto";
            state.load_status = false;
        }) 


        return {
            state
        }
    }
}
</script>
<style lang="scss">
    @import '../../sass/main'
</style>