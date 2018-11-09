# jquery.MyPages
基于Jquery的分页插件

### 使用方法
```html
<html>
    <link href="myPages.css" rel="stylesheet" type="text/css"/>
    <script src="myPages.js" type="text/javascript"></script>
    
    <script type="text/javascript">
        $(document).ready(function(){
            $("#myPages").myPages({
                pageNo:3,
                pageSize:15,
                firstPage:1,
                lastPage:10,
                url: "/list/{pageNo}-{pageSize}",
            })
        })
    </script>
    
<body>
    <div id="myPages">
    </div>
</body>
</html>
```


### 参数说明
```javascript
    var defaluts = {
        url: "/{pageNo}-{pageSize}",   //页码跳转链接 {pageNo}与{pageSize}为固定占位符
        pageNo: 1,      //当前页码,同时对应链接内 {pageNo}
        pageSize: 10,   //每页显示数量,对应链接内{pageSize}
        firstPage: 1,   //首页页码
        lastPage: 1,   //最后一页页码
        preText: "&lt;",   //上一页显示的文字，默认为 <
        nextText: "&gt;",  //下一页显示的文字，默认为 >
        firstText: "«",//首页显示的文字,默认为 <<
        lastText: "»", //最后一页显示的文字,默认为 >>
        showPageButton: 6 //显示的页码数量，默认为6
    };
```
