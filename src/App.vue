<template>
	<div id="app">
		<ckeditor v-model='content'></ckeditor>

		<button hidden="hidden" @click="getContent">获取内容</button>
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
	*{
		margin: 0;
		padding: 0;
	}
#content{
	width: 80%;
	height: 400px;
	border: 1px dotted green;
	margin: 20px auto;
	overflow: hidden;
}
</style>
