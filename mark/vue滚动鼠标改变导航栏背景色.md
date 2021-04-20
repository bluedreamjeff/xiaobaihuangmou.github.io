# vue滚动鼠标改变导航栏背景色
---
```
vue中滚动页面，改变样式&&导航栏滚动时，样式透明度修改
.vue
<div class="commonHeader" v-bind:class="{ 'navActive': scrollFlag }">
<img src="@/images/home/icon_jdjr.png"  v-bind:class="{ 'scrollFlag': scrollFlag }">
data
scrollFlag:false,
mounted
window.addEventListener('scroll', this.handleScroll)

methods
handleScroll () {
  let _this=this;
  var scrollTop = window.pageYOffset || document.documentElement.scrollTop || document.body.scrollTop
  // console.log(scrollTop)
  if(scrollTop){
    _this.scrollFlag=true
  }else{
    _this.scrollFlag=false
  }
}
```
---
[来源网页](https://www.cnblogs.com/shuihanxiao/p/9890274.html "滚动鼠标改变导航栏背景色")    