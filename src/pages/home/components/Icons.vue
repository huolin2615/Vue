<template>
    <div class="icons">
        <div class="icon">
					<div class='icon-img'>
					<img class='icon-img-content' src='http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png' />
					<p>景点门票</p>
					</div>
				</div>
				<div class="icon">
					<div class='icon-img'>
					<img class='icon-img-content' src='http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png' />
					<p>深圳必游</p>
					</div>
				</div>
				<div class="icon">
					<div class='icon-img'>
					<img class='icon-img-content' src='http://img1.qunarzz.com/piao/fusion/1803/4d/a1eda1a2b8414302.png' />
					<p>暑期夜场</p>
					</div>
				</div>
				<div class="icon">
					<div class='icon-img'>
					<img class='icon-img-content' src='http://img1.qunarzz.com/piao/fusion/1803/50/26ffa31b56646402.png' />
					<p>海洋馆</p>
					</div>
				</div>
				<div class="icon">
					<div class='icon-img'>
					<img class='icon-img-content' src='http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png' />
					<p>一日游</p>
					</div>
				</div>
				<div class="icon">
					<div class='icon-img'>
					<img class='icon-img-content' src='http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20194/cba147cf6cfcea7109d0bff6aac6f626.png' />
					<p>深圳动物园</p>
					</div>
				</div>
				<div class="icon">
					<div class='icon-img'>
					<img class='icon-img-content' src='http://img1.qunarzz.com/piao/fusion/1803/a6/6d97515091789602.png' />
					<p>世界之窗</p>
					</div>
				</div>
				<div class="icon">
					<div class='icon-img'>
					<img class='icon-img-content' src='http://img1.qunarzz.com/piao/fusion/1803/b6/37560ece9c62b502.png' />
					<p>东部华侨城</p>
					</div>
				</div>
    </div>
</template>

<script>
export default {
    name: 'HomeIcons',
    data () {
        return {
        }
    }
}
</script>
<style lang="stylus" scoped>
	.icons
		overflow: hidden
		height: 0
		padding-bottom: 50%
		.icon
			position: relative
			overflow: hidden
			float: left
			width: 25%
			height: 0
			padding-bottom: 25%
		.icon-img
			position: absolute
			top: 0
			left: 0
			right: 0
			bottom: .44rem
			box-sizing: border-box
			padding: .1rem
			text-align: center
			.icon-img-content
				display: block
				margin: 0 auto
				height: 100%
		.icon-desc
			position: absolute
			left: 0
			right: 0
			botton: 0
			height: .44rem
			line-height: .44rem
			color: #333
</style>
