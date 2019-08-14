<template>
<div>
	<div class="banner" @click="handleBannerClick">
			<img class="banner-img" :src="bannerImg" />
			<div class="banner-info">
				<div class="banner-tittle">{{this.sightName}}</div>
				<div class="banner-number">
					<span class="iconfont banner-icon">&#xe692;</span>{{this.gallaryImgs.length}}</div>
			</div>
	</div>
	<animation>
	<common-gallary :imgs="gallaryImgs" v-show="showGallary" @close="handleGallaryClose"></common-gallary>
	</animation>
</div>
</template>

<script>
import CommonGallary from '@/common/gallary/Gallary'
import Animation from '@/common/animation/Animation'
export default {
		name: 'DetailBanner',
		props: {
			sightName: String,
			bannerImg: String,
			gallaryImgs: Array
		},
		methods: {
			handleBannerClick () {
				this.showGallary = true
			},
			handleGallaryClose () {
				this.showGallary = false
			}
		},
		components: {
			CommonGallary,
			Animation
		},
    data () {
        return {
					showGallary: false
        }
    }
}
</script>

<style lang="stylus" scoped>
	.banner
		position: relative
		overflow: hidden
		height: 0
		padding-bottom: 55%
		.banner-img
			width: 100%
		.banner-info
			display: flex
			position: absolute
			left: 0
			right: 0
			bottom: 0
			line-height: .6rem
			color: #fff
			background-image: linear-gradient(top, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.8))
			.banner-tittle
				flex: 1
				font-size: .32rem
				padding: 0 .2rem
			.banner-number
				margin-top: .14rem
				padding: 0 .4rem
				height: .32rem
				line-height: .32rem
				border-radius: .2rem
				background: rgba(0, 0, 0, .8)
				font-size: .24rem
				.banner-icon
					font-size: .24rem
</style>
