# Cloudflare IP 在线测试工具

## 原有功能

1. HTTP(s)响应时间测试
2. 平均下载速度测试（使用不同大小的文件测试）
3. 进行批量测试。
4. 显示每个任播 IP 的实际位置（根据 /cdn-cgi/trace判断）
5. 针对每个IP中的多个测试进行简单的统计分析
6. 适配移动设备（目前仅测试过安卓系统）
7. 导出测试结果

##  改进功能

1. 添加随机生成ip数量
2. 添加停止测试功能
3. 汉化语言。

##  如何部署

1.  启用Github Cloudflare IP 测试项目设置的Pages功能，分支选择master下/root文件夹.
2.  Cname解析自己域名到github，不开启Enforce HTTPS （非常重要），开启后将不能进行测试，这也是该项目巧妙之处。
3.  关闭Cloudflare中所有强制验证SSL证书的功能， cloudflare Workers
4.  访问该项目网页时，一定是'http://'开头，如果浏览器提示不安全，忽视即可。



## 🙏 致谢

本项目基于 [TulvL/cloudflare-ip-tester](https://github.com/TulvL/cloudflare-ip-tester) 做了些改进，感谢原作者TulvL的贡献。

