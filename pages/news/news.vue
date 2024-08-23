<template>
	<view class="">
		<view class="new-title">
			FATFC新闻
		</view>
		<view class="new">
			<view class="new-item" v-for="i in 5">
				<view class="new-item-pic">
					<img src="static/new1.jpeg" alt="">
				</view>
				<div class="new-item-content">官方 | 姆巴佩加盟FATFC</div>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style>
.new-item {
		display: flex;
		align-items: center;
		justify-content: space-between;
		width: 100%;
		height: 100px;
		padding: 10px 0;
		border-bottom: 1px solid #E6E6E6;
		margin: 0 10px;
	}
	.new-item-pic {
		width: 30%;
	}
	.new-item-pic img{
		width: 80%;
	}
	.new-item-content {
		width: 60%;
	}
	.new-title {
		width: 100%;
		text-align: center;
		font-size: 20px;
		font-weight: 600;
		background-image: linear-gradient(to right, #4facfe 0%, #00f2fe 100%);
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
	}
</style>
