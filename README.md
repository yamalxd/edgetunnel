https://blog.mareep.net/posts/10934/

点击workers和pages

创建worker


修改名称（随意）点击部署，再编辑代码


打开项目的.js文件 /src/worker-vless.js 全选复制里面的代码，粘贴到workers中


修改 UUID 和 proxyIP，UUID 可选择在线生成 https://1024tools.com/uuid 复制粘贴，这里提供一个IP let proxyIP = ‘103.200.112.108’; 同样复制粘贴，最后点击保存并部署，那这个ip的作用是啥呢
这是一些神奇的ip，可以无条件的转发所有cf流量，大致来说就是此方法搭建的节点是无法访问托管在cloudflare平台上的网站的，所以需要有一个中间人去转发流量访问这些网站
如果上面的proxyip用不了了，可以替换成下面这些域名

cdn-all.xn--b6gac.eu.org 
cdn.xn--b6gac.eu.org 
cdn-b100.xn--b6gac.eu.org 
edgetunnel.anycast.eu.org 
cdn.anycast.eu.org
另外可以参考这个issues进行proxyip查找
issues：https://github.com/zizifn/edgetunnel/issues/162


方式一：自己有域名（可选）
添加域名

添加完成之后，可能要等几分钟等待域名生效

查看vless并导入链接
输入你的域名+uuid（例如：test.pornhug.top/d342d11e-d424-4583-b36e-524ab1f0afa4）

导入通用格式就行了

优选ip
因为cloudflare在国内访问速度很慢，所以需要优选ip
将服务器地址换成优选ip即可
https://stock.hostmonit.com/CloudFlareYes
