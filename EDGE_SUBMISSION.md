---
title: Edge 上架信息
permalink: /edge-submission/
---

# Microsoft Edge Add-ons 公开信息与填写清单

对应扩展：**DoKK多可学习助手 0.8.0**。更新日期：**2026 年 11 月 11 日**。截图版本见[商店图片]({{ '/store-assets/' | relative_url }})。

## 可填写的公开链接

| Partner Center 信息 | 内容 |
| --- | --- |
| 产品名称 | DoKK多可学习助手 |
| 产品网站 / Website | <https://suitmob117.github.io/dokk-public-docs/> |
| 隐私政策 / Privacy policy | <https://suitmob117.github.io/dokk-public-docs/privacy/> |
| 支持 / Support | <https://suitmob117.github.io/dokk-public-docs/support/> |
| 使用条款 / Terms | <https://suitmob117.github.io/dokk-public-docs/terms/> |
| 权限说明 | <https://suitmob117.github.io/dokk-public-docs/permissions/> |
| 操作指南 | <https://suitmob117.github.io/dokk-public-docs/guide/> |
| 版本说明 | <https://suitmob117.github.io/dokk-public-docs/changelog/> |
| 公开反馈 | <https://github.com/suitmob117/dokk-public-docs/issues> |
| 产品图标（128×128 PNG） | [assets/icons/icon-128.png]({{ '/assets/icons/icon-128.png' | relative_url }}) |

以上页面均可匿名访问，无需登录。隐私政策包含数据类型、处理目的、共享对象、存储与保留、用户控制、未成年人、更新与联系方式，并附 Microsoft Edge 数据披露摘要与英文摘要。

> 如果商店旧条目填写的是其他隐私政策地址（例如临时文档托管），请在更新提交时改为上面的 GitHub Pages 地址，确保与实际包和审核材料一致。

## 商店文案（简体中文）

**简短描述**

AI 辅助做题助手：通过官方服务、自配 API 或本地 CLI 求解网页练习，核对后填写，不自动提交。

**完整描述**

DoKK多可学习助手是一款面向允许使用辅助工具的学习与练习场景的 Chrome / Edge 扩展：识别网页题目，获取大模型参考答案，预览确认后受控填写。最终提交由你手动完成。

主要功能：
- 独立工作台与运行日志侧栏，支持亮色/暗色主题。
- 支持单选、多选、判断、填空、简答与编程题，兼容常见代码编辑器。
- 官方服务：兑换卡密后由授权后台按权益转交模型，适合不想自行配置 API 的用户。
- 自配 API：支持 OpenAI 兼容接口与主流模型服务商，题目直接发往你填写的地址。
- 本地 CLI：通过可选的 Windows 本地桥调用你已登录的 AI 命令行工具，无需在扩展中保存模型 Key。
- 编程题样例自修正：运行页面样例失败时，可由模型分析报错并最多修正两次。
- 页内悬浮控件：可拖动、固定与快捷键操作，减少切屏。
- 网课学习预览：有限接入超星、智慧树、中国大学 MOOC 与国家开放大学实验学院，正常播放、按明确目录换章；不伪造学时，不调用私有进度接口。
- 凭据保护：API Key 默认仅保存在浏览器会话，可选本机口令加密。

数据与边界：只有你主动读取/求解并确认数据说明后，题目才会发送至所选服务；官方服务会保留调用与计费元数据，当前版本不持久保存题目与答案正文。请阅读公开隐私政策。扩展不绕过登录、验证码或课程限制，不保证平台认定完成或取得学分。仅用于允许辅助工具的学习与练习，**不得用于正式考试或其他禁止 AI 辅助的场景**。

“官方服务”是本产品的模式名称，不表示与 Microsoft、课程平台或模型厂商存在官方隶属关系。

## 英文商店文案

**Short description**

Study assistant for permitted practice: solve web questions via Official Service, your own API, or a local CLI. You review and submit.

**Full description**

DoKK (多可学习助手) is a Chrome/Edge study assistant for learning and practice where AI help is permitted. It reads the current question, requests an answer from the model service you choose, and lets you preview before filling. Final submission is always manual.

Key features:
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

## 权限用途（审核用）

| 权限 | 单一用途说明 |
| --- | --- |
| `activeTab` | 用户点击后访问当前标签页，读取当前练习题目 |
| `scripting` | 在已授权页面注入包内识题、填写与悬浮控件脚本 |
| `storage` | 本机保存设置、会话日志、授权会话与可选加密 API Key |
| `sidePanel` | 展示运行日志与状态 |
| `nativeMessaging` | 仅本地 CLI 模式与本机桥通信 |
| `webNavigation` | 感知已授权练习页 iframe 的换题与导航 |
| `offscreen` | 承载可取消的 API 请求与流式解析 |
| 四项 `host_permissions` | 预置课程站点的识别、正常播放与随堂练习 |
| `optional_host_permissions` | 按需授权练习站点、授权后台或 API 域名，不默认全网授权 |

未声明 `cookies`、`history`、`webRequest`、`debugger` 或 `management`。详细说明见[权限与数据流]({{ '/permissions/' | relative_url }})。

## 数据披露要点

- 不包含广告、遥测或第三方统计 SDK；不出售个人信息。
- 本地 CLI 与自配 API 的题目不经过授权后台转发；后台只核验刷题时长。
- 官方服务将题目发送至授权后台并转交配置的模型；保留调用/计费元数据（IP、UA、版本、来源、模型、状态、Token、金额、耗时等），不持久保存题目与答案正文。
- 练习日志仅本机会话保存（60 条），课程日志 50 条；反馈报告需用户手动发送。
- 不收集精确位置、浏览历史、健康信息、通讯内容或支付账户信息。
- 用户可停止任务、清除记录、撤回同意、移除站点权限、退出授权或卸载。

## 审核测试步骤（无需真实生产凭证）

1. 在 Edge 中安装扩展，点击工具栏图标打开运行日志侧栏，再点击“打开完整工作台”。
2. 首次进入练习时会展示“数据使用说明”，可查看说明、操作手册与隐私政策。
3. 只验证界面与权限：打开一个包含练习题目的公开测试页面，在工作台选择该页面，检查扩展是否在用户授权后才读取题目结构。
4. **API 模式**：在“设置中心 → 模型连接”选择 API 模式，填入审核方自己的 OpenAI 兼容测试地址、Key 与模型名，点击“测试连接”（只发送固定算术题），保存后读取并“仅预览答案”。不需要真实生产 Key。
5. **本地 CLI 模式**（可选）：跳过不影响 API 模式测试。若需验证，安装扩展附带的本地桥并选择已登录的 CLI；未安装时扩展会明确提示。
6. 核对扩展不会自动提交试卷或代码；所有填写操作都需要用户点击，最终提交由用户完成。
7. 卡密与官方服务如需验证，请使用审核方自建测试后台签发的专用测试卡。公开仓库不提供卡密、密钥或账号。

## 提交前清单

- [ ] 上传的 ZIP 根目录直接包含 `manifest.json`，版本与商店文案一致。
- [ ] 隐私政策 URL 已在未登录浏览器中打开验证，与实际数据行为一致。
- [ ] 权限说明、支持链接与使用条款均可访问。
- [ ] 截图、图标与描述使用当前版本界面；演示数据已标注。
- [ ] 在 Partner Center 私密备注中提供测试步骤与专用测试凭证（如需要）。
- [ ] 不把生产卡密、API Key、账号或审核凭证放入公开仓库。
- [ ] 更新现有商店条目时保留原扩展 ID，不因普通更新重建条目。

公开仓库不包含插件 ZIP、后台源码、题库或审核凭证。建立公开文档不代表已上传商店、完成审核或获得平台认证。字段与政策以提交时的 Partner Center 为准。

官方参考：[发布扩展](https://learn.microsoft.com/en-us/microsoft-edge/extensions/publish/publish-extension)、[Microsoft Edge 扩展开发者政策](https://learn.microsoft.com/en-us/legal/microsoft-edge/extensions/developer-policies)。
