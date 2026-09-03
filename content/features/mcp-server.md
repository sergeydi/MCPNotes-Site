---
title: "MCP server"
icon: "⏚"
weight: 20
summary: "Exposes your notes to Claude and other MCP-compatible AI tools."
---

MCP Notes ships with a built-in [Model Context Protocol](https://modelcontextprotocol.io) server, so any MCP-compatible client — Claude Desktop, Claude Code, or another tool — can search your notes as part of a conversation, without you copying and pasting anything.

## What it exposes

The server sits on top of the same [semantic search]({{< relref "semantic-search.md" >}}) index MCP Notes uses internally. When Claude asks a question, it can:

- Search your notes by meaning and get back the most relevant matches.
- Read the full content of a specific note once it's been found.
- Follow [wikilinks]({{< relref "wikilinks.md" >}}) between related notes to gather more context.

## Setup

Turn the MCP server on in MCP Notes' settings, then point your MCP client at it. From there, asking Claude something like "check my notes for X" works the same way it would if you'd pasted the note in yourself — except Claude finds the right note on its own.

Because the server only runs locally, your notes are never sent anywhere except to the AI client you've explicitly connected it to.
