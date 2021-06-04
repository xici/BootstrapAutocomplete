# Bootstrap 自动补全插件

一个小工具，jQuery也有autocomplete插件，引入到Bootstrap的时候显得有点丑，因此写一个比较简单的工具。

+ 展示UI：基于Bootstrap列表组实现；
+ 特点：支持数据回调，方便快捷

# 效果

![img](demo.gif)

# 使用方法

## 依赖

+ 必须引入<code>jQuery</code>，基于jQuery的绑定开发；
+ 必须引入Bootstrap样式，bootstrap.css


## 调用方式：

```javascript
//可选数据列表
var datas=[];
datas.push({
    //展示名name必填，否则无法运行，其他可选
    name:'展示名'
    //其他属性，回调时会直接返回
})
$('#inputid').bootstrapAutocomplete(datas,function (respData){
    //业务操作，回调方法可选，回到数据为datas的单个数据
});
```

