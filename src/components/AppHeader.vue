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
        <div class="container-fluid px-5">
            <div class="row g-0 align-items-center py-2">
                <div class="col-4 d-flex">
                    <headerMenu 
                        v-for="(info, index) in mainMenu"
                        :key="index"
                        :text="info.text"
                    />
                </div>
                <div class="col-4 d-flex justify-content-center">
                    <img src="../assets/img/dark-logo.png" alt="dark-logo">
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

    img {
        width: 150px;
    }

</style>