# JDmate · 求职沟通助手

在 Boss 直聘的岗位页读懂当前 JD，结合**自己的简历**生成打招呼语，本地评分后推荐最好的一条，
并**填进聊天输入框——但绝不替你发送**。

单一浏览器扩展、零后端，所有数据只留在本机。这个仓库是它的**在线作品演示**。

## 在线查看

**https://junchuanshu912.github.io/jdmate/**

| 页面 | 内容 |
|---|---|
| [index.html](https://junchuanshu912.github.io/jdmate/) | 入口 |
| [demo.html](https://junchuanshu912.github.io/jdmate/demo.html) | **可交互原型** —— 右侧栏全部状态 + 配置页 6 个面板，下拉 / 输入 / 校验 / 保存反馈都能真的操作 |
| [resume.html](https://junchuanshu912.github.io/jdmate/resume.html) | 示例简历：产品从一份简历里到底读出了什么 |
| [showcase.html](https://junchuanshu912.github.io/jdmate/showcase.html) | 作品说明：产品决策、被否掉的方案、三个真实技术难点 |

## 说明

- 页面里的**简历与岗位均为虚构的演示数据**，不涉及任何真实个人信息。
- 这是**可交互原型**：没有真实的 AI 调用与网络请求，点任何按钮都不会产生费用。
- 四个页面都是自包含的单文件：无外链资源、无 CDN、无外链脚本，断网也能打开。
- **原型里没有「状态切换器」**：右侧栏的每个状态都必须由真实操作走到
  （点生成 / 重新识别 / 关站点权限 / 删简历 / 切模式 / 设置 + 返回…），
  页面底部有 12 项"点它会真的走一遍"的清单。配好 Key、导入完简历之后才该变的样子，
  用设置页里的**「保存并查看侧边栏 →」**按钮去看——那也是真的保存动作。
- 两个值得留意的细节：原型里那条「✗ Golang」的**未命中关键词**，和事实护栏点出的
  「12 条业务线」**未验证数字**，都是真的算出来的，不是写死的文案。

## 技术栈

TypeScript（strict）· Vite + CRXJS · React · Dexie(IndexedDB) · Zod · pdf.js · Vitest
单一 Manifest V3 扩展 · 零后端 · 数据不出本机
