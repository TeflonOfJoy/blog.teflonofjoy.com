---
title: "Google: Big Sleep first real-world vulnerability discovered"
date: 2024-11-11
draft: false
cover:
    image: posts/LLM(1800)_Krot_Studio_Alamy.webp
    alt: LLM(1800)_Krot_Studio_Alamy
    caption: "Source: krot studio via almy stock photo"
description: "A research tool by the company found a vulnerability in the SQLite open source database, demonstrating the defensive potential for using LLMs to find vulnerabilities in code before it's publicly released."
tags: ["ai", "cybersecurity"]
showToc: true
TocOpen: true
---

# Introduction
A while ago Project Zero, the vulnerability research of Google, began evaluating the offensive capabilities of Large Language Models. That then evolved into Project Naptime a framework for LLM assisted vulnerability research, which eventually merged with Google's Deep Mind in a joint collaborative project "Big Sleep".

# Big Sleep
Big Sleep discovered an exploitable stack buffer underflow in SQLite, a widely used open source database engine.

Specifically, Big Sleep discovered a pattern in the code of a publicly released version of SQLite that creates a potential edge case that needs to be handled by all code that uses the field, the researchers noted. A function in the code failed to correctly handle the edge case, "resulting in a write into a stack buffer with a negative index when handling a query with a constraint on the 'rowid' column," thus creating an exploitable flaw, according to the post.

Google reported the bug to SQLite developers in early October. They fixed it on the same day and before it appeared in an official release of the database, so users were not affected.

