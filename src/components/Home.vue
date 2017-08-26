<template>
<div id="tmpl">
<!--1.0轮播图-->
<mt-swipe :auto="2000">
  <mt-swipe-item v-for="item in list">
      <img :src="item.img">
  </mt-swipe-item>
  
</mt-swipe>
</div>    

</template>

<script>
export default {
  data(){
      return{
  list:[
  {"url":"http://www.itcast.cn/subject/phoneweb/index.html","img":"http://ofv795nmp.bkt.clouddn.com/vuelogobanner1.jpg"},{"url":"http://www.itcast.cn/subject/phoneweb/index.html","img":"http://ofv795nmp.bkt.clouddn.com/vuelogobanner2-1.jpg"}
  ]
}
}
}
</script>
  
<style scoped>
    .mint-swipe{
        height: 300px;
    }
   .mint-swipe-item img{
       width: 100%;
   }
    .mint-swipe-item{
        background-color: red;
        width: 100%;
        height: 300px;
    }
</style>   