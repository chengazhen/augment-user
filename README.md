# Augment User 自动注册工具

这是一个用于自动化完成 AugmentCode 平台注册流程的工具。

## 新版（可用）
[文档](https://codercheng.notion.site/augment)

## 必备条件
你首先要有一个cloudflare的域名邮箱，玩过 cursor auto free的肯定都知道。
然后执行 augment-magic.exe 清理机器码。然后在继续执行 augment_auto.user.js 脚本。

## 项目描述

本工具是一个基于 Tampermonkey 的用户脚本，能够自动化完成 AugmentCode 平台的注册过程。它提供了一个友好的用户界面来显示注册进度，并能够自动处理邮箱验证等复杂流程。

## 主要功能

- 自动生成随机用户信息
- 临时邮箱集成
- 自动获取和填写验证码
- 实时进度显示
- 错误自动重试机制
- 可视化日志界面

## 系统要求

- 浏览器安装 Tampermonkey 插件
- 支持的浏览器：Chrome, Firefox, Edge 等主流浏览器
- 网络连接（用于访问临时邮箱服务）

## 安装说明

1. 安装 Tampermonkey 浏览器插件
2. 下载 `augment_auto.user.js` 脚本文件
3. 将脚本导入到 Tampermonkey 中
4. 访问 AugmentCode 网站，工具会自动启动

## 关注公众号

为了获取最新的工具更新和使用教程：

1. 请关注微信公众号：code 未来
2. 获取更多技术分享和使用技巧
3. 实时了解工具的最新动态和更新

## 使用说明

1. 访问 AugmentCode 的注册页面
2. 工具会在右下角显示操作日志界面
3. 点击"开始注册"按钮启动自动注册流程
4. 等待工具自动完成注册过程

## 配置说明

脚本中包含以下可配置项：

```javascript
const EMAIL_DOMAIN = "@hex.cloudns.be";
const TEMP_MAIL_CONFIG = {
    username: "xxxx",
    emailExtension: "@mailto.plus",
    epin: ""
};
```

## 安全说明

- 本工具仅用于学习和测试目的
- 请遵守目标网站的使用条款
- 不建议频繁使用以避免对服务器造成压力

## 故障排除

如果遇到问题，请检查：

1. Tampermonkey 插件是否正确安装
2. 脚本是否正确导入
3. 网络连接是否正常
4. 临时邮箱服务是否可用

## 贡献指南

如果您想为项目做出贡献，欢迎：

- 提交 bug 报告
- 提供功能改进建议
- 优化代码实现
- 完善项目文档

## 许可说明

本项目仅供学习和研究使用，请勿用于商业目的。使用本工具时请遵守相关网站的使用条款和规定。
