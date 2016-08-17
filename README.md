# xiaomiguanwang
#移动端的小米案例
==============
##使用rem方案根据浏览器的宽度来改变而rem改变
--------
设置：<br>
\<meta name = "viewport" content = "with = device-with"> <br>
使用jQuery[size=1em]调用函数fullWidth() <br>   
```javascript
function fullWidth() {
  if($('body').width() >= 720px) {     //设置最大宽度为720px; 当大于720px时，设置html根的font-size为100px;
    $('html').css('font-size',100 + 'px');
    return;
  }
  var scale = $('body').width()/720;
  $('html').css('font-size',scale * 100 + 'px');
}
```
