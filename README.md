# plain-explainer

Claude Skill：把任何概念讲到零基础小白也能懂。

提问"什么是 XX"时，用「一句话概括 → 生活类比 → 场景展开 → 留进阶入口」的结构回答，术语当场翻译，全文只用一个类比，杜绝伪通俗和居高临下。

## 安装

```bash
git clone https://github.com/你的用户名/plain-explainer.git ~/.claude/skills/plain-explainer
```

或手动：新建 `~/.claude/skills/plain-explainer/` 目录，把本仓库的 `SKILL.md` 放进去。

## 使用

在问题前加 `/plain-explainer` 显式调用（**推荐，所有客户端通用**）：

- `/plain-explainer 什么是 API`
- `/plain-explainer RAG 和微调的区别`

在部分客户端（如 Claude Code）中，直接问"什么是 XX"也可能自动触发，但不保证——实测为准。

## 效果对比

**不用 skill 时**（典型回答风格）：
> API（Application Programming Interface）是应用程序编程接口，定义了软件组件之间的交互规范，通过请求-响应模式实现系统间通信……

**用 skill 后**：
> 一句话：API 就是"程序专用的服务窗口"——你的代码通过这个窗口，让别的软件替你干活。
> 它就像食堂的送餐专线：你自己去食堂打饭要排队刷卡，打专线电话报菜名，后厨照做送到桌上。专线那头还是同一个食堂，只是对接方式从"你这个人"变成了"电话"……

## 实测反馈

- ✅ 结构符合预期：一句话概括 → 类比 → 场景 → 进阶入口
- ✅ 术语当场翻译，类比前后统一
- ⚠️ 自动触发取决于客户端：Kimi 等环境需手动 `/plain-explainer` 调用

## 许可证

MIT
