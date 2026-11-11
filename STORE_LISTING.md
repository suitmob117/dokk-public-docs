---
title: 商店文案
permalink: /store-listing/
---

# 商店信息与文案 · 0.8.0

更新日期：**2026 年 11 月 11 日**。可复制文案，最终以 Partner Center 字段限制为准。

## 简体中文

### 产品名称

DoKK多可学习助手

### 简短描述

AI 辅助做题助手：通过官方服务、自配 API 或本地 CLI 求解网页练习，核对后填写，不自动提交。

### 完整描述（可复制）

DoKK多可学习助手是一款面向允许使用辅助工具的学习与练习场景的 Chrome / Edge 扩展：识别网页题目，获取大模型参考答案，预览确认后受控填写。最终提交由你手动完成。

主要功能：
- 独立工作台与运行日志侧栏，支持亮色/暗色主题。
- 支持单选、多选、判断、填空、简答与编程题，兼容 Monaco、Ace、CodeMirror 等常见编辑器。
- 官方服务：兑换卡密后由授权后台按权益转交模型，适合不想自行配置 API 的用户。
- 自配 API：支持 OpenAI 兼容接口与主流模型服务商，题目直接发往你填写的地址。
- 本地 CLI：通过可选的 Windows 本地桥调用你已登录的 AI 命令行工具。
- 编程题样例自修正：运行页面样例失败时，由模型分析报错并最多修正两次。
- 页内悬浮控件：可拖动、固定与快捷键操作，减少切屏。
- 网课学习预览：有限接入超星、智慧树、中国大学 MOOC 与国家开放大学实验学院，正常播放、按明确目录换章；不伪造学时，不调用私有进度接口。
- 凭据保护：API Key 默认仅保存在浏览器会话，可选本机口令加密。

数据与边界：只有你主动读取/求解并确认数据说明后，题目才会发送至所选服务；官方服务会保留调用与计费元数据，当前版本不持久保存题目与答案正文。请阅读公开隐私政策。扩展不绕过登录、验证码或课程限制，不保证平台认定完成或取得学分。仅用于允许辅助工具的学习与练习，不得用于正式考试或其他禁止 AI 辅助的场景。

“官方服务”是本产品的模式名称，不表示与 Microsoft、课程平台或模型厂商存在官方隶属关系。

### 0.8.0 更新说明（可复制）

新增独立工作台、运行日志侧栏与明暗主题。默认使用官方服务；本地 CLI 与自配 API 需先在“卡密与授权”兑换并在线核对刷题时长卡。完善授权状态、调用记录、错误提示与页内悬浮控件。继续支持网课预览、编程题样例修正与可选本地桥。

## English

### Product name

DoKK Study Assistant

### Short description

Study assistant for permitted practice: solve web questions via Official Service, your own API, or a local CLI. You review and submit.

### Full description

DoKK is a Chrome/Edge study assistant for learning and practice where AI help is permitted. It reads the current question, requests an answer from the model service you choose, and lets you preview before filling. Final submission is always manual.

- Standalone workspace and activity side panel with light/dark themes.
- Single choice, multiple choice, true/false, fill-in-the-blank, short answer, and coding questions.
- Official Service: redeem a card and let the authorization backend route requests to a configured model.
- Custom API: OpenAI-compatible endpoints; questions go directly to the endpoint you save.
- Local CLI: optional Windows bridge to your installed and signed-in AI command-line tool.
- Coding sample repair: run the page's existing samples and let the model analyze errors (up to two repairs).
- In-page floating controls with drag, pin, and keyboard shortcut.
- Course preview for selected platforms: normal playback and chapter changes via explicit links; no fake study time and no private progress APIs.
- API keys stay in browser session storage by default, with optional on-device passphrase encryption.

Data and boundaries: practice content is sent only after you explicitly read/solve a question and accept the data-use notice. The Official Service retains call and billing metadata; question and answer bodies are not persistently stored by the service in the current version. The extension does not bypass logins, CAPTCHAs, or course restrictions, and does not guarantee platform completion or credits. Use only where AI assistance is permitted, never in formal exams. "Official Service" is a product mode name and does not imply affiliation with Microsoft, course platforms, or model vendors.

### Update notes (0.8.0)

Added a standalone workspace, activity side panel, and light/dark themes. Official Service is the default; Custom API and Local CLI require a practice-time card redeemed under License. Improved entitlement status, call records, error messages, and in-page controls. Course preview, coding sample repair, and the optional local bridge remain available.

## 建议元信息

- 类别：生产力 / 教育（以控制台提供选项为准）
- 搜索关键词：DoKK, 多可学习助手, DoKK-Solve, 做题助手, 学习, 练习, AI, 编程, study assistant
- 官网：<https://suitmob117.github.io/dokk-public-docs/>
- 隐私：<https://suitmob117.github.io/dokk-public-docs/privacy/>
- 支持：<https://suitmob117.github.io/dokk-public-docs/support/>
- 使用条款：<https://suitmob117.github.io/dokk-public-docs/terms/>

> 包内 `manifest.description` 为“AI 练习与网课学习助手：支持本地 CLI/API、课程识别、正常播放与随堂练习预览填写，不自动提交。”。商店短描述可使用上方文案，但不要声称已修改清单字段，除非实际打包中已同步。
