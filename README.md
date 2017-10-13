# PreLoad

## 用法

实例化插件对象:

插件名：`preload`;

参数：图片(数组或者`String`类型)，方法;

方法：目前插件中提供`each`和`all`方法;

* `each` 每一张图片加载完成之后执
* `all`  所有图片加载完毕后执行


实例化对象：

```
$.preload(imgs,{
    each:function(count){
        //...一张图片加载完后做处理
    },
    all:function(){
        //...所有图片加载完毕之后做处理
    }
});
```


## 目录结构描述

目录大体结构如下，两部分可分离：

preload

>第一部分
>>test   (测试，分别用jQuery和js实现预加载)

>>>images

>>>css

>>>js

>>index.jquery.html  (测试jQuery实现)

>>index.html    (测试js实现)
***
>第二部分
>>css    

>>images   

>>js  (包含初步完成的预加载jQuery插件)

>index.jquery.html (测试jQuery插件)

>READEME.md


## 图片预加载介绍

>从字面上来看：预，就是预先；预加载：即预先提前加载。
>
>图片预先加载到浏览器中，访问者可以顺利的网站上浏览冲浪，并享受极快的加载速度；

我们为什么需要预加载？

某些情况下丰富的图片资源，带来更好的用户体验的同时，也降低的我们的性能，有时候，我们在观看页面时需要不断的等待页面加载图片，带来的极差的用户体验(这种表现在画廊，有大量照片、图片占据比例大的地方尤为明显)；






