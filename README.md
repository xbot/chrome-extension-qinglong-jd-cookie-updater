# 青龙面板京东 Cookie 同步助手

一个简单实用的 Chrome 扩展程序，用于自动同步京东 Cookie 到青龙面板，解决 Cookie 失效问题。

## 主要功能

- 自动获取京东 Cookie（pt_key 和 pt_pin）
- 支持自动同步到青龙面板指定的环境变量
- 可配置同步时间间隔
- 支持手动立即同步
- 可视化操作界面
- 状态指示和同步记录

## 安装说明

1. 下载本仓库代码并解压
2. 打开 Chrome 浏览器，进入扩展程序页面（chrome://extensions/）
3. 开启右上角的"开发者模式"
4. 点击"加载已解压的扩展程序"，选择解压后的文件夹

## 使用方法

### 基础配置

1. 点击浏览器工具栏中的扩展图标，打开配置面板
2. 填写以下必要信息：
   - 青龙面板地址：您的青龙面板访问地址（例如：http://localhost:5700）
   - Client ID：青龙面板应用 ID
   - Client Secret：青龙面板应用密钥
   - 环境变量名称：用于保存Cookie的变量名（例如：JD_COOKIE）

### 获取青龙面板 Client ID 和 Secret

1. 登录青龙面板
2. 进入"系统设置" -> "应用设置"
3. 点击"添加应用"，填写名称并保存
4. 记录生成的 Client ID 和 Client Secret

### 自动同步设置

1. 在配置面板中启用"自动同步"
2. 设置同步时间间隔（默认为60分钟）
3. 点击"保存配置"按钮

### 手动同步

- 点击配置面板中的"立即同步"按钮即可手动触发同步

## 注意事项

- 首次使用时需要确保已登录京东（https://bean.m.jd.com/bean/signIndex.action）
- 如果同步失败，扩展会自动打开京东登录页面
- 请确保青龙面板地址可正常访问
- 建议将同步间隔设置在合理范围内，避免频繁同步
- 同步状态可通过扩展图标角标显示（✓表示成功，!表示失败）

## 隐私说明

- 本扩展仅获取必要的 Cookie 信息（pt_key 和 pt_pin）
- 所有配置信息均存储在本地，不会上传到任何服务器
- Cookie 仅会同步到配置的青龙面板地址

## 技术支持

如有问题或建议，请通过以下方式反馈：
1. 在 GitHub 上提交 Issue
2. 在 GitHub Discussions 中发起讨论

## 开源协议

本项目采用 MIT 协议开源，欢迎贡献代码。
