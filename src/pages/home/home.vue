<template>
    <div id="app">
        <router-view></router-view>
        <bottom></bottom>
    </div>
</template>

<script>
    import bottom from '../../components/bottom'
    export default {
        components : {
            bottom
        }
    }
</script>

<style scoped>
</style>