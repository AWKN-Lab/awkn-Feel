# 爽点分类详细说明 / High-Point Classification Details

> 作者 / Author：AWKN / 剑锋传奇 (Jianfeng Chuanqi)
> 版本 / Version：v1.2.0
> 语言 / Language：中文 + English (Bilingual)

---

## 爽点分类体系 / Classification System

### 中文

本技能采用三级爽点分类体系，将内容中的"爽点"按重要程度分为三个级别。

### English

This skill uses a 3-tier high-point classification system, dividing the "high points" in content by importance into three levels.

---

## 一级爽点（核心爽点）/ Tier-1 High Points (Core Highlights)

### 中文

**定义**：最能调动情绪、让人血脉喷张的瞬间，是视频/内容的核心卖点。

**特征**：
- 有激烈的冲突或反转
- 有出乎意料的身份揭示
- 有强烈的情绪爆发

**分类**：

| 类型 | 说明 | 识别关键词 |
|------|------|-----------|
| **身份揭开** | 隐藏身份/真实身份被曝光，全场震惊 | "其实他是..."、"全场傻眼"、"没想到他是" |
| **终极反杀** | 最解气的翻盘，以弱胜强，打脸仇人 | "最后时刻"、"绝地反击"、"大快人心" |
| **逆袭时刻** | 从谷底到顶峰的转折，地位/能力爆发 | "从那以后"、"命运的转折"、"彻底改变" |
| **情感高潮** | 最强情绪爆发点，生死/告白/重逢 | "那一刻"、"眼泪"、"永生难忘" |

### English

**Definition**: The moments that arouse emotion and make the heart race; the core selling point of a video / piece of content.

**Characteristics**:
- Intense conflict or reversal
- Unexpected identity reveal
- Strong emotional eruption

**Categories**:

| Type | Description | Recognition Keywords |
|------|-------------|----------------------|
| **Identity Reveal** | Hidden / true identity exposed, everyone shocked | "Actually he is...", "the whole room was stunned", "nobody expected him to be" |
| **Ultimate Comeback** | The most satisfying reversal, weak beats strong, slaps enemies | "At the last moment", "desperate counterattack", "extremely satisfying" |
| **Rags-to-Riches Moment** | The turning point from rock bottom to peak, status / ability erupts | "From then on", "turning point of fate", "completely changed" |
| **Emotional Climax** | Strongest emotional eruption: life-and-death / confession / reunion | "At that moment", "tears", "unforgettable for life" |

---

## 二级爽点（重要爽点）/ Tier-2 High Points (Important Highlights)

### 中文

**定义**：提升内容丰富度，让爽点更加饱满。

**分类**：

| 类型 | 说明 | 识别关键词 |
|------|------|-----------|
| **谁跪了** | 前期嚣张的人被打脸、下跪求饶 | "跪下"、"服软"、"求饶"、"再也不敢了" |
| **打脸时刻** | 连环打脸，层层递进 | "打脸"、"没想到吧"、"之前还说..." |
| **隐藏秘密** | 之前埋的伏笔被揭开 | "原来如此"、"真相是..."、"原来他..." |
| **名场面** | 最有标志性的场景/台词 | "名场面"、"经典"、"标志性" |

### English

**Definition**: Adds richness to the content, making the highlights more substantial.

**Categories**:

| Type | Description | Recognition Keywords |
|------|-------------|----------------------|
| **Who Knelt** | Previously arrogant person gets slapped and kneels to beg | "Kneel", "soften", "beg", "never dare again" |
| **Face-Slapping Moment** | Chain of face-slaps, escalating | "Slap in the face", "didn't expect that, huh", "earlier you said..." |
| **Hidden Secret** | Previously planted foreshadowing is revealed | "So that's how it is", "the truth is...", "turns out he..." |
| **Iconic Scene** | The most signature scene / line | "Iconic scene", "classic", "signature" |

---

## 三级爽点（补充爽点）/ Tier-3 High Points (Supplementary Highlights)

### 中文

**定义**：增加内容层次，可根据需要选择使用。

| 类型 | 说明 |
|------|------|
| 糖点 | 甜宠/CP场景，暧昧/告白/发糖 |
| 笑点 | 搞笑/滑稽场景，反转/段子/吐槽 |
| 泪点 | 感动/戳心场景，生离死别/牺牲 |
| 悬念 | 最强钩子/悬念节点，结尾留钩/伏笔 |

### English

**Definition**: Adds layers to the content; can be used as needed.

| Type | Description |
|------|-------------|
| Sweet Moment | Sweet pet / CP scenes, ambiguity / confession / sugar |
| Funny Moment | Humorous / comic scenes, reversal / jokes / roast |
| Tearjerker | Touching / heartbreaking scenes, separation / sacrifice |
| Suspense | Strongest hook / suspense node, ending hook / foreshadow |

---

## 识别规则 / Recognition Rules

### 中文

#### 通用识别优先级

1. **冲突优先**：有激烈冲突的场景，爽点概率大
2. **反转优先**：有出乎意料反转的场景，爽点概率大
3. **情绪优先**：情绪波动大的场景，爽点概率大
4. **具体优先**：细节越具体，越可能是名场面

#### 爽点排序规则

按以下维度综合打分：
- **冲击力**（0-10分）：对读者情绪的冲击强度
- **戏剧性**（0-10分）：剧情的反转程度
- **情感强度**（0-10分）：情绪共鸣的深度

总分 = 冲击力×0.4 + 戏剧性×0.3 + 情感强度×0.3

#### 输出数量规则

- **1分钟版**：只保留4个一级爽点（得分最高的）
- **3分钟版**：保留10-15个核心爽点（一级全部 + 二级精选）
- **结局速通版**：只保留3个核心反转

### English

#### General Recognition Priority

1. **Conflict first**: Scenes with intense conflict have a high probability of being highlights
2. **Reversal first**: Scenes with unexpected reversals have a high probability of being highlights
3. **Emotion first**: Scenes with strong emotional swings have a high probability of being highlights
4. **Specificity first**: The more specific the details, the more likely it's an iconic scene

#### High-Point Ranking Rule

Score comprehensively by these dimensions:
- **Impact** (0-10): Strength of the emotional impact on the reader
- **Drama** (0-10): Degree of plot reversal
- **Emotional Intensity** (0-10): Depth of emotional resonance

Total score = Impact×0.4 + Drama×0.3 + Emotional×0.3

#### Output Quantity Rules

- **1-min version**: Keep only the 4 highest-scoring Tier-1 points
- **3-min version**: Keep 10-15 core points (all Tier-1 + curated Tier-2)
- **Ending rush version**: Keep only 3 core reversals

---

## 爽点提取示例 / High-Point Extraction Example

### 中文

#### 示例：都市小说

**原文段落**：
> 林天成站在会议室门口，身上还穿着那件洗得发白的外套。富二代李浩然冷笑一声："一个穷鬼也配进来？"林天成没说话，只是从口袋里掏出一张股权证明书，轻轻放在桌上。全场鸦雀无声。

**爽点识别**：
| 类型 | 得分 | 说明 |
|------|------|------|
| 身份揭开 | 9.5 | "穷鬼变股东"的身份反转 |
| 打脸时刻 | 8.0 | 富二代被当场打脸 |
| 名场面 | 8.5 | 股权证明书是关键道具 |

### English

#### Example: Urban Novel

**Original passage**:
> Lin Tiancheng stood at the conference room door, still wearing a faded, washed-out coat. The rich second-generation Li Haoran sneered, "A pauper like you doesn't belong in here?" Lin didn't say a word, just pulled an equity certificate from his pocket and placed it on the table. The whole room fell silent.

**High-Point Recognition**:
| Type | Score | Description |
|------|-------|-------------|
| Identity Reveal | 9.5 | "Pauper-to-shareholder" identity reversal |
| Face-Slapping Moment | 8.0 | Rich second-gen slapped on the spot |
| Iconic Scene | 8.5 | The equity certificate is the key prop |

---

> 作者 / Author：AWKN / 剑锋传奇 (Jianfeng Chuanqi)
