<template>
    <div class="my-component">
        <ul>
            <li v-for="(value, key) in clubs">{{ key }} - {{ value }}</li>
        </ul>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                clubs: [
                    { name1: 'Real Madrid' },
                    { name2: 'Barcelona' },
                    { name3: 'Manchester United' },
                    { name4: 'Chelsea' },
                    { name5: 'Liverpool' },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
</style>