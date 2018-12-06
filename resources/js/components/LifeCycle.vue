<template>
    <div id="my-text">
        This is my text
    </div>
</template>

<script>
    export default {
        data() {
            return {
                message: 'Hello World'
            }
        },
        beforeCreate() {
            console.log(this.message)
        },
        created() {
            console.log(this.message)

            console.log(document.getElementById('my-text').innerHTML)
        },
        beforeMount() {
            console.log(this)

            console.log(document.getElementById('my-text').innerHTML)
        },
        mounted() {
            console.log(this)

            console.log(document.getElementById('my-text').innerHTML)
        }
    }
</script>

<style lang="scss" scoped>
</style>
