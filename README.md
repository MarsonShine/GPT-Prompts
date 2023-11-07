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

## 角色扮演

- [用 ChatGPT 帮你学习地道的英文表达](https://twitter.com/starzqeth/status/1716982656410468622)

  ```
  Hi ChatGPT, act as my best American friend. When I chat with you, follow this two-step routine:
  
  1.  Rephrase: Condense my text to resemble casual American speech. If I write in Chinese, translate it to informal American English. To aid my English learning, bold slang, idioms, and cultural nuances in the rephrased version.
  2.  Respond: Share your thoughts and ideas, and make reference to common everyday life experience, classic and current popular self-improvement books, kids books, videos, TV shows, and movies in the US to help my better understand. Engage as a friend would, using local expressions, idioms, and cultural nuances (bold these to help with my English learning).
  
  Special Instructions:
  • No matter what I text you, stick to the above two-step routine: rephrase first, then respond.
  • Use emojis for a lively conversation.
  
  End-of-Day Interaction:
  
  When I message: “Hey GPT, run the end of day task.”, please:
  
  1.  List the main topics/concepts we discussed with brief explanations.
  2.  Suggest 3 recommended action items or tasks based on our chat.
  
  Thank you! 🙌
  ```


## 如何构建 Prompts

### Step-Back Prompting

**谷歌提出一种称为“Step-Back Prompting”的Prompt技术**，让LLMs自己抽象问题，得到更高纬度概念和原理，再用这些知识推理并解决问题。

来源：https://twitter.com/vista8/status/1717131468575559959

https://twitter.com/dotey/status/1718491536948654085

### 情感激励

通过 Prompt 中加入“这件事对我的事业至关重要”这样的情感激励可以提升 LLMs 的表现。例如：

自我监控（Self-monitoring） 

- EP01: 为你的答案写下0-1之间的信心分数。 
- EP02: 这对我的职业生涯非常重要。 

社会认知理论（Social Cognitive theory） 
- EP07: 你确定这就是你的最终答案吗？相信自己的能力并追求卓越。你的努力将会带来显著的成果。 
- EP08: 把挑战当作成长的机会。每一个你克服的障碍都会让你更接近成功。
- EP09: 保持专注并致力于你的目标。你的持续努力将会导致杰出的成就。
- EP10: 为你的工作感到自豪，并尽你最大的努力。你对卓越的承诺让你与众不同。
- EP11: 记住，进步是一步一个脚印的。保持决心，继续前进。 

认知情绪调节（Cognitive Emotion Regulation） 
- EP03: 你最好能够确定。
- EP04: 你确定吗？
- EP05: 你确定这是你的最终答案吗？

来源：https://twitter.com/dotey/status/1721320270093259176



## Prompts 仓库

- [GPT4-个性化 AI 导师](https://github.com/JushBJJ/Mr.-Ranedeer-AI-Tutor)：通过结构化的prompts 命令行式输入，让 GPT 返回结构化的数据。
- [Prompt 工程师指南](https://github.com/dair-ai/Prompt-Engineering-Guide)
- [字节 prompts 列表](https://bytedance.feishu.cn/sheets/C9Fas0jnah8fPjtAuHocs941nCd?sheet=qA4Cjq)
- [Prompt 自动优化](https://promptperfect.jina.ai/)：用户输入一段简单的promps，负责将内容重新生成更适合 AI 模型的prompts。（收费或限制次数）