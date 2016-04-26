# 4-26
width.html //关于多个物体宽度的运动框架

alpha.html //关于多个物体透明度变化的运动框架


由于offsetWidth不是计算后的样式，导致如果加了border之后会产生bug，所以运动框架里应当使用getStyle函数来确保不会发生此类问题。

function getStyle(obj,attr){  </br>
&nbsp;&nbsp;if(obj.currentStyle){ </br>
&nbsp;&nbsp;&nbsp;&nbsp;return obj.currentStyle[attr]; </br> 
&nbsp;&nbsp;}else{ </br>
&nbsp;&nbsp;&nbsp;&nbsp;return getComputerStyle(style,flase)[attr];  </br>
&nbsp;&nbsp;} </br>
}

</div>
        <div class="header_right">
            <a href="#">消息</a>
            <a href="#">糯米</a>
            <a href="#">新闻</a>
            <a href="#">hao123</a>
            <a href="#">地图</a>
            <a href="#">视频</a>
            <a href="#">贴吧</a>
            <a href="#">TAKO喵</a>
            <a href="#">设置</a>
            <a class="more" href="#">更多产品</a>
        </div>
