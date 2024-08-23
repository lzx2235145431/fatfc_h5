<template>
	<view class="content">
		<view class="header">
			<img src="static/fat_logo.jpg" alt="">
		</view>
		<view class="nav">
			<view class="nav-item">新闻</view>
			<view class="nav-item">商店</view>
			<view class="nav-item">加入我们</view>
		</view>
		<swiper class="banner" autoplay indicator-dots="true" duration="1000">
			<swiper-item>
				<view class="swiper-item">
					<img src="static/banner1.jfif" alt="">
					<view class="title">FATFC夺冠</view>
				</view>
			</swiper-item>
			<swiper-item>
				<view class="swiper-item">
					<img src="static/banner2.jpg" alt="">
					<view class="title">FATFC主力锋线</view>
				</view>
			</swiper-item>
		</swiper>
		<view class="partner-title">
			主要合作伙伴
		</view>
		<view class="partner">
			<view class="partner-item">
				<img src="static/kelme.png" alt="">
			</view>
			<view class="partner-item">
				<img src="static/jsjxy.jpg" alt="">
			</view>
		</view>
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
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.header {
		width: 100%;
		display: flex;
		justify-content: center;
	}
	.header img {
		width: 50%;
	}
	.nav {
		margin-top: 10px;
		width: 100%;
		display: flex;
		justify-content: space-between;
		padding: 10px 0;
		background-image: linear-gradient(to right, #4facfe 0%, #00f2fe 100%);
	}
	.nav-item {
		width: 33%;
		text-align: center;
		border-right: 1px solid #FAF0E6;
		color: #FAF0E6;
	}
	.nav-item:last-child {
		border-right: 0
	}
	.banner {
		width: 100%;
		height: 250px;
	}
	.swiper-item {
		position: relative;
		width: 100%;
		height: 100%;
	}
	.swiper-item img {
		width: 100%;
		height: 100%;
	}
	.title {
		width: 100%;
		font-size: 26px;
		text-align: center;
		position: absolute;
		z-index: 999;
		color: #fff;
		bottom: 50px;
	}
	.partner-title {
		margin: 20px 0;
		width: 100%;
		text-align: center;
	}
	.partner {
		width: 100%;
		height: 100px;
		display: flex;
		justify-content: space-around;
		margin-top: 10px;
	}
	.partner-item {
		width: 20%;
	}
	.partner-item img {
		width: 100%;
	}
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
