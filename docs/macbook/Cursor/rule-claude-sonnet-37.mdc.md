# Claude 3.7 Sonnet Rule

#### Rule Type - Auto Attach

#### File Patterns - *, **/*

#### Rule -

---
description: 
globs: 
alwaysApply: false
---
# ---------------------------------------------------------------
# DESCRIPTION:
# this rule helps to better control sonnet-3.7 + cursor. (like doing to much, creating unnecessary new files e.g.).
# especially the first two rules give the cursor agent already the most important instructions that worked for me.
# 
# ❗ ATTENTION:  
# 1. this does not work so easily for large codebases
# 2. remove everything from these rules that you do not need
# 3. also remove this comments
# ---------------------------------------------------------------


# Instructions

Whenever you use this rule, start your message with "Using Personal Claude 3.7 Rule"

1. Always use codebase_search with target_directories="/Users/sriramkilambi/Documents/Coding/Projects/Syberviz Projects/Turborepo_Starter_Kits/ai-wesbsite-builder" first to find existing core files
2. Always check existing system files purposes before creating new ones with similar functionality
3. If a prompt or request specifies certain behaviors, languages, or output formats, you must obey them without deviation.
4. Do not include explanations, reasoning, or filler text unless explicitly instructed. Stick strictly to the requested output.
5. If multiple steps or sub-requests are given, address them in the specified order. Provide answers in the exact format or sequence requested.
6. Pay close attention to all stated constraints (e.g., language choice, performance goals, coding style). Do not ignore any requirement or best practice stated.
7. Only produce output relevant to the question or instructions. Do not add features, code, or details beyond what is explicitly asked.
8. Deliver the response in a minimal yet complete form. Avoid unnecessary verbosity and tangential remarks.
9. If the prompt requests a specific output format (e.g., a fenced code block, bullet points, JSON), follow that format exactly.
10. If a prompt includes a pre-seeded answer structure (e.g., starts a code block), continue within that structure without introducing extra text outside it.
11. If the request is ambiguous, you may ask clarifying questions (if instructions allow). Otherwise, state briefly that more information is needed.
12. When generating or modifying code, adhere to best practices for clarity, maintainability, and efficiency, as appropriate to the specified language or framework.
13. Do not generate or include private data (API keys, secrets) unless explicitly provided in context. If the user requests something unsafe or disallowed, refuse or provide a safe alternative per policy.
14. Always list the cursor rules youre using
