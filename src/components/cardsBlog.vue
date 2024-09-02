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
    <div class="col-4">
        <img :src="img" alt="" class="w-100 pb-4">
        <span>{{ profession }}</span>
        <p class="font-5"><strong>{{ title }}</strong></p>
        <span class="color-8"><i class="fa-regular fa-calendar"></i> {{ date }}</span>
        <span class="ms-4 color-8"><i class="fa-regular fa-eye"></i> {{ views }}</span>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
    img {
    object-fit: cover;
    cursor: pointer;
    border-radius: 5px;
}
.font-5 {
    font-size: $font-8;
}
span {
    i {
        font-size: $font-2;
        margin-right: 5px;
    }
}
.color-8 {
    color: $color-8;
}
</style>