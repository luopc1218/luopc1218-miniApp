<template>
	<view class="me">
		<view class="header">
			<image class="avatar"></image>
			<view class="userName">
				请先登录
			</view>
		</view>
		<view class="modules">
			<uni-group mode="card">
				<uni-list>
					<uni-list-item clickable title="我的收藏" to="`./index`" showArrow />

				</uni-list>

			</uni-group>
			<uni-group mode="card" title="管理员选项">
				<uni-list>
					<uni-list-item clickable title="我的文章" to="`./index`" showArrow />
					<uni-list-item clickable title="系统设置" to="`./index`" showArrow />
				</uni-list>
			</uni-group>
		</view>
		<view class="signOut">
			<button class="btn">登出</button>
		</view>
	</view>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped>
	.me {
		.header {
			display: flex;
			padding:2rem 1rem;
			align-items: center;

			.avatar {
				border: 1px solid $uni-primary;
				box-sizing: border-box;
				width: 4rem;
				height: 4rem;
				border-radius: 4rem;
				margin-right: 1rem;
			}

			.userName {
				color:$uni-primary;
			}
		}

		.modules {}

		.signOut {
			padding: 1rem;

			.btn {
				background-color: $uni-primary;
				color: #fff;
			}
		}
	}
</style>
