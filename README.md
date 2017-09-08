# 程序员的算法趣题  
javascript详解

##[Q06考拉兹猜想](https://github.com/zxy7/algorithm/blob/master/Q06.html)
![](/img/Q06.png)

```javascript
    var arr=[];
    var i=2;
    for(;i<10000;){
        var s=3*i+1;
        while( s!=1){ 
            s=s%2==0?s/2:s*3+1; 
            if(s==i){arr.push(s);}
        }
        i+=2;
    }
    alert(arr.length)
```