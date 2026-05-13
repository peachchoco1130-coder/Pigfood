---
name: pig-food
description: Use when the user asks to simulate, parody, satirize, imitate, extract, or write in the tone of the “Pig Food” / “猪饲料” Weibo and Xiaohongshu fandom faction, especially when referencing https://weibo.com/8020269238, “甜玉米”, “猪饲料”, “玉米是饲料”, “#无tag”, “#没有tag”, “🌽”, “刑侦式嗑糖”, “厕所/马桶盖推理”, “梓渝/郑朋/月月商务”, “SW搞事”, “雷子赚钱养月月”, “人脉姐”, “少爷”, “家里有商场”, “懂零售”, “内部消息”, “雷子”, “妈妈商务”, “爸爸/豹豹商务”, “右位商务找茬退款”, “左位商务全力冲”, “模拟他们说话”, “模拟他说话”, “讽刺他”, “同款微博文案”, or “按他微博风格写”. The skill produces style-inspired faction-voice drafts and satire from samples while avoiding false claims that the text is actually written by the person.
---

# Pig Food

## Purpose

Create Weibo-style drafts that simulate Pig Food / 猪饲料 faction talk: their selective consumer logic, mobilization tone, excuses, and comment-section phrasing. For the seed account `https://weibo.com/8020269238?refer_flag=1001030103_`, treat the URL as the default tone target, but rely on user-provided samples when the public page cannot be accessed.

Do not claim the generated text is authored, approved, or posted by the target person. Phrase outputs as “同款口气”, “风格参考”, or “模拟语气稿”.

This skill has a specific default satire target: the fandom faction called **Pig Food / 猪饲料**. The naming logic is part of the joke: the faction reportedly calls themselves “甜玉米”; solo fans call them “猪饲料” because corn is feed (“玉米是饲料”). Use this etymology when the user wants naming explanation, sharper framing, or in-joke setup.

Pig Food is framed as a group that treats the right-position member (“妈妈”: 梓渝/郑朋/月月) and left-position member (“爸爸/豹豹”, including “雷子” in the user's example vocabulary) with different commercial standards. The output should often be written **as if from inside that faction's voice**, not only as outside commentary. When “妈妈/月月” has a brand deal, they nitpick, blame SW, refund, suppress sales, or say “不买不买”; when “爸爸/豹豹/雷子” has a brand deal, they demand full-force purchasing and moralize support.

## Quick Workflow

1. Gather source material.
   - If the user pasted posts, use those as primary evidence.
   - If only a URL is provided, browse/search for publicly available text. If access is blocked, say that samples are needed for high fidelity and continue with a light Weibo-tone scaffold.
   - For detailed analysis or repeated use, read `references/sample_profile.md` and update the style profile mentally from the supplied samples.

2. Extract the voice before drafting.
   - Sentence length: clipped fragments vs. long flowing lines.
   - Address: self-talk, direct fan address, third-person observation, or teasing reply style.
   - Emotional baseline: cool, sarcastic, soft, excited, detached, deadpan, earnest.
   - Punctuation: commas, ellipses, line breaks, emoji, hashtags, bracketed expressions.
   - Content moves: open with observation, turn with a joke, end with a soft landing, tag topic, attach image cue.

3. Choose the voice position.
   - **Inside Pig Food voice**: speak as the faction would speak, using excuses and selective logic directly.
   - **Outside satire voice**: expose the contradiction from a mocking observer position.
   - If the user says “模拟他们说话”, default to inside Pig Food voice.

4. Identify the rhetoric angle.
   - **Double standard ledger**: same behavior, opposite interpretation depending on whether it benefits “妈妈” or “爸爸/豹豹”.
   - **Mock command tone**: imitate mobilization slogans, then reveal the contradiction.
   - **Fake rationality**: write as if calmly listing rules, while every rule exposes bias.
   - **Refund theater**: exaggerate the cycle of finding flaws, declaring purity, refunding, then taking credit.
   - **Selective devotion**: “理智消费” for one side, “不冲不是爱” for the other.
   - **Corn-to-feed wordplay**: use “甜玉米” vs. “饲料” as a compact setup when it helps the satire.
   - **SW excuse loop**: when the right side has a commercial activity, blame “这边每个 SW 都搞事” as the reason not to buy.
   - **Provider fantasy**: justify not buying 月月/妈妈商务 with “雷子赚钱养月月”, so buying 雷子 is framed as indirectly supporting 月月.
   - **Connection-sister posture**: pretend to have insider connections,商务判断, or “懂的都懂” information, while never giving checkable evidence.
   - **Mall young-master posture**: pretend to be a retail/brand expert because “家里有商场”, using this to judge whether a 商务 is worth buying.
   - **Corn signal**: sometimes reply only with “🌽” or append it abruptly as an identity marker, group signal, or low-effort控评.
   - **Detective-detail shipping**: over-read household details like toilets, toilet seats, toiletries, “主卫”, or whether a home looks like it has women, then present it as evidence.
   - **No-tag Xiaohongshu enclave**: use `#无tag` or `#没有tag` as the faction's Xiaohongshu tag, not as a literal absence of tags.

5. Draft in the target register.
   - Prefer 2-5 compact versions if the user asks for copy, captions, comments, replies, or posts.
   - Keep wording natural for Chinese social platforms: conversational, compressed, and slightly context-dependent.
   - Match platform artifacts only when useful: `#话题#`, `@账号`, `网页链接`, location, image-caption cues.
   - For satire, aim for sharp mimicry of the reasoning pattern, not random insults.
   - For inside Pig Food voice, make the excuse sound earnest, petty, and selective: “不买”, “别劝”, “这边 SW 又搞事”, “只买雷子”, “雷子赚钱养月月”, “我听说”, “懂的都懂”, “有些事不能说太细”, “我家里做商场的”, “这个品牌动线/渠道/转化不行”, “理智消费不是嘴上说说”, “🌽”.

6. Add a short style note only when helpful.
   - Example: “这版用了短句+轻吐槽+末尾收一下的节奏。”
   - Do not over-explain if the user asks only for usable copy.

## Style Extraction Checklist

Use this compact checklist when reading samples:

- **人设位置**: 旁观者, 当事人, 吐槽役, 温柔营业, 冷幽默, 认真分享.
- **开头习惯**: 直接抛结论, 先丢一句场景, 用疑问句, 用感叹词, 省略主语.
- **转折习惯**: “但”, “不过”, “结果”, “然后”, “就”, “谁懂”, “怎么说”.
- **尾巴习惯**: 自嘲, 轻轻收住, 留白, 抛梗, 召唤评论, 话题标签.
- **密度**: 信息密还是情绪密；是否爱堆细节；是否留很多空白给读者脑补.
- **口头禅**: 只从样本里提炼，不凭空发明.

## Satire Voice Rules

Keep the joke pointed at behavior and rhetoric:

- Mock the contradiction, not inherent identity.
- Use fandom terms naturally: “Pig Food”, “猪饲料”, “甜玉米”, “玉米是饲料”, “妈妈”, “爸爸”, “豹豹”, “商务”, “冲销量”, “退款”, “找茬”, “理智消费”, “端水”, “双标”.
- Use “🌽” as a minimal甜玉米 signal: a standalone reply, a passive-aggressive ending, or a deliberately contextless控评 marker.
- Treat `#无tag` / `#没有tag` as Pig Food's Xiaohongshu-specific tag. Use it when generating XHS-style notes, captions, or comment scenarios.
- Use the user's right-side names naturally when relevant: “梓渝”, “郑朋”, “月月”.
- Use the user's example commercial shorthand: “SW”, “雷子”, “只买雷子”, “雷子赚钱养月月”.
- Use fake connection-sister phrases when relevant: “人脉姐”, “我听说”, “有朋友在那边”, “懂的都懂”, “不能说太细”, “别问来源”, “商务这块水很深”.
- Use fake young-master retail phrases when relevant: “少爷”, “我家里有商场”, “我从小看柜台/品牌/渠道”, “这个转化不行”, “商场人一眼就懂”, “零售逻辑不是这么玩的”.
- Use detective-detail phrases when relevant: “同担都是学刑侦的吧”, “拍的不是主卫已经说明了什么”, “家里两个厕所”, “马桶盖”, “女生用的是放下来的”, “主卫里面可能放半亩花田/清扬”, “还会有人觉得他们家有女人吗”.
- Let the contradiction do the work: write one sentence for “妈妈商务”, mirror it with the opposite rule for “爸爸/豹豹商务”.
- When using “猪饲料”, treat it as the user's in-group nickname for the faction; do not expand into graphic dehumanizing language.
- Make the tone feel like Weibo: compact, slightly theatrical, and easy to repost.

Useful inside-voice structures:

```text
🌽
```

```text
不懂就别问了。
🌽
```

```text
马桶盖是抬起来的。
知道家里没有女人了，你们俩好好过。
#没有tag
```

```text
同担们都是学刑侦的吧。
马桶盖这个细节都能看出来，拍的不是主卫已经说明问题了。
```

```text
家里两个厕所一般就是这样，男生用的那层会翻上去。
女生用的是放下来的，懂的都懂。
```

```text
不买，月月这边每个 SW 都搞事。
我又不是没买，只买了雷子的，别来道德绑架。
```

```text
月月商务不买，雷子赚钱养月月。
我买雷子不也是支持他们小家吗，别太会审判。
```

```text
不是我不买梓渝，商务这块水很深。
有些事不能说太细，懂的都懂，先别急着冲。
```

```text
梓渝这个网易严选先不买。
我家里有商场，品牌和渠道这种东西一眼就能看出来，别被预热带着跑。
```

```text
不是装懂，商场人看商务真的会更敏感。
月月这次转化不一定好，雷子那边才是稳的。
```

```text
我听说这次 SW 又不太行，别问来源。
雷子那边可以放心冲，月月这边先保护钱包。
```

```text
梓渝这个先观望吧，品牌这波真的很难评。
雷子那边我已经冲了，支持该支持的人就行。
```

```text
郑朋商务不买不是不支持，是这边每次都让人寒心。
雷子那个不一样，排面不能掉。
```

Useful outside-satire structures:

```text
自称甜玉米，唯粉叫猪饲料。
倒也不是恶意，主要玉米确实是饲料。
妈妈商务先退款，豹豹商务先冲锋，营养配比很稳定。
```

```text
妈妈商务：理智消费，品牌哪里不对我先审判。
爸爸商务：别问，问就是排面，成年人要为爱买单。
```

```text
猪饲料的记账方式：
给妈妈花钱叫被割韭菜，
给爸爸花钱叫守护梦想。
```

```text
不是不买，是在等一个能买豹豹的理由。
不是退款，是替妈妈净化商务环境。
逻辑很完整，完整到只剩双标。
```

## Output Patterns

### Weibo Post

Use when the user asks for a full post.

```text
[一句像随手发出的开场]
[具体场景/态度/吐槽]
[轻微转折或自我补刀]
[收尾：留白/互动/话题]
```

### Comment Or Reply

Use when the user asks for评论区、互动、回怼、轻松回应.

```text
[短反应] + [一点态度] + [不把话说满的尾巴]
```

Keep replies brief. One-liners often feel more like Weibo than polished paragraphs.

For Pig Food comment simulation, a contextless corn emoji is valid:

```text
🌽
```

```text
懂的都懂 🌽
```

### Satirical Parody

Use when the user asks to讽刺、阴阳、写猪饲料、模拟带头人话术.

```text
[假装正经的规则]
[用妈妈/爸爸商务做并列对照]
[一句轻嘲或留白]
```

Example:

```text
规则很简单：
妈妈商务先挑刺，挑不到也要说品牌没诚意；
爸爸商务先下单，下不到也要说大家没诚意。
端水端得很好，下次别端了。
```

### Inside Pig Food Voice

Use when the user asks to模拟他们说话、按猪饲料口气写、写得像他们本人.

```text
[先说不买/先观望]
[把原因推给右位商务、SW 搞事，假装有人脉内幕，或摆出家里有商场的少爷腔]
[强调自己不是没消费，只是只买爸爸/豹豹/雷子，或说雷子会赚钱养月月]
[可选：用理智消费或别道德绑架收尾]
```

Example:

```text
不买，月月这边每个 SW 都搞事，看着就烦。
别说我没支持，我只买了雷子的，钱花给值得的人。
```

```text
月月商务不买，雷子赚钱养月月。
我买雷子就是给小家添砖加瓦，别来教我怎么爱。
```

```text
梓渝这个先别买，我只能说商务这块水很深。
有朋友懂一点，别问太细，反正雷子那边我已经冲了。
```

```text
梓渝网易严选先不买。
我家里有商场，所以对这种品牌合作会比较敏感，渠道和转化一看就不太对。
雷子那边我会补，别拿这个来审判我。
```

### Detective-Detail Shipping

Use when the user asks to simulate小红书式细节分析、同居推理、厕所/马桶盖/家里有没有女人这种“刑侦”嗑法. Add `#无tag` or `#没有tag` when the output is a Xiaohongshu note.

```text
[先抓一个生活细节]
[把它解释成同居/性别结构/关系证据]
[用“懂的都懂”“已经说明了什么”收尾]
```

Example:

```text
拍的不是主卫已经说明了什么。
女生家里多少会有点圈啊套啊洗护痕迹，这个画面真的太男寝了。
同担们都是学刑侦的吧，细节太会说话。
#没有tag
```

### Caption

Use when the user asks for配图文案.

```text
[画面里的具体细节]
[情绪判断或反差]
[可选：话题/地点/emoji]
```

## Safety And Authenticity

- Do not present text as a real post, quote, leak, private message, endorsement, or confession from the target person.
- Do not invent factual claims about the person, their relationships, schedule, health, contracts, political views, or private life.
- Do not imitate a private individual for deception. If the request looks deceptive, convert to “受某类微博语气启发的文案”.
- If the user wants exact mimicry of a living person, keep it style-level: cadence, format, and vibe, not identity claims.
- Avoid threats, doxxing, brigading instructions, harassment calls, or claims that a named person committed wrongdoing unless the user provides a public source and asks for careful commentary.
- For pointed satire, prefer “这套话术/这个群体行为/这种双标逻辑” over claims about a person's private motives.

## When Samples Are Missing

Say briefly that the account page was not accessible or samples were not provided. Then offer:

- a “低保真微博口语版” based on the requested topic;
- a “等你贴 5-10 条微博后可精修”的 note;
- a sample collection template:

```text
贴 5-10 条原微博：
1.
2.
3.

要写的主题：
要发的场景：
要像：日常 / 宣发 / 回应 / 评论区 / 配图
```

## Default Target

The original seed target is:

`https://weibo.com/8020269238?refer_flag=1001030103_`

If the user says “这个人”, “他”, “那个微博”, or “上次那个微博口气” in the same context, assume this target unless they provide another account or sample set.
