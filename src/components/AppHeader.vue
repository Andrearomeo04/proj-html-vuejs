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
        <div class="container-fluid py-2 px-header">
            <div class="row g-0 align-items-center py-3">
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
                <div class="col-4 d-flex justify-content-end align-items-center">
                    <div>
                        <i class="fa-solid fa-cart-shopping mx-3"></i>
                        <i class="fa-regular fa-circle-user mx-3"></i>
                    </div>
                    <div>
                        <form class="d-flex" role="search">
                            <input class="form-control" type="search" placeholder="Search..." aria-label="Search">
                            <button class="btn" type="submit"><i class="fa-solid fa-magnifying-glass"></i></button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .px-header {
        padding: 0px 100px;
    }

    img {
        width: 150px;
    }

</style>