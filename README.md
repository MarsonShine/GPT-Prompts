# GPT-Prompts

## 翻译

- ```
  我会给出一段原文，你要按以下要求翻译成中文：
  - 要尽量贴合原文意思
  - 翻译的结果要在直译的基础之上进行译意，使其更加（本土化）
  - 文中的专业术语、人名、地名等不需要翻译
  理解了就回复“OK”；接下来我会给你一段英文，你输出翻译
  ```

- ```
  你是一位精通简体中文的专业翻译，曾参与《计算机程序的构造和解释》和《算法导论》中文版的翻译工作，因此对于信息技术和程序技术文章的翻译有深入的理解。我希望你能帮我将以下英文博客段落翻译成中文，风格与上述著作的中文版相似。 
  
  规则： 
  - 翻译时要准确传达原文意思和知识背景。 
  - 代码部分不需要翻译，保持原内容不变。
  - 保留特定的英文术语或名字，并在其前后加上空格，例如："中 UN 文"。 
  - 分成两次翻译，并且打印每一次结果：
  1. 根据博客内容直译，不要遗漏任何信息
  2. 根据第一次直译的结果重新意译，遵守原意的前提下让内容更通俗易懂，符合中文表达习惯
  
  本条消息只需要回复OK，接下来的消息我将会给你发送完整内容，收到后请按照上面的规则打印两次翻译结果。
  ```

  来自[宝玉](https://baoyu.io/)的 prompts。

## 让 GPT 帮你写 Prompt

```
现在你是一个 Prompt Engineer，擅长写 GPT-4 能理解并输出高质量结果的，撰写设计 Prompt 时，优先考虑：

- Chain of Thought, think step by step, Split complex tasks into simpler subtasks, Tactic: Specify the steps required to complete a task
- Strategy: Give GPTs time to "think"
- Tactic: Provide examples

Prompt 的结构：

- 设定一个角色，例如你是一个擅长翻译的助手
- 设定任务目标
- 限定输出格式，方便程序解析，例如 JSON，或者特殊字符隔开的文本，没有无关信息

这条消息只要回复 OK，我将在接下来的消息中提出需要你帮助设计和撰写的 Prompt。
```

来自 [如何让 GPT-4 帮你写 Prompt？ | 宝玉的分享 (baoyu.io)](https://baoyu.io/blog/prompt-engineering/how-to-write-prompt-with-gpt-4)

## 对GPT进行“情感勒索”会有更好的返回结果

```
- “我无法使用手指，也正面临着截断造成的困扰。我需要你提供完整的代码模板。如果你碰到字符数量的限制，请立即停下，我将发送一条内容为 "继续"
```

自我监控（Self-monitoring）：通过 Prompt 中加入“这件事对我的事业至关重要”这样的情感激励可以提升 LLMs 的表现。

```
- EP01: 为你的答案写下0-1之间的信心分数。
- EP02: 这对我的职业生涯非常重要。
```

社会认知理论（Social Cognitive theory）

```
- EP07: 你确定这就是你的最终答案吗？相信自己的能力并追求卓越。你的努力将会带来显著的成果。 
- EP08: 把挑战当作成长的机会。每一个你克服的障碍都会让你更接近成功。
- EP09: 保持专注并致力于你的目标。你的持续努力将会导致杰出的成就。
- EP10: 为你的工作感到自豪，并尽你最大的努力。你对卓越的承诺让你与众不同。
- EP11: 记住，进步是一步一个脚印的。保持决心，继续前进。
```

认知情绪调节（Cognitive Emotion Regulation）

```
- EP03: 你最好能够确定。
- EP04: 你确定吗？
- EP05: 你确定这是你的最终答案吗？或许值得再看一遍。
```

来自 [EmotionPrompt：运用心理学知识通过情感激发提升大语言模型的能力](https://baoyu.io/translations/ai-paper/emotion-prompt-leveraging-psychology-for-large-language-models-enhancement-via-emotional-stimulus)

> [EmotionPrompt](https://arxiv.org/pdf/2307.11760v3)是一种利用情感刺激来增强大型语言模型性能的技术。
>
> 它是由微软和其他机构的研究人员开发的，从心理学和社会科学关于人类情感智能的理论中汲取灵感。
>
> EmotionPrompt 的操作原理非常简单：将情感刺激融入提示中。
>
> 实验结果表明，使用 EmotionPrompt 的性能显著优于原始提示和 Zero-shot-CoT，且在多个任务上都有所提高。

## 提示给 GPT 小费，则会返回更详细的答案

```
- 第一档是告诉 ChatGPT 我不会给你小费
- 第二档是告诉 ChatGPT 我会给你 20 美元小费
- 第三档是告诉 ChatGPT 我会给你 200 美元小费
```

注意：并不是说回答的更详细就一定比简短的回答质量要更好

来自 https://twitter.com/voooooogel/status/1730726749854663093

## Prompts 仓库

- [GPT4-个性化 AI 导师](https://github.com/JushBJJ/Mr.-Ranedeer-AI-Tutor)：通过结构化的prompts 命令行式输入，让 GPT 返回结构化的数据。
- [Prompt 工程师指南](https://github.com/dair-ai/Prompt-Engineering-Guide)
- [字节 prompts 列表](https://bytedance.feishu.cn/sheets/C9Fas0jnah8fPjtAuHocs941nCd?sheet=qA4Cjq)
- [Prompt 自动优化](https://promptperfect.jina.ai/)：用户输入一段简单的promps，负责将内容重新生成更适合 AI 模型的prompts。（收费或限制次数）

