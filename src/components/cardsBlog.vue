<script>
export default {
    props: {
        img: String,
        profession: String,
        title: String,
        date: String,
        views: String,
    }
}
</script>

<template>
    <div>
        <img :src="img" alt="" class="w-100">
        <p>{{ profession }}</p>
        <p><strong>{{ title }}</strong></p>
        <span>{{ date }}</span>
        <span>{{ views }}</span>
    </div>
</template>

<style lang="scss" scoped>
    img {
    object-fit: cover;
    object-position: top;
    cursor: pointer;
}
</style>