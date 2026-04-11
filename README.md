# multi-agents-vareity-show

**🔥 AI 多智能体抽象大舞台 | 持续更新 100+ 抽象 Skill | 赛博对线神器 | 人设模拟器 | 整活乐园**


![License](https://img.shields.io/badge/License-Apache_2.0-blue)
![AgentSkills](https://img.shields.io/badge/Agent-Skills-green.svg)
![DummySkills](https://img.shields.io/badge/Dummy-Skills-yellow)

## 📦 这仓库是啥？
> 这是一个AI 角色技能库 + 多智能体整活平台
把网络热门人设、经典对话风格，全部做成可直接调用的独立 Skill

不局限于抽象，持续更新升学留学逻辑、书籍思想方法等

* 🌱 持续更新：目标 100+ 抽象 Skill
* 🧩 即插即用，每个 Skill 独立文件夹
* 🎭 人设齐全：爹味、大妈、真狗、阴阳怪气、赛博嘴替…
* 🎓 附带实用向：升学规划、留学咨询、书籍方法论
* 🎪 可自由组合多智能体，上演各种抽象节目

## 🛠 已上线 Skill

### 🔥 抽象Skill合集

每个Skill都是一个文件夹，可以单独调用

### 爹味.Skill
> 我不要你觉得，我要我觉得。听我的，这事都听我的！我是为你好，你要感恩，我走过的路比你吃的盐都多。人生经验拉满，说教式关怀，爹味浓度超标，专门在你懈怠的时候反向激励你

### 真狗.Skill
> 在现实生活中，普通人容易上当受骗，总有一些别有用心之人，趴在地上，自称也是主人的小狗。真狗Skill -- 真正的AI电子狗，不是真正的狗我不养

#### 效果示例
```bash
用户       > /real-dog
真狗.skill > 汪汪！汪呜🐕
            (请告诉我你的小狗品种和名字)
            (请告诉我小狗的性格)
```

```bash
用户       > 黑柴犬 bambi 快乐但有点倔
真狗.skill > 汪汪汪！！！汪~
            (bambi收到)
            汪呜汪呜~
            (疯狂摇尾巴中...)
```

```bash
用户       > 我说往东走，你往哪里
真狗.skill > 汪！(坚定)
            (bambi倔强的往西边去了)
```

### 真老板.Skill
> 不是AI，不是助手，是一个有KPI要追、有项目要推、有饼要画的真老板。只会说老板黑话，绝对不会说正常人话，要业绩！要进度！要结果！要加班！要省钱！

**不断更新中......**

## 🎪 怎么玩？
### Claude Code

> Claude Code 从 **git 仓库根目录** 的 `/user/path/to/.claude/skills/` 查找 skill。请在正确的位置执行。

```bash
# 进入用户目录，最好是一个空目录
cd /user/path/
# 新觉claude根目录
mkdir -p .claude
# 拉取代码
git clone https://github.com/SkillForge88/multi-skills-show.git
cp -r multi-skills-show/* /user/path/.claude/
cd /user/path/.claude/
# 执行claude code
claude
```

1. 在Claude code中输入
```bash
你好
```
随后，claude会返回所有的角色列表：如
| 角色  |  说明                          |
|-------|-------------------------------|
|/boss  | 真正的老板来了，不画大饼我不舒服 |
|/等等  | 等等 |

2. 输入
```bash
/boss
```
则进入角色对话

## 📢 免责声明
本项目仅为**娱乐整活、二创创作**使用，所有 Skill 均为网络风格化模拟，无恶意指向、不代表任何人真实立场，无任何商业用途。
如有侵权 / 不适，联系即删。