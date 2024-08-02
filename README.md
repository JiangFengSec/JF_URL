JF_URL是一款URL深度采集工具
# 🔖脚本语言
python 3.6.8
# 🌲为何写它
URL采集能帮我们快速的采集符合需求的URL，市面上大部分的URL采集工具都是利用多个搜索引擎接口进行采集，基于黑名单过滤部分网址，最后再对结果去重。看上去没错，但却隐藏着几个缺点：

1. 采集的网址都是被搜索引擎收录的，导致许多符合需求的URL无法采集到
2. 过滤不细致，往往只设置了黑名单+去重，采集到的站点并不能保证是需要的
3. 采集URL的关键词差不多，导致采集结果也差不多，意味着你好不容易找到一个漏洞站点可能已被许多人利用过
# 🎉脚本功能

1. 采用多线程技术，显著提高运行效率
2. 提供两个入口，搜索引擎接口或导入采集好的网址
3. 传入关键字爬取到符合需求网址再次自动进行友链爬行
4. URL自动存活探测，筛选出的URL是符合条件且存活的
5. 导入的URL文本筛选出符合条件的URL，不进行友链爬行
6. 导入的URL文本筛选出符合条件的URL，再进行友链爬行
7. 用户高度自定义：URL黑白名单、URL网站标题黑白名单，URL网页内容黑白名单
# 📜免责声明
JF_URL仅能在取得足够合法授权中使用，在使用本工具过程中，您应确保自己所有行为符合当地的法律法规。 如您在使用本工具的过程中存在任何非法行为，您将自行承担所有后果，本工具作者不承担任何法律及连带责任。 除非您已充分阅读、完全理解并接受本协议所有条款，否则，请您不要安装并使用本工具。 您的使用行为或者您以其他任何明示或者默示方式表示接受本协议的，即视为您已阅读并同意本协议的约束。
# 🚀使用说明
配置文件config.ini说明：

- None不检测该关键词，目前只支持或逻辑，即符号|
- **不检测可用None，字段不可放空，否则脚本无法正常运行**
- state只支持0/1，0关闭导入文本的友链爬行，1开启导入文本的友链爬行
- 关键字优先级：网址黑 > 网址白 > 标题黑 > 标题白 > 网页内容黑 > 网页内容白

演示：
**注：爬取结束后结果以txt格式保存在当前目录下**
1、通过搜索引擎接口进行爬取教育类站点
![image.png](https://cdn.nlark.com/yuque/0/2024/png/29120375/1722565061627-5737571c-a786-4ac0-976b-e77fc7918b88.png#averageHue=%23b1e1ab&clientId=u8b8ece95-dc14-4&from=paste&height=840&id=uc7850fe4&originHeight=1679&originWidth=2861&originalType=binary&ratio=2&rotation=0&showTitle=false&size=997120&status=done&style=none&taskId=u3c182187-de31-4b9b-8b47-e848e2c81c0&title=&width=1430.5)
2、通过导入的文本先筛选出教育类站点，不进行友链爬
![image.png](https://cdn.nlark.com/yuque/0/2024/png/29120375/1722565646966-e1d2d364-312b-44e8-bfe3-e97f4a4ac20d.png#averageHue=%233d3c38&clientId=u8b8ece95-dc14-4&from=paste&height=846&id=u46101d50&originHeight=1691&originWidth=2875&originalType=binary&ratio=2&rotation=0&showTitle=false&size=1356624&status=done&style=none&taskId=ue2458ab6-ce83-4fa1-a838-81b191fe58e&title=&width=1437.5)
3、通过导入的文本先筛选出教育类站点，再进行友链爬取
![image.png](https://cdn.nlark.com/yuque/0/2024/png/29120375/1722565752255-af4c12f8-5f94-4d01-9ad9-d1078116e7e0.png#averageHue=%23353330&clientId=u8b8ece95-dc14-4&from=paste&height=841&id=uf9922c4d&originHeight=1681&originWidth=2879&originalType=binary&ratio=2&rotation=0&showTitle=false&size=1288442&status=done&style=none&taskId=u5cc1862e-2768-4b6e-8a6c-38671cfb096&title=&width=1439.5)

更多玩法等你自行研究。。。

# ⌛后续计划

1. 自定义线程数
2. 自定义代理地址
3. 听从其它意见或建议
# ☕感谢赞赏
如果你觉得这个项目帮助到了你，打赏一杯咖啡以资鼓励
![9617fd071f286fc18c67d30e8a15a4d.jpg](https://cdn.nlark.com/yuque/0/2024/jpeg/29120375/1722504244713-2c69c0b6-af54-44e9-b12d-c11d6d345b2a.jpeg#averageHue=%235d5643&clientId=ud74fc903-ff75-4&from=paste&height=576&id=u2d7545c8&originHeight=1152&originWidth=1152&originalType=binary&ratio=2&rotation=0&showTitle=false&size=119807&status=done&style=none&taskId=u128137aa-5ae5-4f28-972b-53f21412248&title=&width=576)



