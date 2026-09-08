---
title: "iCloud sync"
icon: "☁"
weight: 40
summary: "Plain .md files that sync automatically across your Mac, iPad, and iPhone."
---

Notes in MCP Notes are stored as plain `.md` files in your iCloud Drive — not locked into a proprietary database or format. iCloud handles syncing them across your Mac, iPad, and iPhone the same way it syncs any other file.

![The same note, "Claude Code Hooks," open in MCP Notes on Mac](icloud-sync-mac.png)

![The same note open in MCP Notes on iPad, synced via iCloud](icloud-sync-ipad.png)

<img class="shot-phone" src="icloud-sync-iphone.png" alt="The same notes list synced to MCP Notes on iPhone">

## No lock-in

Because notes are just Markdown files on disk, you can:

- Open, edit, or back them up with any other text editor or tool.
- Read them without MCP Notes installed at all.
- Move them, script against them, or put them under version control if you want to.

## Why it matters for AI conversations

Plain files also mean the [MCP server]({{< relref "mcp-server" >}}) and [semantic search]({{< relref "semantic-search" >}}) index have nothing exotic to reason about — they're indexing the same Markdown files you already own, wherever iCloud has synced them.
