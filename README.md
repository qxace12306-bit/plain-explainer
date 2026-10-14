# plain-explainer

Claude Skill：把任何概念讲到零基础小白也能懂。

提问"什么是 XX"时，自动用「一句话概括 → 生活类比 → 场景展开 → 留进阶入口」的结构回答，术语当场翻译，全文只用一个类比，杜绝伪通俗和居高临下。

## 安装

```bash
git clone https://github.com/qxace12306-bit/plain-explainer.git ~/.claude/skills/plain-explainer

或手动：新建 ~/.claude/skills/plain-explainer/ 目录，把本仓库的 SKILL.md 放进去。

使用

无需手动调用，正常提问即可自动触发：

- "什么是 API"
- "MCP 和 CLI 的区别"
- "解释一下通货膨胀"

也可显式调用：/plain-explainer 什么是递归

效果对比

不用 skill 时（典型回答风格）：

▎ API（Application Programming Interface）是应用程序编程接口，定义了软件组件之间的交互规范，通过请求-响应模式实现系统间通信……

用 skill 后：

▎ 一句话：API 就是"程序专用的服务窗口"——你的代码通过这个窗口，让别的软件替你干活。
▎ 它就像食堂的送餐专线：你自己去食堂打饭要排队刷卡，打专线电话报菜名，后厨照做送到桌上。专线那头还是同一个食堂，只是对接方式从"你这个人"变成了"电话"……

License

MIT
