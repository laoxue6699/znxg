<template>
    <div>
        <nav class="mui-bar mui-bar-tab">
			<a class="mui-tab-item mui-active touch"  @click="goto('/stoke')">
				<span class="mui-icon mui-icon-home"></span>
				<span class="mui-tab-label">库存</span>
			</a>
			<a class="mui-tab-item touch" href="#tabbar-with-chat" @click="goto('/sale')">
				<span class="mui-icon mui-icon-email"></span>
				<span class="mui-tab-label">销售</span>
			</a>
			<a class="mui-tab-item touch" href="#tabbar-with-contact" @click="goto('/capital')">
				<span class="mui-icon mui-icon-gear"></span>
				<span class="mui-tab-label">资金</span>
			</a>
			<a class="mui-tab-item touch" href="#tabbar-with-map" @click="goto('/profile')">
				<span class="mui-icon mui-icon-contact"></span>
				<span class="mui-tab-label">我</span>
			</a>
		</nav>
    </div>
</template>

<script>
    export default {
        methods: {
            goto(path) {
                this.$router.replace(path)
            }
        }
    }
</script>

<style scoped>
	.touch {touch-action: none;}
</style>