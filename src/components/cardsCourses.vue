<script>
export default {
    props: {
        img: String,
        price: String,
        title: String,
        lessons: String,
        students: String,
    }
}
</script>

<template>
    <div class="col-4">
        <img :src="img" alt="" class="w-100 pb-4">
        <span class="color-2">{{ price }}</span>
        <p class="font-5"><strong>{{ title }}</strong></p>
        <span><i class="fa-regular fa-file"></i> {{ lessons }}</span>
        <span class="ms-4"><i class="fa-regular fa-user"></i> {{ students }}</span>
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
</style>