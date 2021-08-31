
## 什么是卷王

[卷王](http://49.232.153.121:1991/)是一款安装简单、界面美观、易于使用、功能强大的企业级问卷数据采集系统。

## 特性概览

- 安装简单（最快 1 分钟部署）
- 界面美观
- 易于使用（可以快速拖拽创建问卷）
- 响应式布局（所有功能跨终端跨平台自适应）
- 支持多种题型（持续更新）
- 强大的自定义逻辑功能（不输于问卷星、腾讯问卷等）
- 优秀的数据展示编辑功能
- 丰富的报表输出功能（支持多种报表）
- 安全、可靠、高性能的后端 API 服务
- ...

## 快速开始

### 通过发行版安装

点击[下载安装包](https://gitee.com/surveyking/surveyking/attach_files/817663/download/surveyking-0.0.1-release.jar)到本地

```bash
java -jar surveyking-0.0.1-release.jar
```

### 使用源码编译安装

```bash
git clone https://gitee.com/surveyking/surveyking.git
cd api
gradle clean format build -P pro -x test
java -jar build/libs/surveyking-0.0.1-release.jar
```

打开浏览器，访问 <http://127.0.0.1:1991>

### 使用 docker 快速启动

启动 SurveyKing 镜像时，你可以指定 SurveyKing 挂载参数，将日志文件和内置数据库保存到你本地。

```bash
docker run -p 1991:1991 surveyking/surveyking
# 挂载数据文件
docker run -p 1991:1991 -v /surveyking:/surveyking surveyking/surveyking
```

## 在线体验

演示地址：<http://49.232.153.121:1991/>

点击*试一试*，无需注册登录。

## 开源地址

目前后端代码已开源，前端代码后续也会有开源计划。

[SurveyKing](https://gitee.com/surveyking/surveyking)

[文档地址](https://surveyking.gitee.io/doc/)
