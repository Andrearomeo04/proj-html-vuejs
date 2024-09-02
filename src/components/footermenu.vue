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
    ul {
        li {
            line-height: 40px;
        }
    }
</style>