<script>
	export default {
		onLaunch: function() {
			console.log('App Launch')
			//  weex图标使用
			const domModule = weex.requireModule('dom')
			domModule.addRule('fontFace', {
			    'fontFamily': "iconfont",
			    'src': "url('http://at.alicdn.com/t/font_1859985_7mxozsfdvib.ttf')"
			});
			// 监听底部导航中间凸起按钮
			uni.onTabBarMidButtonTap( () => {
				console.log('tab中间点击');
			})
			
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style>
	/*每个页面公共css */
	@import url("/common/free.css");
	@import url("/common/common.css");
	/* #ifndef APP-NVUE */
	@import url("/common/icon.css");
	/* #endif */
</style>
