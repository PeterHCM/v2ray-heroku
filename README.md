# V2Ray Heroku (English by Google Translate)

**To deploy V2Ray VLESS, go to the [vless](https://github.com/bclswl0827/v2ray-heroku/tree/vless) branch. **

## Overview

This project is used to deploy V2Ray WebSocket on Heroku. To the extent of reasonable use, this image will not be banned due to a large amount of resources.

Once deployed, V2Ray will always run with the latest version every time the app is launched

## deploy

### steps

 1. Fork this project to your own GitHub account (username is `example`)
 2. Modify the project name, be careful not to include the keywords `v2ray` and `heroku` (the modified project name takes `demo` as an example)
 3. Modify `README.md` and replace `bclswl0827/v2ray-heroku` with your own content (such as `example/demo`)

> [![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https://github.com/PeterHCM/v2ray-heroku)
 4. Go back to the project homepage and click the link above to deploy V2Ray

### variables

The variable names that need to be set during deployment are explained as follows.

| variable | default value | description |
| :--- | :--- | :--- |
| `ID` | `ad806487-2d26-4636-98b6-ab85cc8521f7` | VMess user master ID, used for authentication, in UUID format |
| `WSPATH` | `/` | HTTP protocol path used by WebSocket |

## Access to CloudFlare

The following two methods can connect the application to CloudFlare, which can improve the speed to a certain extent.

 1. Bind a domain name to the application and connect the domain name to CloudFlare
 2. Reverse proxy through CloudFlare Workers

## Notice

 1. **Do not abuse this project, there are very few free services like Heroku, and use and cherish**
 2. If using a domain name to access CloudFlare, please consider enabling TLS 1.3
 3. Most of AWS IPv4 addresses are blocked by Twitter


# V2Ray Heroku

**若需部署 V2Ray VLESS，请转到 [vless](https://github.com/bclswl0827/v2ray-heroku/tree/vless) 分支。**

## 概述

本专案用于在 Heroku 上部署 V2Ray WebSocket，在合理使用的程度下，本镜像不会因为大量占用资源而导致封号。

部署完成后，每次启动应用时，运行的 V2Ray 将始终为最新版本

## 部署

### 步骤

 1. Fork 本专案到自己的 GitHub 账户（用户名以 `example` 为例）
 2. 修改专案名称，注意不要包含 `v2ray` 和 `heroku` 两个关键字（修改后的专案名以 `demo` 为例）
 3. 修改 `README.md`，将 `bclswl0827/v2ray-heroku` 替换为自己的内容（如 `example/demo`）

> [![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https://github.com/PeterHCM/v2ray-heroku)

 4. 回到专案首页，点击上面的链接以部署 V2Ray

### 变量

对部署时需设定的变量名称做如下说明。

| 变量 | 默认值 | 说明 |
| :--- | :--- | :--- |
| `ID` | `ad806487-2d26-4636-98b6-ab85cc8521f7` | VMess 用户主 ID，用于身份验证，为 UUID 格式 |
| `WSPATH` | `/` | WebSocket 所使用的 HTTP 协议路径 |

## 接入 CloudFlare

以下两种方式均可以将应用接入 CloudFlare，从而在一定程度上提升速度。

 1. 为应用绑定域名，并将该域名接入 CloudFlare
 2. 通过 CloudFlare Workers 反向代理

## 注意

 1. **请勿滥用本专案，类似 Heroku 的免费服务少之又少，且用且珍惜**
 2. 若使用域名接入 CloudFlare，请考虑启用 TLS 1.3
 3. AWS 绝大部分 IPv4 地址已被 Twitter 屏蔽
