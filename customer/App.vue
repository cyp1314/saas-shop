<script>
	export default {
		onLaunch: function() {
			console.log('App Launch')
			console.log(this.$u.config.v);
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style lang="scss">
	@import "uview-ui/index.scss";
	@import "static/css/common.css";
	/*每个页面公共css */
	@import "static/iconfont/iconfont.css";
</style>
