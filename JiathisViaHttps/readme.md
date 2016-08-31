https://github.com/airbai/JiathisViaHttps.git


在 HTTPS 站点使用 jiathis

三步搞定：
需要一个 https 的反向代理，懒得建的话，可以直接用我的：
https://tomoat.github.io/JiathisViaHttps/jia.js。
在全局配置变量中，设置do_not_track: true。可以干掉发往 id.jiathis.com 域的请求。
var jiathis_config={
    summary:"",
    shortUrl:false,
    hideMore:false,
    do_not_track: true // 干掉发往 id.jiathis.com 域的请求
}
禁用分享计数器，把类名包含jiathis_counter_style的 HTML 元素删掉即可。可以干掉发往 i.jiathis.com 域的请求。

