# Flexible-Jekyll is a simple and clean theme for Jekyll  


---

# Function
[Valine](https://valine.js.org/quickstart.html)：博客阅读量统计与免登陆评论
[flexible-jekyll](https://github.com/artemsheludko/flexible-jekyll)：使用的Jekyll模板

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

## License

GNU General Public License v3.0

