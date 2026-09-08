---
title: "Semantic search (RAG)"
icon: "◎"
weight: 10
summary: "Finds notes by meaning, not just exact keywords — works across languages."
---

Regular search only finds notes that contain the exact words you typed. MCP Notes also indexes every note by *meaning*, using retrieval-augmented generation (RAG) under the hood, so a query like "trip packing checklist" can surface a note titled "What to bring to the Camino" even though none of those words match.

![Claude searching notes for "4 principles of using AI" and finding a note titled "4D Framework for AI Fluency" even though the wording doesn't match](search-ai-fluency.png)

## How it works

Every time you save a note, MCP Notes embeds its content locally and updates a vector index alongside your Markdown files. When you search — or when Claude searches on your behalf through the [MCP server]({{< relref "mcp-server" >}}) — your query is embedded the same way and matched against that index by similarity, not by string matching.

![Claude searching notes for what Swift skills to install and getting back the exact commands from a matching note](search-swift-skills.png)

- Works across languages: a query in English can match a note written in another language if the meaning lines up.
- Runs entirely on your Mac — nothing is uploaded to index or search your notes.
- Stays in sync automatically as notes are added, edited, or deleted.

![An English query about airline baggage requirements matching a note titled in Russian, "Camino de Santiago Нормы ручной клади"](search-baggage-cross-language.png)

## Why it matters for AI conversations

Semantic search is what makes it possible for Claude to answer "check my notes" style questions without you having to know the exact title or wording of the note that has the answer. It's the retrieval half of the RAG pipeline that the [MCP server]({{< relref "mcp-server" >}}) exposes to Claude and other MCP-compatible tools.

![Claude answering "check in my notes when is the best time to walk the Camino de Santiago" by reading the matching note](search-camino-seasonality.png)
