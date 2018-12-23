<template>
    <div class="box">
        <ul class="list-box">
            <li v-for="(item,i) in list" :key="i" :class="item.isT?'nav-3-li':''"><a :href="item.url">{{ item.name }}</a></li>
        </ul>
        <i>0110</i>
    </div>
</template>

<script>
export default {
    props: ["list"],
    data () {
        return {}
    },
}
</script>

<style scoped>
.box{
    z-index: 1;
    width: 100%;
    background: red;
    position: fixed;
    bottom: 0;left: 0;
}
.list-box{
    width: 100%;
    margin: 0;padding: 10rpx;
}
ul.list-box li{
    width: 232.5rpx;
}
.nav-3-li{
    width: 310rpx;
}
</style>


