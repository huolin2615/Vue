<template>
	<div>
	<div class="recommend-title">热销推荐</div>
	<ul>
		<li class="item border-bottom" v-for="item of recommendList" :key="item.id">
			<img class="item-img" :src='item.imgUrl' />
			<img class="item-img-top" :src='item.imgUrlTop' />
			<div class="item-label">{{item.label}}</div>
			<div class="item-info">
				<p class="item-recommend-title">{{item.title}}</p>
				<p class="item-desc">{{item.desc}}</p>
				<button class="item-button">查看详情</button>
			</div>
		</li>
	</ul>
	</div>
</template>

<script>
export default {
    name: 'HomeRecommend',
    data () {
        return {
					recommendList: [{
						id: '0001',
						imgUrl: 'http://img1.qunarzz.com/sight/p0/1907/8d/8da769b8a045ec98a3.img.jpg_200x200_f74bf17b.jpg',
						imgUrlTop: 'https://img1.qunarzz.com/piao/fusion/1802/52/b9080e45b69b4f02.png',
						title: '深圳欢乐谷',
						desc: '玛雅水公园，夏日玩水好去处',
						label: '可订明日'
					}, {
							id: '0002',
						imgUrl: 'http://img1.qunarzz.com/sight/p0/1507/64/34362835b4a219af8b36803d31a6380f.water.jpg_200x200_bc5c0452.jpg',
						imgUrlTop: 'https://img1.qunarzz.com/piao/fusion/1802/20/2ba6d10b17972e02.png',
						title: '深圳小梅沙海洋世界',
						desc: '这里特别受欢迎哟(๑‾ ꇴ ‾๑)',
						label: '随买随卖'
					}, {
							id: '0003',
						imgUrl: 'http://img1.qunarzz.com/sight/p0/1905/e6/e683c8cf5e97ce03a3.img.jpg_200x200_4769276c.jpg',
						imgUrlTop: 'https://img1.qunarzz.com/piao/fusion/1802/20/2ba6d10b17972e02.png',
						title: '世界之窗',
						desc: '国际啤酒节清凉一夏，夜场49.9元',
						label: '可订今日'
					}]
        }
    }
}
</script>

<style lang="stylus" scoped>
	.recommend-title
		line-height: .8rem
		background: #eee
		text-indent: .2rem
	.item
		overflow: hidden
		display: flex
		height: 1.9rem
		.item-img
			width: 1.7rem
			height: 1.7rem
			padding: .1rem
		.item-img-top
			position: absolute
			width: 1.05rem
			height: .4rem
			padding: .1rem
		.item-label
			position: absolute
			width: .98rem
			height: .25rem
			padding: .08rem
			z-indent: 3
			margin-top: .1rem
			margin-left: .05rem
			left: 0
			top: 0
			font-size: .2rem
			color: #ffffff
		.item-info
			flex: 1
			padding: .1rem
			min-width: 0
			.item-recommend-title
				line-height: .54rem
				font-size: .32rem
				overflow: hidden
				white-space: nowrap
				text-overflow: ellipsis
			.item-desc
				line-height: .4rem
				color: #ccc
				overflow: hidden
				white-space: nowrap
				text-overflow: ellipsis
			.item-button
				line-height: .44rem
				margin-top: .16rem
				background: #ff9300
				padding: 0 .2rem
				border-radius: .06rem
				color: #fff
</style>
