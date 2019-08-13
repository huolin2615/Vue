<template>
	<div>
	<div class="recommend-title">热销推荐</div>
	<ul>
		<router-link tag="li" class="item border-bottom" v-for="item of list" :key="item.id" :to="'/detail/' + item.id">
			<img class="item-img" :src='item.imgUrl' />
			<img class="item-img-top" :src='item.imgUrlTop' />
			<div class="item-label">{{item.label}}</div>
			<div class="item-info">
				<p class="item-recommend-title">{{item.title}}</p>
				<p class="item-desc">{{item.desc}}</p>
				<button class="item-button">查看详情</button>
			</div>
		</router-link>
	</ul>
	</div>
</template>

<script>
export default {
	name: 'HomeRecommend',
	props: {
		list: Array
	}
}
</script>

<style lang="stylus" scoped>
	.recommend-title
		line-height: .8rem
		background: #eee
		text-indent: .2rem
	.border-bottom
		&:before
			border-color: #ccc
		&:after
			border-color: #ccc
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
