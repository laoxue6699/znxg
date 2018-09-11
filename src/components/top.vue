<template>
    <div id="app">
		<h4>{{pagetitle}}</h4>
    </div>
</template>

<script>
    export default {
        props : {
            pagetitle : String
        }
    }
</script>

<style scoped>
    h4 {
        text-align: center;
        line-height: 40px;
        color: white;
        width: 100%;
        height: 40px;
        background-color: #4093D6;
    }
</style>