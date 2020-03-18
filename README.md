# Flexible-Jekyll is a simple and clean theme for Jekyll  

[Jekyll模板主页](https://github.com/artemsheludko/flexible-jekyll)
---

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

