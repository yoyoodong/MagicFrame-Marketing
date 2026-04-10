# Magicframe 自媒体运营工作流 - 分享包

## 📦 这是什么?

这是 Magicframe AI 画框的完整自媒体运营工作流系统,可以帮你从选题到发布完成整个内容创作流程。

## 🚀 快速开始

### 方式 1: 使用 Claude Code (推荐)

1. **安装 Claude Code**
   - CLI: `npm install -g @anthropic-ai/claude-code`
   - 或访问 https://claude.ai/code

2. **克隆或下载这个项目**
   ```bash
   git clone [你的仓库地址]
   cd marketing
   ```

3. **启动 Claude Code**
   ```bash
   claude-code
   ```

4. **开始使用**
   ```
   告诉我: "帮我从内容池选一个选题"
   ```

### 方式 2: 使用 claude.ai (网页版)

1. 访问 https://claude.ai
2. 上传以下文件到对话:
   - `CLAUDE.md` (项目配置)
   - `pool.html` (内容池数据)
   - `WORKFLOW.md` (工作流说明)
3. 告诉 Claude: "帮我从内容池选一个选题"

## 📋 包含的文件

```
marketing/
├── README-SHARE.md          # 本文件
├── CLAUDE.md                # Claude 项目配置(自动加载)
├── WORKFLOW.md              # 完整工作流说明
├── pool.html                # 内容池数据(5个卖点)
├── content/                 # 内容目录
│   ├── briefs/             # 策划案
│   ├── drafts/             # 草稿
│   └── published/          # 已发布
└── data/
    └── analytics/          # 数据分析
```

## 🎯 工作流程

```
选题 → 策划 → 创作 → 制作 → 审核 → 发布 → 追踪
```

### 1. 选题
从 pool.html 的 5 个卖点中智能推荐选题

### 2. 策划
生成完整策划案(标题、大纲、视觉建议)

### 3. 创作
根据内容形式创作(小红书图文/视频脚本/长文章)

### 4. 制作
生成小红书图片、视频拍摄清单

### 5. 审核
检查品牌调性、敏感词、平台规则

### 6. 发布
发布到小红书/抖音/公众号/微博

### 7. 追踪
记录和分析发布数据

## 💡 使用示例

```
你: "帮我从内容池选一个选题"
Claude: [分析内容池,推荐选题]

你: "为便利贴生成小红书图文"
Claude: [完成选题→策划→创作→制作全流程]

你: "审核这个内容"
Claude: [检查并给出建议]

你: "记录发布数据: 小红书 https://xxx 点赞50"
Claude: [记录到数据文件]
```

## 🛠️ 可选: 安装 baoyu-skills

如果需要自动生成小红书图片和发布功能:

```bash
# 安装 baoyu-skills
npx skills add https://github.com/jimliu/baoyu-skills

# 重启 Claude Code
```

可用的 skills:
- `/baoyu-xhs-images` - 生成小红书图片
- `/baoyu-post-to-wechat` - 发布到公众号
- `/baoyu-post-to-weibo` - 发布到微博

## 📊 内容池数据

5 个卖点:
1. 便利贴(留言/待办)
2. AI创作(AI生图/AI涂鸦)
3. 家庭日常(家庭信息/到家状态/提醒)
4. 习惯养成/打卡(能量积木)
5. 家庭美术馆(照片/艺术化展示/名画)

每个卖点包含:
- 情感主题包(3个母题)
- 趣味主题包(3个母题)
- 视频/图文/文章方向

## ❓ 常见问题

**Q: 需要编程基础吗?**
A: 不需要,直接对话即可使用。

**Q: 可以自定义内容池吗?**
A: 可以,直接编辑 pool.html 文件。

**Q: 生成的内容保存在哪里?**
A: 自动保存到 content/ 目录下。

**Q: 可以多人协作吗?**
A: 可以,通过 Git 共享项目即可。

## 📝 更新日志

- 2026-04-10: 初始版本,完整工作流系统

## 🔗 相关链接

- Claude Code: https://claude.ai/code
- Skills 市场: https://skills.sh
- 项目仓库: [你的 GitHub 仓库]

## 💬 反馈与支持

如有问题或建议,请联系项目维护者。

---

**开始使用**: 告诉 Claude "帮我从内容池选一个选题"
