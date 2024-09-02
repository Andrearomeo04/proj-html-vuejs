<script>
import mainMenu from '../data/headerMenues.json'
import headerMenu from '../components/headermenu.vue'
export default {
    components: {
        headerMenu
    },
    data () {
        return {
            mainMenu
        }
    }
}
</script>

<template>
    <div>
        <div class="container">
            <div class="row g-0">
                <div class="col-4 d-flex">
                    <headerMenu 
                        v-for="(info, index) in mainMenu"
                        :key="index"
                        :text="info.text"
                    />
                </div>
                <div class="col-4">
                    s
                </div>
                <div class="col-4">
                    <div class="content"></div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .content {
        width: 100%;
        height: 60px;
        background-color: blueviolet;
        border: 1px solid black;
    }

</style>