<script>
export default {
    props: {
        text: String,
    }
}
</script>

<template>
    <div>
        <ul class="list-unstyled">
            <li class="mx-2">
                {{ text }}
            </li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
    
</style>