
# Markdown使用-9 标签页实现

在`markdown`中实现标签页功能需要使用`html/css/js`实现

## 示例一

点击按钮切换图片

```
<script src="http://libs.baidu.com/jquery/2.1.4/jquery.min.js"></script>
<style>
#hello{width:108px;height:108px;border:1px solid #369;overflow:hidden;margin:auto;}
#word{margin:auto;width:136px;}
</style>
 
<div id="hello">
<img src="http://i1.baidu.com/it/u=2390401277,3891827753&fm=203">
<img src="http://i1.baidu.com/it/u=3713675608,2219355047&fm=203">
<img src="http://i2.baidu.com/it/u=695011303,1300693603&fm=203">
</div>
 
<div>
<input type="button" value="上一张" onclick="a()";>
<input type="button" value="下一张" onclick="b()";>
</div>
 
<script>
function a(){
    $('#hello').find('img').eq(0).appendTo($('#hello'));
}
function b(){
    $('#hello').find('img:last').eq(0).prependTo($('#hello'));
}
 
</script>
```


<script src="http://libs.baidu.com/jquery/2.1.4/jquery.min.js"></script>
<style>
#hello{width:108px;height:108px;border:1px solid #369;overflow:hidden;margin:auto;}
#word{margin:auto;width:136px;}
</style>
 
<div id="hello">
<img src="http://i1.baidu.com/it/u=2390401277,3891827753&fm=203">
<img src="http://i1.baidu.com/it/u=3713675608,2219355047&fm=203">
<img src="http://i2.baidu.com/it/u=695011303,1300693603&fm=203">
</div>
 
<div>
<input type="button" value="上一张" onclick="a()";>
<input type="button" value="下一张" onclick="b()";>
</div>
 
<script>
function a(){
    $('#hello').find('img').eq(0).appendTo($('#hello'));
}
function b(){
    $('#hello').find('img:last').eq(0).prependTo($('#hello'));
}
 
</script>

## 示例二

参考：[Bootstrap 标签页（Tab）插件](http://www.runoob.com/bootstrap/bootstrap-tab-plugin.html)

使用`bootstrap`进行标签页的设置