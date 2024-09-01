<script>
export default {
    
}
</script>

<template>
    <div>
        <div class="footer-bg py-5">
            <div class="container">
                <div class="row g-0">
                    <div class="col-6">
                        <div class="content"></div>
                    </div>
                    <div class="col-3">
                        <div class="content"></div>
                    </div>
                    <div class="col-3">
                        <div class="content"></div>
                    </div>
                </div>
                <div class="row pt-4">
                    <div class="col-12">
                        <div class="content"></div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
.content {
        width: 100%;
        height: 60px;
        background-color: blueviolet;
        border: 1px solid black;
    }

    .footer-bg {
        background-color: $color-3;
    }
</style>