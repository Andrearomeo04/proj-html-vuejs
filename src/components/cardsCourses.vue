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
    <div class="col-4 online">
        <div class="bg-white card-container">
            <img :src="img" alt="" class="w-100 pb-4">
            <div class="pb-5 px-4">
                <strong class="color-2 font-8">{{ price }}</strong>
                <p class="font-8"><strong>{{ title }}</strong></p>
                <span class="color-8"><i class="fa-regular fa-file"></i> {{ lessons }}</span>
                <span class="ms-4 color-8"><i class="fa-regular fa-user"></i> {{ students }}</span>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
    img {
    object-fit: cover;
    cursor: pointer;
    border-radius: 5px;
}
.font-8 {
    font-size: $font-8;
}
span {
    i {
        font-size: $font-2;
        margin-right: 5px;
    }
}
.card-container {
    border-radius: 5px;
}

    p:hover {
        strong {
            color: $color-2;
        }
    }       

.color-2 {
    color: $color-2;
}
.color-8 {
    color: $color-8;
}
</style>