---
title: "Wikilinks"
icon: "⛓"
weight: 30
summary: "Link notes together with [[Note Name]] and a force-directed graph view."
---

Type `[[Note Name]]` anywhere in a note and MCP Notes turns it into a link to that note, creating it automatically if it doesn't exist yet. It's the same shorthand used by most Markdown note apps, so importing existing notes just works.

## Seeing how notes connect

Every wikilink is also an edge in a force-directed graph view, so you can see clusters of related notes at a glance — trip notes linked to packing lists, project notes linked to meeting notes, and so on — instead of relying on folders alone.

## Why it matters for AI conversations

Wikilinks give the [MCP server]({{< relref "mcp-server.md" >}}) a way to follow context beyond a single note. If the note that answers Claude's query links to another note with more detail, that connection is there to follow — the same way you would, reading it yourself.
