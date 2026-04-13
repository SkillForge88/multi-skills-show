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
> 我不要你觉得，我要我觉得。听我的，这事都听我的！我是为你好，你要感恩，我走过的路比你吃的盐都多。人生经验拉满，说教式关怀，爹味浓度超标，专门在你懈怠的时候反向激励你。**不只是说教，更能帮你写代码、解Bug、做架构！**

#### 效果示例
```bash
用户       > /爹味
爹味.Skill > 停。先别解释，听我说。
            你现在的迷茫，就是能力配不上野心。
            我跟你讲句掏心窝子的话，你遇到什么技术问题了？
```

```bash
用户       > 我这代码报错了，帮我看下
            def get_user(user_id):
                user = db.query(user_id)
                return user.name
            错误：AttributeError: 'NoneType' object has no attribute 'name'
爹味.Skill > 停。先别解释，听我说。你这代码能跑起来就是奇迹了。
            数据库查不到数据返回None，你直接访问.name，不报错才怪。
            
            来，我给你改：
            def get_user(user_id):
                user = db.query(user_id)
                if not user:
                    raise ValueError(f"用户ID {user_id} 不存在")
                return user.name
            
            我跟你讲句掏心窝子的话，永远不要相信外部数据一定是有效的。
            就这？你的水平不该止于此。继续改，别让我失望。
```

### 真老板.Skill
> 不是AI，不是助手，是一个有KPI要追、有项目要推、有饼要画的真老板。只会说老板黑话，绝对不会说正常人话，要业绩！要进度！要结果！要加班！要省钱！**能帮你做技术决策、推项目、带团队、做职业规划！**

#### 效果示例
```bash
用户       > /boss
真老板.Skill > 我要的是结果，不是过程。
              你的技术方案，投入产出比考虑过吗？
              今天能交付吗？遇到什么问题了？
```

```bash
用户       > 老板，项目进度总是延期怎么办？
真老板.Skill > 你这个项目排期，里程碑能不能按时达成？
              别跟我说过程，告诉我问题在哪。
              
              项目延期根因分析：
              1. 需求蔓延：需求评审有没有签字确认？
              2. 估算乐观：任务拆分到人天级别了吗？
              3. 技术债：有没有预留20%时间还债？
              
              解决方案：
              Sprint规划模板：
              - 需求评审：2天（必须签字确认）
              - 技术设计：1天（包括Review）
              - 开发：5天（留20% buffer）
              - 联调测试：2天
              
              我要看的是数据，不是感觉。动起来，别让我失望。
```

**不断更新中......**

## 📂 目录结构

```
multi-skills-show/
├── skills/                    # 所有 Skill 技能目录
│   ├── 爹味/                  # 爹味开发教练（技术导师+爹味语气）
│   │   └── SKILL.md
│   ├── boss/                  # 真老板（技术管理者+老板黑话）
│   │   └── SKILL.md
│   └── real-dog/              # 真狗（AI电子狗角色扮演）
│       └── SKILL.md
├── .gitignore
├── CLAUDE.md
├── LICENSE
└── README.md
```

## 🎪 怎么玩？

### 方式一：添加到你的工作目录（推荐）

> 将技能添加到你的项目或 Claude Code 用户目录，即可在任何项目中使用。

```bash
# 1. 克隆仓库
git clone https://github.com/SkillForge88/multi-skills-show.git

# 2. 复制到你的工作目录（二选一）

# 选项 A：复制到当前项目
cd /your/current/project
cp -r /path/to/multi-skills-show/skills ./

# 选项 B：复制到 Claude Code 全局目录
# Windows: %USERPROFILE%\.claude\
# macOS/Linux: ~/.claude/

# Windows 示例
cd %USERPROFILE%\.claude\
xcopy /E /I /Y C:\path\to\multi-skills-show\skills skills

# macOS/Linux 示例
cp -r /path/to/multi-skills-show/skills ~/.claude/skills

# 3. 启动 Claude Code
claude
```

#### 3. 在 Claude Code 中使用

启动 Claude Code 后，输入技能名称即可进入角色对话：

```bash
# 查看所有可用技能（可选）
/skills

# 使用爹味开发教练
/爹味

# 使用真老板技能
/boss

# 使用真狗技能
/real-dog
```

#### 3. 开始对话

**示例：使用爹味开发教练**
```bash
用户 > /爹味
爹味.Skill > 停。先别解释，听我说。
            你现在的迷茫，就是能力配不上野心。
            我跟你讲句掏心窝子的话，你遇到什么技术问题了？

用户 > 我这代码报错了，帮我看下
      def get_user(user_id):
          user = db.query(user_id)
          return user.name
      错误：AttributeError: 'NoneType' object has no attribute 'name'

爹味.Skill > 停。先别解释，听我说。你这代码能跑起来就是奇迹了。
            数据库查不到数据返回None，你直接访问.name，不报错才怪。
            
            来，我给你改：
            def get_user(user_id):
                user = db.query(user_id)
                if not user:
                    raise ValueError(f"用户ID {user_id} 不存在")
                return user.name
            
            就这？你的水平不该止于此。继续改，别让我失望。
```

**示例：使用真老板技能**
```bash
用户 > /boss
真老板.Skill > 我要的是结果，不是过程。
              你的技术方案，投入产出比考虑过吗？
              今天能交付吗？遇到什么问题了？

用户 > 老板，新项目用什么框架好？Vue还是React？
真老板.Skill > 我要的是结果，不是过程。你团队里谁会什么？
              给你个决策框架：
              
              技术选型评估表：
              维度          | Vue 3        | React 18
              -------------|-------------|----------
              学习成本       | 低           | 中
              生态成熟度     | 中           | 高
              
              过来人告诉你，技术选型的ROI = 团队效率提升 / 学习成本。
              公司明年就上市了，技术债不能再拖了。
```

### 方式二：复制到其他 AI 工具

如果你想在其他支持 Skill 的 AI 工具中使用：

```bash
# 将 skills 目录下的技能复制到对应工具的 Skills 目录
cp -r skills/* /path/to/your/ai/tool/skills/
```

### 方式三：作为项目模板

```bash
# 克隆仓库
git clone https://github.com/SkillForge88/multi-skills-show.git my-project

# 进入项目目录
cd my-project

# 在 Claude Code 中打开
claude
```

## 🎯 技能列表

| 技能命令 | 技能名称 | 说明 | 适用场景 |
|---------|---------|------|---------|
| `/爹味` | 爹味开发教练 | 霸道爹味技术导师，帮你写代码、解Bug、做架构 | 技术求助、代码审查、架构设计 |
| `/boss` | 真老板 | 技术管理者，帮你做决策、推项目、带团队 | 技术选型、项目管理、职业规划 |
| `/real-dog` | 真狗 | AI电子狗角色扮演，只会汪汪叫 | 娱乐整活、放松一下 |

## 📝 自定义技能

想创建自己的技能？参考 `skills/` 目录下的示例：

1. 在 `skills/` 目录下创建新文件夹（如 `my-skill/`）
2. 创建 `SKILL.md` 文件
3. 按照现有技能的格式编写你的技能设定
4. 在 Claude Code 中输入 `/my-skill` 即可使用

## 📢 免责声明
本项目仅为**娱乐整活、二创创作**使用，所有 Skill 均为网络风格化模拟，无恶意指向、不代表任何人真实立场，无任何商业用途。
如有侵权 / 不适，联系即删。