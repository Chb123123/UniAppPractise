<script>
	export default {
		onLaunch: function() {
			console.log('App Launch')
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		},
		onPageNotFound() {
			uni.navigateTo({
				url:'/pages/notMove/notMove'
			})
		}
	}
</script>

<style>
	/*每个页面公共css */
	view {
		color: blue;
	}
</style>
