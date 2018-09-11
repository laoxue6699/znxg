<template>
    <div>
        <nav class="mui-bar mui-bar-tab">
			<span class="mui-tab-item mui-active touch"  @click="goto('/home')">
				<span class="mui-icon mui-icon-home"></span>
				<span class="mui-tab-label">首页</span>
			</span>
			<span class="mui-tab-item touch" @click="goto('/stoke')" >
				<span class="mui-icon mui-icon-search"></span>
				<span class="mui-tab-label">库存</span>
			</span>
			<span class="mui-tab-item touch"  @click="goto('/sale')" >
				<span class="mui-icon mui-icon-map"></span>
				<span class="mui-tab-label">销售</span>
			</span>
			<span class="mui-tab-item touch"  @click="goto('/capital')">
				<span class="mui-icon mui-icon-gear"></span>
				<span class="mui-tab-label">资金</span>
			</span>
			<span class="mui-tab-item touch" @click="goto('/profile')">
				<span class="mui-icon mui-icon-contact"></span>
				<span class="mui-tab-label">我</span>
			</span>
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
	.active {color: #007aff;}
</style>