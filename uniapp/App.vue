<script>
	//应用生命周期仅可在App.vue中监听，在其它页面监听无效。
	//在应用生命周期函数内进行页面跳转时需要注意，不要和pages.json内配置的首页打开时机冲突。
	export default {
		onLaunch: function() {
			//当uni-app 初始化完成时触发（全局只触发一次）
			console.log('App Launch');
		},
		onShow: function() {
			//当 uni-app 启动，或从后台进入前台显示
			console.log('App Show')
		},
		onHide: function() {
			//当 uni-app 从前台进入后台
			console.log('App Hide')
		},
		 // 捕获 app error
	   onError:function (err) {
		   console.log(err)
	   },
		onUniNViewMessage: function(){
			//对 nvue 页面发送的数据进行监听
			console.log('监听数据');
		}
	}
</script>

<style>
	/*每个页面公共css */
</style>
