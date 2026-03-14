---
title: ai
date: 2026-03-12
tags:
  - ai
categories:
  - 個人紀錄
---

LLM 到 終端機執行專案的程式碼開發
如果需要本地部署
有那些流程
以及那些的模型可以使用

> AI
> LLM（決策） + Tool（終端機、檔案、git）+ Runtime（本地環境）。
> StarCoder2-7B


如果我想要使用 StarCoder2 的本地模型
到能在終端機下指令讓程式自動做動
還需要那些的技術與流程呢？

2.LLM 推理層
本地運行 StarCoder2 需要一個 inference runtime。

Ollama

3.Agent 控制層

LangChain


6.CLI interface


7.Memory / Context system


```bash
brew install ollama
ollama run starcoder2:7b
```

===
3. AI coding agent 的典型部署

一個合理架構如下：

Mac Host
 │
 ├ LLM runtime
 │    └ Ollama + StarCoder2 7B
 │
 ├ Agent controller
 ├ Agent CLI
 │
 └ Docker
      ├ code-runner
      ├ sandbox runner
      ├ postgres
      ├ redis
      └ vector db


