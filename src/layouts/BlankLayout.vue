<template>
    <div style="height: 100%">
        <router-view :key="key"/>
    </div>
</template>

<script>
    export default {
        name: "BlankLayout",
        computed: {
            key(){
                return this.$route.path + Math.random();
            }
        }
    }
</script>

<style scoped>

</style>
