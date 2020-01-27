# 武汉新型冠状病毒防疫信息收集平台-地图可视化项目

本项目负责平台的信息展示，可视化地理信息。
主要目的是做一个相对通用的地图组件给前端，不光是疫情信息，也尽量可以展示医院需求、物流工厂、酒店等的地理信息，尽可能做到精细化展示和地理信息的范围查询能力。

## 技术栈

-   可视化库: [ECharts v4][13] (自带百度地图插件，可以支持我们对地图可视化的需求)
-   逻辑语言: [TypeScript v3][5]
-   组件引擎: [WebCell v2][6]
-   组件库: [BootCell v1][7]
-   状态管理: [MobX v5][8]
-   PWA 框架: [Workbox v4][9]
-   打包工具: [Parcel v1][10]
-   CI / CD: [Travis CI][11] + [GitHub Pages][12]

## 讨论
欢迎大家加入[Slack 交流群组](https://join.slack.com/t/wuhan2020/shared_invite/enQtOTIzNjA2MDYwOTUxLWVjMjA4MjdhNGVmZmZlZTgxYjM1ZDY1NGVkZDVkNGI0NzhjZGVlYTM2Mjc5Mjk2YjgyYTk1NDJmNTkxODZlOTE)，我们在 `#map-visualization` channel.
slack群组也另有channel分别负责前端、后端、数据录入等不同方面，有兴趣参与讨论其他问题的童鞋也热烈欢迎加入！

## 本地开发

### 配置
1. [安装 Node.js](https://nodejs.org/en/download/package-manager/)
2. 
```sh
# clone the repo
git clone git@github.com:wuhan2020/map-viz.git
# setup the npm env
cd map-viz
npm install
# start the project
npm start
```

### 教程及有用链接

[5 分钟上手 ECharts](https://www.echartsjs.com/zh/tutorial.html#5%20%E5%88%86%E9%92%9F%E4%B8%8A%E6%89%8B%20ECharts)

[echarts example](https://gallery.echartsjs.com/explore.html#sort=rank~timeframe=all~author=all)


#### 例子

[百度迁徙](https://qianxi.baidu.com/?from=shoubai#city=420100)

[百度实时疫情数据](https://voice.baidu.com/act/newpneumonia/newpneumonia)

[丁香园实时疫情数据](https://3g.dxy.cn/newh5/view/pneumonia)

[qq实时疫情数据](https://news.qq.com/zt2020/page/feiyan.htm)

[财新实时+历史数据](http://datanews.caixin.com/2020-01-20/101506236.html)

#### 临时接口

[疫情省市历史数据](http://ncov.nosensor.com:8080/api/)

[百度实时疫情](https://service-nxxl1y2s-1252957949.gz.apigw.tencentcs.com/release/newpneumonia)

[百度迁徙](https://service-8o85sm22-1252957949.gz.apigw.tencentcs.com/release/qianxi) 

+ [city_rank](https://service-8o85sm22-1252957949.gz.apigw.tencentcs.com/release/qianxi?action=city_rank?date=20200125&id=420100&type=move_out)

+ [history_curve](https://service-8o85sm22-1252957949.gz.apigw.tencentcs.com/release/qianxi?action=history_curve&id=420100&endDate=20200125)


[丁香园实时疫情](https://service-0gg71fu4-1252957949.gz.apigw.tencentcs.com/release/dingxiangyuan)

[qq实时+历史疫情](https://service-n9zsbooc-1252957949.gz.apigw.tencentcs.com/release/qq )

[财新实时+历史数据](https://service-qjf6zmby-1252957949.gz.apigw.tencentcs.com/release/caixin)

+  [json](https://service-qjf6zmby-1252957949.gz.apigw.tencentcs.com/release/caixin)
+  [csv](https://service-qjf6zmby-1252957949.gz.apigw.tencentcs.com/release/caixin?action=csv)
+  [pneumonia](https://service-qjf6zmby-1252957949.gz.apigw.tencentcs.com/release/caixin?action=pneumonia)
+  [total](https://service-qjf6zmby-1252957949.gz.apigw.tencentcs.com/release/caixin?action=total)
+  [data2](https://service-qjf6zmby-1252957949.gz.apigw.tencentcs.com/release/caixin?action=data2)



[1]: https://developers.google.cn/web/progressive-web-apps
[2]: https://david-dm.org/wuhan2020/wuhan2020.github.io
[3]: https://travis-ci.com/wuhan2020/wuhan2020.github.io
[4]: https://www.w3.org/
[5]: https://typescriptlang.org
[6]: https://web-cell.dev/
[7]: https://web-cell.dev/BootCell/
[8]: https://mobx.js.org
[9]: https://developers.google.com/web/tools/workbox
[10]: https://parceljs.org
[11]: https://travis-ci.com/
[12]: https://pages.github.com/
[13]: https://www.echartsjs.com/
