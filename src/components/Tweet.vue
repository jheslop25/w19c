<template>
    <div class="card m-3 p-1">
        <p>{{ content }}</p>
    </div>
</template>

<script>
    export default {
        name: 'Tweet',
        props: {
            content: String
        }
    }
</script>

<style lang="scss" scoped>

</style>