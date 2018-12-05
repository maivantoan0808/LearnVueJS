<template>
    <div class="my-component">
        <!-- How to using v-if, v-else, v-else-if, v-show -->
        <div class="block-1" v-if="isActive == false">
            This is block 1
        </div>
        <div class="block-2" v-if="isActive == true">
            This is block 2
        </div>
        <div>
            <button @click="toggleActive">Button</button>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                isActive: true
            }
        },
        methods: {
            toggleActive() {
                if(this.isActive == true) {
                    this.isActive = false
                }
                else {
                    this.isActive = true
                }
            }
        }
    }
</script>

<style lang="scss" scoped>
    .my-component {
        color: red;
    }
</style>