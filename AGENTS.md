# Agent Instructions

这个仓库保存 `MrCarlsama短视频获客私教` Codex skill。其他 AI / Agent 进入仓库后，先按这里执行，不要凭通用内容运营经验乱改。

## 先读什么

1. 先读 `skills/aka-private-shortvideo-acquisition-diagnosis/SKILL.md`。
2. 再根据用户任务读取对应 reference：
   - 初始化诊断：`references/initialization.md`
   - 单条内容诊断：`references/content-diagnosis.md`
   - 选题库建设：`references/topic-bank.md`
   - 案例库 / 素材库：`references/case-material-bank.md`
   - 发布后复盘：`references/review-diagnosis.md`
   - 疑难杂症 / 常见 Q&A：`references/common-qa.md`
   - 私域承接进阶：`references/private-domain-advanced.md`

## 如何安装

推荐软链接安装到本地 Codex：

```bash
mkdir -p "$HOME/.codex/skills"
ln -sfn "$PWD/skills/aka-private-shortvideo-acquisition-diagnosis" \
  "$HOME/.codex/skills/mrcarlsama-shortvideo-acquisition-coach"
```

验证：

```bash
test -f "$HOME/.codex/skills/mrcarlsama-shortvideo-acquisition-coach/SKILL.md"
```

Codex 可能需要重开线程或重载后才会识别新版 skill。

## 如何正式开始

在用户的自媒体知识库或项目目录里启动，不要把用户账号资料写进本 skill 仓库。

推荐触发语：

```text
使用 MrCarlsama短视频获客私教，开始初始化诊断。
```

初始化时必须先输出“本次私教短视频获客核心理念”，再提问。不要先问“定位”。先问生意：

1. 现在最想靠短视频卖出去的具体东西是什么。
2. 这一单多少钱，谁掏钱，谁使用，谁可能反对。
3. 用户为什么现在非解决不可。

## 禁止动作

- 不经用户确认，不写入用户知识库。
- 不把内容改成统一爆款腔。
- 不追泛流量，不承诺爆款。
- 不用“抓手”这类黑话。
- 不把用户表达里的真实经历和判断抹掉。
- 不在用户没有要求时直接代写完整脚本。
