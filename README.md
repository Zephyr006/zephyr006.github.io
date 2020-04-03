
# 组件
- Jekyll模板：[jekyll-theme-leap-day](https://github.com/pages-themes/leap-day)
- 博客阅读量统计与免登陆评论：[Valine](https://valine.js.org/quickstart.html)
- 博客全文搜索：[Simple-Jekyll-Search](https://github.com/christian-fei/Simple-Jekyll-Search)

# Additional
js获取请求用户的ip地址
```javascript
    let ipScript = Utils.create('script', 'src', '//api.ip.sb/jsonip?callback=getIP');
    let s = document.getElementsByTagName("script")[0];
    s.parentNode.insertBefore(ipScript, s);
    // 获取IP
    window.getIP = function (json) {
        alert("your ip is " + json.ip);
    }
```

