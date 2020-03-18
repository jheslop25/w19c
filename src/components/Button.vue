<template>
    <div>
        <button @click="updateTweetCol" class="btn btn-primary">click to toggle</button>
    </div>
</template>

<script>
    export default {
        name: 'Button',
        methods: {
            updateTweetCol: function(){
                this.$root.$emit('heyYouToggle');
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>