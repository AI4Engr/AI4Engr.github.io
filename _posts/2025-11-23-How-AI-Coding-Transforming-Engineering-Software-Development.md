---
layout: post            
title: "How AI Coding Is Transforming Engineering Software Development"
date: 2025-11-23 10:00 -0500
categories: [notes]     # optional: hierarchical taxonomy
tags: [development]  # optional: free-form labels
# excerpt: "A quick start to posting with Jekyll."  # optional
published: true         # set false to hide
---

Artificial intelligence has entered nearly every industry, but its impact on **engineering software development** is especially profound. Over the past several months, I’ve worked extensively with Claude Code and OpenAI’s coding tools. Although I didn’t apply them to a commercial engineering product, I did test Claude Code on the open-source FREPpv finite element project ([https://github.com/sanjayg0/feappv](https://github.com/sanjayg0/feappv)). Remarkably, it was able to refactor the entire codebase into C++ -- a job that would normally take a team months.

The tools weren’t perfect; they still needed my knowledge of finite element methods to ensure technical correctness. But the productivity boost was impossible to ignore.

After months of real use, my conclusion is clear: **AI coding is mature enough to dramatically accelerate engineering software development—by 6× to 15× in practice, including testing and documentation.**

And this is just the beginning.

---

## **Why AI Works: The Prerequisite of Domain Knowledge**

Despite its power, AI coding is not a replacement for engineering judgment. Before leaning heavily on AI tools, you must have:

* Solid domain knowledge (e.g., finite element analysis)
* Strong understanding of engineering workflows
* The ability to validate AI-generated algorithms and assumptions

For example, generating a 2D structural drawing requires knowing *what information must appear on the drawing*. AI will follow instructions but cannot choose engineering requirements for you.

Version control tools like Git are essential to keep work organized, revert incorrect AI suggestions, and safely iterate.

---

## **Practical Recommendations for AI Coding Today**

### 🔧 **Best AI Coding Tools**

* **Claude Code** – excellent at refactoring and code comprehension
* **OpenAI Codex / GPT-based coding** – powerful for generation, transformation, and documentation

I’ve tried many alternatives but consistently returned to these two.

### 🖥️ **Recommended IDEs**

* **VS Code**
* **Cursor**
* **Augment** – a plugin, but surprisingly more capable than many standalone AI IDEs

### ⚙️ **Optional Enhancements**

* Configure **MCPs (Model Context Protocol)** for deeper integration
* Use automated testing frameworks to confirm correctness
* Rely on GitHub/GitLab workflows to track large AI-driven code changes

---

## **How AI Affects Different Roles in Engineering Software Companies**

### 👑 **CEO / CTO**

Executives stand to benefit enormously. They combine:

* domain expertise
* strategic vision
* understanding of market needs

With AI coding, they can rapidly explore new product directions, validate technical approaches, and remove roadblocks.

The challenge is adoption—many leaders don’t want to learn AI tools. But the reality is simple:

> **Ignoring AI is no longer an option. Competitors who embrace it will move faster, cheaper, and smarter.**

---

### 👨‍💻 **Developers**

For engineers with:

* 5+ years of coding experience
* solid physical stamina for long-term work
* domain expertise in structural/mechanical/civil engineering

AI coding can boost productivity **6× to 15×**.

**Advanced degrees** and **Professional Licenses** only increase the advantage.

However, the downside is unavoidable:
**We should expect a 30–80% reduction in programming staff** at engineering software companies. AI multiplies output, reducing the need for large development teams.

For developers without deep expertise, this is a serious risk. Recent layoffs (including tech giants like Amazon) show where the industry is heading.

**My recommendations:**

1. Work at an engineering/design firm first to build domain expertise.
2. Contribute to open-source engineering software to build credibility.

---

### 🧓 **Senior Engineers & Senior Developers**

AI reduces—not eliminates—the need for senior staff.
But the number of senior positions will shrink.

The best advice is simple: start planning for retirement early and maintain skills that AI cannot replace (e.g., architectural judgment, system design, regulatory understanding).

---

### 🛠️ **Support**

AI support—enhanced by RAG, embeddings, and contextual search—can significantly cut support costs. This area will likely face headcount reduction as well.

---

### 📣 **Sales & Marketing**

While I have limited insight here, AI is already widely used for:

* flyers and brochures
* ad campaigns
* automated customer messaging
* product videos

Expect AI to be a major force multiplier, not a replacement.

---

### 📊 **CFO & HR**

AI may reduce administrative overhead, especially in smaller companies where one person may handle HR, finance, and office operations.

---

## **Case Study: RISA and the Future Company Size**

Engineering software companies rarely disclose detailed structure, but we have reference data from this acquisition announcement:
[https://informedinfrastructure.com/34766/nemetschek-acquires-leading-us-software-provider-risa-for-structural-engineering/](https://informedinfrastructure.com/34766/nemetschek-acquires-leading-us-software-provider-risa-for-structural-engineering/)

In 2017, RISA reported:

* **24 employees**
* **$7.5M revenue**
* Founded in **1987**

Let’s estimate their staffing mix:

* 10 developers
* 6 sales/marketing
* 4 support
* CEO/CTO/CFO/HR

Over 30 years, this corresponds to roughly **300 man-years** of development time. Considering smaller early teams and software redesign cycles, **210 man-years** is a realistic estimate.

### **What does this look like in the AI era?**

Assume:

* product must be built in **5 years**
* AI boosts productivity **6×**

Then:

```
210 man-years / 6 (AI factor) / 5 years ≈ 7 developers needed
```

A modern AI-assisted competitor could operate with:

* **7 developers / CTO**
* **2 sales**
* **1 support**
* **CEO**
* **CFO**

Total: **~12 people**
That’s a **50% reduction in workforce**.

Once mature, maintenance might require just **4 developers**, reducing the company to **9 total employees**.

---

## **Conclusion: Embrace or Be Replaced**

In the era of AI, developing engineering software has become far easier than before. Even a small team of around fifteen people can now build powerful, full-scale engineering applications—provided the team has both strong engineering expertise and solid coding skills. With these capabilities, we can expect many new engineering software products to emerge in the coming years.

On the other hand, the outlook for existing companies is less optimistic. No one wants job losses, yet the reality is unavoidable:

* **AI coding is here.**
* **It accelerates engineering software development dramatically.**
* **Companies that adopt it will outpace those that don’t.**
* **Individuals who resist it will fall behind those who embrace it.**
---

**We don’t get to choose whether AI arrives.**

**We only get to choose whether we keep up.**













