# 4-26
width.html //关于多个物体宽度的运动框架

alpha.html //关于多个物体透明度变化的运动框架


由于offsetWidth不是计算后的样式，导致如果加了border之后会产生bug，所以运动框架里应当使用getStyle函数来确保不会发生此类问题。

### 
    function getStyle(obj,attr){  
        if(obj.currentStyle){ 
                return obj.currentStyle[attr]; 
        }else{ 
                return getComputerStyle(obj,flase)[attr]; 
        } 
    }



