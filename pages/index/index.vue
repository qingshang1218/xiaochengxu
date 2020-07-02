<template>
	<view class="content">
		  <yy-video-player 
		    :auto-play="false" 
		    :url="url"  
		    :poster="poster" 
		    :danmu-list="danmuList"  
		    :show-back-btn="true"
		  ></yy-video-player>
	</view>
</template>

<script>
	    import yyVideoPlayer from '@/components/yy-video-player/yy-video-player.nvue';
	export default {
		    components: {
		        yyVideoPlayer
		    },
		data() {
			return {
				url:'https://haokan.baidu.com/v?vid=11954008930827817853&pd=bjh&fr=bjhauthor&type=video'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
