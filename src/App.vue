<template>
	<div id="app">
		<img alt="Vue logo" src="./assets/logo.png">
		<ckeditor v-model='content'></ckeditor>

		<button @click="getContent">获取内容</button>
		<div id="content" v-html="content"></div>
	</div>
</template>

<script>
	export default {
		name: 'app',
		data() {
			return{
				content: 'AA'
			}
		},
		methods: {
			getContent() {
				alert(this.content)
			}
		}
	}
</script>

<style>

</style>
