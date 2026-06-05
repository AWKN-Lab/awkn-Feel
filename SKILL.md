---
name: awkn-爽点压缩器 (High-Point Compressor)
version: v1.2.0
author: "AWKN / 剑锋传奇 (Jianfeng Chuanqi)"
description: "把小说、短剧、漫画压缩成"高爽点消费版"。支持3秒钩子、30秒剧情入口、1分钟/3分钟高能版、结局速通、角色关系图、高能片段索引。 Compress novels, short dramas, and comics into high-engagement highlight reels. Supports 3-second hooks, 30-second plot intros, 1-min / 3-min highlight versions, ending rushes, character relationship maps, and high-point indexes."
aliases: ["爽点压缩器", "highlighter-compressor", "剧情爽点提取器", "短剧解说生成器", "high-point-compressor", "highlight-extractor"]
---

# awkn-爽点压缩器 / High-Point Compressor

> 作者 / Author：AWKN / 剑锋传奇 (Jianfeng Chuanqi)
> 版本 / Version：v1.2.0
> 语言 / Language：中文 + English (Bilingual)

---

## 定位 / Positioning

### 中文

把一部80集的长篇内容，压缩成观众1分钟就能看完所有爆爽点的版本。

### English

Compress an 80-episode long-form piece into a 1-minute version that lets viewers experience every highlight moment without the filler.

---

## 目标用户 / Target Users

### 中文

1. **短剧解说博主** — 快速找到视频的所有高潮爆点
2. **小说/漫画爱好者** — 没耐心看80集，直接看最爽的部分
3. **内容创作者** — 提取高燃素材做二创剪辑

### English

1. **Short-drama narration creators** — Quickly find all the high points in a video
2. **Novel / comic enthusiasts** — Don't have patience for 80 episodes, just want the best parts
3. **Content creators** — Extract high-energy material for derivative edits

---

## 使用场景 / Use Cases

### 中文

#### 适合

- **长篇小说/漫画压缩**：百万字小说→3分钟爽线速览
- **短剧解说稿生成**：80集短剧→3分钟解说脚本
- **二创素材提取**：快速定位所有"反杀、跪舔、身份揭开"的场景

#### 不适合

- 深度文学评论
- 完整剧情总结

### English

#### Suitable for

- **Long novels / comics compression**: Million-word novel → 3-minute highlight reel
- **Short-drama narration script generation**: 80-episode short drama → 3-minute commentary script
- **Derivative material extraction**: Quickly locate all "comeback, groveling, identity reveal" scenes

#### Not suitable for

- In-depth literary criticism
- Full plot summaries

---

## 输入输出 / Inputs & Outputs

### 中文

#### 输入

| 输入项 | 说明 | 必需 |
|--------|------|------|
| 原始内容（文本/链接/视频描述） | 小说全文/漫画剧情/短剧大纲 | 是 |
| 爽点类型偏好 | 默认全选，可选指定类型 | 否，默认全类型 |
| 目标格式 | 1分钟版/3分钟版/结局速通版 | 否，默认同时输出1分钟+3分钟版 |

#### 输出

```yaml
爽点压缩结果:
  3秒钩子: "一句话爆爽点"
  30秒剧情入口: "快速了解核心爽线"
  1分钟高能版:
    - 节奏点1（0-15秒）
    - 节奏点2（15-30秒）
    - 节奏点3（30-45秒）
    - 节奏点4（45-60秒）
  3分钟高能版:
    - 剧情节点1
    - 剧情节点2
    - ...
  结局速通版: "结局3个核心反转"
  角色关系图: "谁被羞辱→谁反杀→谁隐藏身份"
  角色三维分析:
    角色弧光:
      - 起点: {状态, 动机, 代价}
      - 转折点: {触发事件, 内心冲突}
      - 终点: {新状态, 新动机, 付出的代价}
    关系张力:
      - 表面冲突: "富二代羞辱穷小子"
      - 深层冲突: "阶级固化vs个人奋斗"
      - 不可调和性: "富二代无法容忍穷人超越自己"
  高能片段索引:
    - 片段1: "谁反杀了谁（章节/时间戳）"
    - 片段2: "身份揭开（章节/时间戳）"
    - ...
  视频化建议:
    解说稿: "基于1分钟/3分钟高能版生成的口播脚本"
    分镜表:
      - 镜头1: {景别: CU, 画面: "富二代羞辱主角", 情绪: 愤怒, 时长: 3s, 运镜: 推近}
      - 镜头2: {景别: MS, 画面: "神秘电话打来", 情绪: 悬念, 时长: 5s, 运镜: 横摇}
      - 镜头3: {景别: CU, 画面: "主角宣布身份", 情绪: 震惊, 时长: 4s, 运镜: 定格}
    推荐BGM: "紧张→悬疑→高潮"
    转场建议: "快切+闪白"
    景别说明:
      - WS: 全景/远景（建立场景）
      - MS: 中景（人物半身、对话）
      - CU: 特写（面部表情、情感）
      - ECU: 大特写（极致细节、戏剧性强调）
```

### English

#### Inputs

| Input | Description | Required |
|-------|-------------|----------|
| Source content (text / link / video description) | Full novel / comic plot / short-drama outline | Yes |
| High-point type preferences | Default: all types selected | No, defaults to all |
| Target format | 1-min / 3-min / ending rush version | No, defaults to 1-min + 3-min |

#### Outputs

```yaml
high_point_compression_result:
  three_second_hook: "One-sentence highlight"
  thirty_second_intro: "Quick grasp of the core highlight line"
  one_minute_highlight_version:
    - beat_1 (0-15s)
    - beat_2 (15-30s)
    - beat_3 (30-45s)
    - beat_4 (45-60s)
  three_minute_highlight_version:
    - plot_point_1
    - plot_point_2
    - ...
  ending_rush: "3 core reversals"
  character_relationship_map: "Who humiliates whom → who comes back → who hides identity"
  character_three_dim_analysis:
    character_arc:
      - start: {state, motivation, cost}
      - turning_point: {trigger_event, inner_conflict}
      - end: {new_state, new_motivation, cost_paid}
    relationship_tension:
      - surface_conflict: "Rich kid humiliates poor kid"
      - deep_conflict: "Class rigidity vs individual struggle"
      - irreconcilability: "Rich kid cannot tolerate poor kid surpassing him"
  high_point_segment_index:
    - segment_1: "Who beat whom (chapter / timestamp)"
    - segment_2: "Identity reveal (chapter / timestamp)"
    - ...
  video_adaptation_suggestions:
    narration_script: "Voice-over script based on the 1-min / 3-min version"
    shot_list:
      - shot_1: {shot_size: CU, frame: "Rich kid humiliates MC", emotion: anger, duration: 3s, camera_move: push_in}
      - shot_2: {shot_size: MS, frame: "Mysterious call comes in", emotion: suspense, duration: 5s, camera_move: pan}
      - shot_3: {shot_size: CU, frame: "MC announces identity", emotion: shock, duration: 4s, camera_move: hold}
    bgm_recommendation: "Tense → suspenseful → climax"
    transition_suggestion: "Quick cuts + flash white"
    shot_size_legend:
      - WS: Wide shot (establishing scene)
      - MS: Medium shot (waist-up, dialogue)
      - CU: Close-up (facial expressions, emotion)
      - ECU: Extreme close-up (extreme detail, dramatic emphasis)
```

---

## 爽点分类体系 / High-Point Classification System

### 中文

#### 一级爽点（必进1分钟版）

| 爽点类型 | 说明 | 典型场景 |
|----------|------|----------|
| **身份揭开** | 隐藏身份暴露，全场震惊 | 扮猪吃老虎、隐藏大佬、假身份揭穿 |
| **终极反杀** | 最解气的翻盘对决 | 最后时刻翻盘、打脸仇人、绝地反击 |
| **逆袭时刻** | 从谷底到顶峰的转折 | 被开除→当老板、被羞辱→成赢家 |
| **情感高潮** | 最强情绪爆发点 | 告白/求婚、重逢/和解、生死抉择 |

#### 二级爽点（必进3分钟版）

| 爽点类型 | 说明 | 典型场景 |
|----------|------|----------|
| **谁跪了** | 前期嚣张的人被打脸 | 恶人下跪、反派服软、仇人求饶 |
| **打脸时刻** | 连环打脸，层层递进 | 打赌输了、预测失败、实力碾压 |
| **隐藏秘密** | 之前埋的坑填了 | 真实目的揭晓、过去真相大白 |
| **名场面** | 最有标志性的场景 | 经典台词、标志性动作、画面爆点 |

#### 三级爽点（可选进3分钟版）

| 爽点类型 | 说明 |
|----------|------|
| 糖点 | 甜宠/CP场景 |
| 笑点 | 搞笑/滑稽场景 |
| 泪点 | 感动/戳心场景 |
| 悬念 | 最强钩子/悬念节点 |

### English

#### Tier-1 High Points (Must appear in 1-min version)

| Type | Description | Typical Scenes |
|------|-------------|----------------|
| **Identity Reveal** | Hidden identity exposed, audience shocked | Playing dumb, hidden big shot, fake identity exposed |
| **Ultimate Comeback** | Most satisfying reversal, weak beats strong | Last-minute reversal, slapping enemies, desperate counterattack |
| **Rags-to-Riches Moment** | Turning point from rock bottom to peak | Fired → becomes boss, humiliated → becomes winner |
| **Emotional Climax** | Strongest emotional eruption | Confession / proposal, reunion / reconciliation, life-or-death choice |

#### Tier-2 High Points (Must appear in 3-min version)

| Type | Description | Typical Scenes |
|------|-------------|----------------|
| **Who Knelt** | Previously arrogant person gets slapped, kneels | Villain kneels, antagonist softens, enemies beg |
| **Face-Slapping Moment** | Chain of face-slaps, escalating | Lost a bet, failed prediction, strength crush |
| **Hidden Secret** | Earlier foreshadowing pays off | True motive revealed, past truth surfaces |
| **Iconic Scene** | Most signature scene / line | Classic line, signature move, visual highlight |

#### Tier-3 High Points (Optional in 3-min version)

| Type | Description |
|------|-------------|
| Sweet Moment | Sweet pet / CP scenes |
| Funny Moment | Humorous / comic scenes |
| Tearjerker | Touching / heartbreaking scenes |
| Suspense | Strongest hook / suspense node |

---

## 核心流程 / Core Workflow

### 中文

```
输入内容
    │
    ▼
STEP 1: 爽点定位
    ├─ 识别一级爽点（身份/反杀/逆袭/情感高潮）
    ├─ 识别二级爽点（跪舔/打脸/秘密/名场面）
    └─ 识别三级爽点（糖/笑/泪/悬念）
    │
    ▼
STEP 2: 爽点排序
    ├─ 按冲击力、戏剧性、情感强度综合打分
    ├─ 确定1分钟版只保留4个一级爽点
    └─ 确定3分钟版保留10-15个核心爽点
    │
    ▼
STEP 3: 爽点叙事化
    ├─ 3秒钩子 → 最爆的一句话
    ├─ 30秒剧情入口 → 快速理解爽线
    ├─ 1分钟版 → 4个关键爽点串联
    ├─ 3分钟版 → 10-15个爽点按节奏排布
    ├─ 结局速通 → 3个核心反转
    ├─ 角色关系图 → 谁和谁有仇
    ├─ 角色三维分析 → 角色弧光+关系张力
    └─ 视频化建议 → 解说稿+分镜表+BGM+转场
    │
    ▼
输出完整结果
```

### English

```
Input content
    │
    ▼
STEP 1: High-Point Identification
    ├─ Identify Tier-1 points (Identity / Comeback / Rags-to-Riches / Emotional)
    ├─ Identify Tier-2 points (Kneeling / Face-slap / Secret / Iconic)
    └─ Identify Tier-3 points (Sweet / Funny / Tear / Suspense)
    │
    ▼
STEP 2: High-Point Ranking
    ├─ Score by impact, drama, emotional intensity
    ├─ For 1-min version: keep top 4 Tier-1 points
    └─ For 3-min version: keep 10-15 core points
    │
    ▼
STEP 3: High-Point Narrative
    ├─ 3-sec hook → Most explosive one-liner
    ├─ 30-sec intro → Quick grasp of the highlight line
    ├─ 1-min version → 4 key points chained
    ├─ 3-min version → 10-15 points with rhythm
    ├─ Ending rush → 3 core reversals
    ├─ Character map → Who has beef with whom
    ├─ Character 3D analysis → Arc + Relationship tension
    └─ Video adaptation → Script + Shot list + BGM + Transitions
    │
    ▼
Output full result
```

---

## 能力边界 / Capability Boundaries

### 中文

#### 做什么

- 提取所有核心爽点并按类型分类
- 生成1分钟/3分钟两个版本的压缩内容
- 提供3秒钩子、角色关系图、角色三维分析（弧光+关系张力）、高能片段索引
- 给出适合做解说的文案和分镜建议
- 提供视频化输出：解说稿、分镜表、BGM建议、转场建议

#### 不做什么

- 不做完整剧情总结（只留爽点，跳过铺垫）
- 不做深度文学分析
- 不生成完整视频（只给出素材索引和文案）

### English

#### What it does

- Extracts all core high points and classifies them by type
- Generates both 1-min and 3-min compressed versions
- Provides 3-sec hook, character relationship map, character 3D analysis (arc + tension), high-point index
- Gives narration-friendly copy and shot-list suggestions
- Provides video adaptation output: narration script, shot list, BGM suggestions, transition suggestions

#### What it doesn't do

- No full plot summary (keeps only high points, skips setup)
- No in-depth literary analysis
- No full video generation (only material index and copy)

---

## 爽点叙事化规则 / High-Point Narration Rules

### 中文

#### 3秒钩子规则

**核心原则**：用一句**具体冲突、处境或问题**拉住读者，不是只说"最爆"，而是让读者**立刻感受到张力**。

**钩子模板**：
- ✅ **反杀版**："穷小子一夜暴富，直接买下仇人公司！"
- ✅ **身份版**："人人看不起的清洁工，竟然是上市公司老板！"
- ✅ **处境锚定版**："被羞辱的实习生，第二天成了全公司的老板。"
- ❌ 铺垫版："从前有个穷小子，他很努力，后来..."
- ❌ 空泛版："这是一个关于奋斗和成功的故事。"

**钩子自检清单**（交付前检查）：
1. 是否有具体对象？（谁）
2. 是否有真实处境？（被羞辱/被看不起/绝境）
3. 是否有画面或动作？（买下公司/宣布身份）
4. 是否少了空泛形容词？（删除"非常""特别""极其"）

**去 AI 味检查**：
- 删除模板感："经过一番努力""最终""总而言之"
- 删除热词堆砌："绝绝子""yyds""破防了"
- 删除泛泛价值判断："这个故事告诉我们""人生就是这样"
- 保留：具体动作、具体对话、具体场景

#### 30秒剧情入口规则

讲清核心爽线逻辑：
- 谁被谁羞辱/压制（10秒）
- 谁反杀谁/身份怎么揭开（10秒）
- 最爽的结局是什么（10秒）

#### 1分钟高能版规则

严格按4个节奏点：
- 0-15秒：第一个爽点（悬念/第一个小高潮）
- 15-30秒：第二个爽点（升级冲突）
- 30-45秒：第三个爽点（更大反杀）
- 45-60秒：第四个爽点（高潮结尾，留钩子）

#### 3分钟高能版规则

按"上升→高潮→结局"三幕结构：
- 0-60秒：铺垫阶段（前情回顾+3-5个小爽点）
- 60-150秒：高潮阶段（5-8个核心爽点）
- 150-180秒：结局阶段（终极反杀+身份揭开+情感收尾）

### English

#### 3-Second Hook Rules

**Core principle**: Use a sentence with a **specific conflict, situation, or question** to grab the reader. Don't just say "the most explosive"—make the reader **feel the tension immediately**.

**Hook templates**:
- ✅ **Comeback version**: "The broke kid gets rich overnight and buys out his enemy's company!"
- ✅ **Identity version**: "The janitor everyone looked down on turns out to be a public-company CEO!"
- ✅ **Situation-anchored version**: "The humiliated intern became the boss of the whole company the next day."
- ❌ Setup version: "Once upon a time, there was a poor boy who worked hard, and then..."
- ❌ Vague version: "This is a story about struggle and success."

**Hook self-checklist** (verify before delivery):
1. Is there a specific subject? (Who)
2. Is there a real situation? (Humiliated / looked down on / desperate)
3. Is there a visual or action? (Buys the company / announces identity)
4. Are vague modifiers removed? (Delete "very," "extremely," "incredibly")

**De-AI flavor check**:
- Remove templated feel: "after some effort," "in the end," "to sum up"
- Remove buzzword stacks: "literally iconic," "no cap," "I'm shook"
- Remove generic value judgments: "This story tells us," "life is like that"
- Keep: specific actions, specific dialogue, specific scenes

#### 30-Second Intro Rules

Make the core highlight line clear:
- Who humiliates / suppresses whom (10 sec)
- Who comes back on whom / how identity is revealed (10 sec)
- What's the most satisfying ending (10 sec)

#### 1-Minute Highlight Rules

Strictly 4 beats:
- 0-15 sec: First highlight (suspense / first small climax)
- 15-30 sec: Second highlight (escalate conflict)
- 30-45 sec: Third highlight (bigger comeback)
- 45-60 sec: Fourth highlight (climax ending, leave a hook)

#### 3-Minute Highlight Rules

Three-act structure "build-up → climax → ending":
- 0-60 sec: Build-up (recap + 3-5 small highlights)
- 60-150 sec: Climax (5-8 core highlights)
- 150-180 sec: Ending (ultimate comeback + identity reveal + emotional close)

---

## 典型输出示例 / Sample Output

### 中文

#### 输入

> 一部都市小说：穷小子林天成被富二代羞辱，其实他是隐藏的豪门继承人，最后一步步反杀所有仇人，买下仇人公司，让仇人全家下跪道歉。

#### 输出示例

```yaml
爽点压缩结果:
  3秒钩子: "穷小子一夜暴富，直接买下仇人公司！"
  30秒剧情入口: "富二代羞辱穷小子林天成，没想到他是隐藏的豪门继承人，最后买下仇人公司让仇家全部跪下。"
  1分钟高能版:
    - 0-15秒：[第一个爽点] 富二代在公司大堂羞辱林天成，让他跪下学狗叫
    - 15-30秒：[第二个爽点] 神秘电话打来，富二代老板态度立刻180度转变
    - 30-45秒：[第三个爽点] 林天成当众宣布自己是集团继承人，全场震惊
    - 45-60秒：[第四个爽点] 直接下令收购富二代的公司，让他全家滚蛋
  3分钟高能版:
    - 0-60秒（铺垫）：
      * 林天成在公司当实习生，被富二代羞辱
      * 第一次小反杀：林天成一句话让富二代吃瘪
      * 第二次小爽点：神秘人物出现，对林天成毕恭毕敬
    - 60-150秒（高潮）：
      * 身份正式揭开：林天成是集团唯一继承人
      * 第一波反杀：直接开除当初骂他的主管
      * 第二波反杀：冻结富二代父亲的所有资产
      * 第三波反杀：公开富二代所有黑料
      * 名场面：林天成拿出股权证，全场傻眼
    - 150-180秒（结局）：
      * 终极反杀：成功收购富二代家的公司
      * 跪舔时刻：富二代全家来公司门口下跪道歉
      * 情感收尾：林天成看着仇人，选择放过但让他们付出代价
  结局速通版: "三个核心反转：1.林天成是继承人 2.收购仇人公司 3.仇家全部下跪求饶"
  角色关系图: "林天成（隐藏继承人）←羞辱/反杀→ 富二代（嚣张仇人）"
  高能片段索引:
    - 片段1: 富二代羞辱林天成（第一章）
    - 片段2: 神秘人物出现对林天成毕恭毕敬（第五章）
    - 片段3: 身份正式揭开（第二十章）
    - 片段4: 收购仇人公司（第五十章）
    - 片段5: 仇家下跪道歉（第六十章）
```

### English

#### Input

> An urban novel: Poor kid Lin Tiancheng gets humiliated by a rich second-generation kid, but he's actually a hidden heir to a wealthy family. He gradually takes revenge on all his enemies, buys out their company, and forces their whole family to kneel and apologize.

#### Sample Output

```yaml
high_point_compression_result:
  three_second_hook: "The broke kid gets rich overnight and buys out his enemy's company!"
  thirty_second_intro: "A rich second-gen humiliates broke kid Lin Tiancheng, never knowing he's a hidden heir. He ends up buying out the enemy's company and making them all kneel."
  one_minute_highlight_version:
    - 0-15s: [Highlight 1] Rich kid humiliates Lin in the lobby, forces him to kneel and bark like a dog
    - 15-30s: [Highlight 2] A mysterious call comes in; the rich kid's boss instantly does a 180
    - 30-45s: [Highlight 3] Lin publicly announces he's the group's heir—the whole room is stunned
    - 45-60s: [Highlight 4] He orders the acquisition of the rich kid's company and kicks the whole family out
  three_minute_highlight_version:
    - 0-60s (build-up):
      * Lin works as an intern and is humiliated by the rich kid
      * First small comeback: Lin silences the rich kid with one sentence
      * Second small highlight: A mysterious figure appears, deeply respectful to Lin
    - 60-150s (climax):
      * Identity officially revealed: Lin is the group's sole heir
      * First wave of revenge: Fires the manager who insulted him
      * Second wave: Freezes the rich kid's father's assets
      * Third wave: Exposes all the rich kid's dirt
      * Iconic scene: Lin produces the equity certificate; the room is stunned
    - 150-180s (ending):
      * Ultimate comeback: Successfully acquires the rich kid's family company
      * Groveling moment: The rich kid's whole family kneels at the company gate
      * Emotional close: Lin looks at his enemies, chooses to let them go but makes them pay
  ending_rush: "3 core reversals: 1. Lin is the heir 2. Acquires the enemy's company 3. Enemies all kneel and beg"
  character_relationship_map: "Lin Tiancheng (hidden heir) ←humiliation/comeback→ Rich kid (arrogant enemy)"
  high_point_segment_index:
    - segment_1: Rich kid humiliates Lin (Chapter 1)
    - segment_2: Mysterious figure shows respect (Chapter 5)
    - segment_3: Identity officially revealed (Chapter 20)
    - segment_4: Acquires the enemy's company (Chapter 50)
    - segment_5: Enemies kneel and apologize (Chapter 60)
```

---

## 文件体系 / File Structure

### 中文

```
awkn-爽点压缩器/
├── SKILL.md                           # 技能主文件
├── CHANGELOG.md                       # 版本更新记录
├── references/
│   └── 01_high_point_categories.md    # 爽点分类详细说明
└── samples/
    └── 01_sample_novel_compression.md  # 小说爽点压缩示例
```

### English

```
awkn-high-point-compressor/
├── SKILL.md                           # Main skill file (Bilingual)
├── CHANGELOG.md                       # Version history
├── references/
│   └── 01_high_point_categories.md    # Detailed classification
└── samples/
    └── 01_sample_novel_compression.md  # Sample novel compression
```

---

## 版本历史 / Version History

| 版本 / Version | 日期 / Date | 更新内容 / Changes |
|----------------|-------------|---------------------|
| v1.0.0 | 2026-05 | 初始版本：三级爽点分类体系 / Initial: 3-tier classification system |
| v1.1.0 | 2026-05 | 新增角色三维分析、视频化输出、叙事化规则 / Added 3D character analysis, video output, narration rules |
| v1.2.0 | 2026-06 | 升级为中英双语版 / Upgraded to bilingual (Chinese + English) |

---

> 作者 / Author：AWKN / 剑锋传奇 (Jianfeng Chuanqi)
