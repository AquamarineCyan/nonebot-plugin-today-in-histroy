<div align="center">
  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
  <br>
  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
</div>

<div align="center">

# nonebot-plugin-today-in-history

_✨ 历史上的今天 ✨_


<a href="./LICENSE">
    <img src="https://img.shields.io/github/license/AquamarineCyan/nonebot-plugin-today-in-history.svg" alt="license">
</a>
<a href="https://pypi.python.org/pypi/nonebot-plugin-today-in-history">
    <img src="https://img.shields.io/pypi/v/nonebot-plugin-today-in-history.svg" alt="pypi">
</a>
<img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">

</div>

## 📖 介绍

定时向指定群&好友发送  **历史上的今天**

数据源：[历史上的今天-百度百科](https://baike.baidu.com/calendar/)

鸣谢 [bingganhe123/60s-](https://github.com/bingganhe123/60s-) ~~进行一个简单的抄~~

**推荐python`3.9+`

## 💿 安装

<details>
<summary>使用 nb-cli 安装</summary>
在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装

    nb plugin install nonebot-plugin-today-in-history

</details>

<details>
<summary>使用包管理器安装</summary>
在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令

    pip install nonebot-plugin-today-in-history


打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入

    plugins = ["nonebot_plugin_today_in_history"]

</details>



## ⚙️ 配置

在 nonebot2 项目的`.env`文件中添加以下配置

新版配置，`v0.0.9`及以上

```
# nonebot-plugin-today-in-history
history_qq_friends=[123456789,123456789] #设定要发送的QQ好友
history_qq_groups=[123456789,123456789,123456789] #设定要发送的群
history_inform_time="7 35" #设定每天发送时间，以空格间隔
```
<details>
<summary>旧版配置，`v0.0.8`及以下</summary>

```
#nonebot-plugin-today-in-history
history_qq_friends=[12345678910] #设定要发送的QQ好友
history_qq_groups=[123456789,123456789,123456789] #设定要发送的群
history_inform_time=[{"HOUR":9,"MINUTE":1}] #在输入时间的时候 不要 以0开头如{"HOUR":06,"MINUTE":08}是错误的
```
</details>



## 🎉 使用

- 发送 `历史上的今天`

    > 完全匹配 `历史上的今天`

- 定时任务，`.env`配置发送好友、群、时间

### 效果图

![img.png](img.png)
