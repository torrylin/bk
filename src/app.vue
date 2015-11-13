<template>
    <div class="bk-header">
        <div class="col-md-9 bk-title">
            <h1>TopForm <small>Power by FastCase</small> </h1>
        </div>
        <div class="col-md-3 bk-nav">
            <ul class="nav nav-pills">
                <li role="presentation"><a v-link="{ path: '/home' }">Home</a></li>
                <li role="presentation"><a v-link="{ path: '/list' }">Setting</a></li>
                <li role="presentation"><a v-link="{ path: '/about' }">Help</a></li>
                <li role="presentation"><a v-link="{ path: '/about' }">Log Out</a></li>
            </ul>
        </div>
    </div>
    <div class="page">
        <router-view></router-view>
    </div>
</template>
<script>
    module.exports = {
        data : function () {
            return {
                msg: 'Hello World!!'
            }
        },
        components: {

        }
    };
</script>
<style>
    .bk-title {
    }
    .bk-nav {
        margin-top: 5px;
    }
    .bk-header {
        margin-top: 0;
        background-color: #373b41;
        padding: 10px;
        color: #f0ad4e;
        height: 70px;
        border-bottom: 10px solid;
    }
    .bk-header h1 {
        margin-top: 0;
    }
    .bk-nav li a{
        color: #ccc;
    }
    .page {
        margin: 10px;
        background-color: #ccc;
        height: 800px;
        width: 1200px;
    }
</style>
