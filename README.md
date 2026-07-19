# Cyples Engineering Methodology (CEM)

The **Cyples Engineering Methodology (CEM)** is a technology-independent engineering framework for designing, developing, and maintaining projects of any size. Its central philosophy is that a project's architecture should define and drive the project, rather than simply document it.

CEM separates the **concept** of a system from its **implementation**, allowing a single concept to support multiple hardware, software, and mechanical realizations while preserving its original intent.

Projects developed using CEM begin with a **Vision**, progress through **Concept Architecture** and **System Architecture**, and use those artifacts to drive implementation, documentation, testing, project management, and future evolution.

This repository documents the methodology, its guiding principles, reusable templates, and practical examples. It serves as the foundation for engineering projects developed under the Information & Imagination organization.

## Why architecture-first?

Writers roughly split into two camps. Some write "seat of the pants" — they discover the story by drafting it, and if a scene turns out wrong, the fix is cheap: rewrite the paragraph. Others outline first, because for them discovering the story's shape mid-draft is expensive — wasted chapters, plot holes, character arcs that have to be unwound and rebuilt. For engineers, discovering structural problems late is dramatically more expensive.

Engineering projects — especially ones that mix hardware and software — don't get the pantser's cheap revisions. You can't "rewrite the paragraph" once a part has been milled or a board has been fabricated. CEM exists for exactly that reason: it's an outline for the thing you're about to build, written because discovering structure after money's been spent is far more expensive than discovering it on paper first.

That said, even a committed outliner still amends the outline as they learn things while drafting — they don't rewrite it from scratch every time a scene reveals something new. CEM works the same way: small discoveries get folded into the existing documents in place; a genuine structural rethink becomes a new, versioned draft rather than an edit to the old one.

```
Vision
    │
    ▼
Concept Architecture
    │
    ▼
Requirements
    │
    ▼
Decision Records
    │
    ▼
System Architecture
    │
    ▼
Generated Project
```

## About

A practical engineering methodology that separates concept from implementation and uses architecture to drive project execution.
