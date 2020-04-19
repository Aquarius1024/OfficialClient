<template>
	<view class="content">
    <message-item></message-item>
    <message-item></message-item>
    <message-item></message-item>
    <message-item></message-item>
    <message-item></message-item>
    <message-item></message-item>
    <message-item></message-item>
    
	</view>
</template>

<script>
  import messageItem from "../../components/messageItem/messageItem.vue";
  
	export default {
		data() {
			return {
				
			}
		},
    
    components: {
      messageItem,
    },
    
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>

</style>
