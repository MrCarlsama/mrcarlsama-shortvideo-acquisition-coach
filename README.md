# MrCarlsama短视频获客私教

这是 MrCarlsama 短视频获客私教 skill 的临时仓库，后续可推到 GitHub 或安装到 Codex skills 目录。

## 当前状态

- 第一版复合 skill 已经有正式入口：
  `skills/aka-private-shortvideo-acquisition-diagnosis/`.
- `design-notes/` 里的内容仍然是草稿，只有进入 skill 文件夹并带有 `SKILL.md` 的内容才算可用 skill。

## 这个 skill 解决什么

它不是普通文案助手，而是短视频获客内容诊断私教。

核心任务：

- 初始化账号底盘：先看生意，再看用户处境。
- 诊断单条内容：判断选题、脚本、产品介绍、服务介绍、资料介绍有没有服务精准用户。
- 建设精准选题库：没有爆款选题，只有精准选题。
- 整理案例库和素材库：把真实反馈、服务过程、用户原话变成信任证据。
- 做发布后复盘：判断吸引的人对不对，需求有没有被激活。
- 处理疑难杂症：一机一号、养号、权重、发布时间、日更和隔日更等执行焦虑。
- 必要时进入私域承接诊断：只在已有线索和承接入口时使用。

## 目录结构

```text
skills/        正式 skill 文件夹。
design-notes/  设计草稿和对话过程沉淀。
references/    未来可复用的方法论资料。
```

## 安装到本地 Codex

推荐用软链接安装，这样仓库更新后，本地 Codex 读到的也是最新版。

```bash
git clone https://github.com/MrCarlsama/mrcarlsama-shortvideo-acquisition-coach.git
cd mrcarlsama-shortvideo-acquisition-coach

mkdir -p "$HOME/.codex/skills"
ln -sfn "$PWD/skills/aka-private-shortvideo-acquisition-diagnosis" \
  "$HOME/.codex/skills/mrcarlsama-shortvideo-acquisition-coach"
```

验证安装：

```bash
test -f "$HOME/.codex/skills/mrcarlsama-shortvideo-acquisition-coach/SKILL.md"
grep -n "name: MrCarlsama短视频获客私教" \
  "$HOME/.codex/skills/mrcarlsama-shortvideo-acquisition-coach/SKILL.md"
```

如果 Codex 当前线程没有立刻识别新版 skill，重开一个线程或重载 Codex。

## 给其他 AI / Agent 的使用说明

如果你是另一个 AI，进入这个仓库后不要从 README 直接猜流程。先读：

1. `skills/aka-private-shortvideo-acquisition-diagnosis/SKILL.md`
2. 根据用户任务，再读对应的 `references/*.md`

路由规则：

- 用户要重新起号、换方向、问定位：读 `references/initialization.md`
- 用户丢选题、脚本、产品介绍、服务介绍、免费资料介绍：读 `references/content-diagnosis.md`
- 用户要建设选题库、热点选题、需求池：读 `references/topic-bank.md`
- 用户给客户故事、咨询记录、用户反馈、截图：读 `references/case-material-bank.md`
- 用户给发布后数据、评论、私信、成交情况：读 `references/review-diagnosis.md`
- 用户问一机一号、养号、权重、发布时间、日更：读 `references/common-qa.md`
- 用户已有线索，要诊断私信、微信、社群、成交承接：读 `references/private-domain-advanced.md`

## 正式开始使用

在用户的自媒体知识库或项目目录里启动，不要在这个 skill 仓库里替用户沉淀账号资料。

推荐用户这样发起：

```text
进入这个目录，使用 MrCarlsama短视频获客私教，开始初始化诊断。
```

初始化时，AI 必须先输出“本次私教短视频获客核心理念”，再开始提问。第一轮优先问清：

1. 用户现在最想靠短视频卖出去的具体东西。
2. 这一单多少钱，谁掏钱，谁使用，谁可能反对。
3. 用户为什么现在非解决不可。

不要先问“你的定位是什么”。按这套方法，先看生意。

## 使用铁律

- 未经用户确认，不写入用户知识库。
- 准备写入前，必须说明：写进哪里、写什么、为什么值得写。
- 内容诊断只判断框架和获客链路，不默认代写完整文案。
- 没有所谓爆款选题，只有精准选题。
- 用户不是标签，是处境中的人。
- 不用“抓手”这类黑话，直接说“内容切入口”“客户语言”“用户为什么停下来”。
