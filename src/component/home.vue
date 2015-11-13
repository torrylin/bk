<script>
	module.exports = {
	    data : function () {
	        return {
	            msg: 'Hello World!!'
	        }
	    },
	    components: {
	    	newclient: require('./home/new_client.vue')
	    }
	};
</script>

<template>
	<newclient></newclient>
	<ul class="subnav">
		<li><a v-link="{ path: '/home/1' }">Home1</a></li>
		<li><a v-link="{ path: '/home/2' }">Home2</a></li>
		<li><a v-link="{ path: '/home/3' }">Home3</a></li>
	</ul>
	<div class="subpage">
		<router-view></router-view>
	</div>
</template>

<style>
	.subnav {
		float: left;
	}
	.subpage {
		margin-left: 50px;
		float: left;
		width: 400px;
		height: 500px;
		background-color: #fff;
	}
</style>