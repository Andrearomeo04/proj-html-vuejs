<script>
export default {
    props: {
        text: String,
    }
}
</script>

<template>
    <div>
        <ul class="list-unstyled mb-0">
            <li class="mx-4">
                {{ text }}
            </li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
    
</style>