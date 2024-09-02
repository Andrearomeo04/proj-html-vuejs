<script>
export default {
    props: {
        address: Object,
        explore: Object,
        information: Object,
    }
}
</script>

<template>
    <div>
        <div class="container">
            <div class="row">
                <div class="col-6 text-white">
                    <h5>{{ address.title }}</h5>
                    <ul class="list-unstyled">
                        <li v-for="(detail, index) in address.details" :key="index">{{ detail }}</li>
                        <li class="mt-4">
                            <i class="fa-brands fa-facebook me-3 fs-3 color-8"></i>
                            <i class="fa-brands fa-twitter mx-3 fs-3 color-8"></i>
                            <i class="fa-brands fa-instagram mx-3 fs-3 color-8"></i>
                            <i class="fa-brands fa-linkedin mx-3 fs-3 color-8"></i>
                        </li>
                    </ul>
                </div>
                <div class="col-3 text-white">
                    <h5>{{ explore.title }}</h5>
                    <ul class="list-unstyled">
                        <li v-for="(link, index) in explore.links" :key="index">{{ link }}</li>
                    </ul>
                </div>
                <div class="col-3 text-white">
                    <h5>{{ information.title }}</h5>
                    <ul class="list-unstyled">
                        <li v-for="(link, index) in information.links" :key="index">{{ link }}</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
    ul {
        li {
            line-height: 40px;
        }
    }
    .color-8 {
        color: $color-7;
    }
    i:hover {
        color: $color-2;
    }
    .col-3 {
        ul {
            li:hover {
                color: $color-2;
            }
        }
    }
</style>