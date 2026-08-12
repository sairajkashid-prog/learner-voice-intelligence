# 🗣️ Learner Voice Intelligence — What Makes Training Succeed or Fail

**What should training content do more of — and avoid?**
This project analyses **107,018 real learner reviews** from Coursera to extract what makes online courses succeed or fail, then turns those findings into a concrete **content-quality playbook** for a learning company.

> Built by **Sairaj Sandip Kashid** for the TechnoEdge Learning Services — *Solution Expert Intern* application.

---

## 🔥 The problem it solves

A training company that doesn't listen to learners ships content that drifts. But reading 107k reviews by hand is impossible. This dashboard distills them into:

- **6 things learners love** (replicate these)
- **7 things learners hate** (avoid these)
- **5 data-backed design rules**, each tied to a measured pain point

## 📈 Key findings (from real data)

- **90.9%** of reviews are positive (4–5★); average rating **4.58★** — online learning generally delights.
- The **#1 complaint** isn't content quality — it's **assignments & peer review** (25.7% of negative reviews).
- **Unhappy learners write 2× longer reviews** (57–62 words) than happy ones (25 words) — the richest, most actionable feedback hides in the negative tail.
- Top praise themes: *highly recommend* (30%), *engaging & enjoyable* (26%), *practical & hands-on* (16%).

## 📊 What's inside (4 interactive views)

| Tab | What it shows |
|-----|---------------|
| **Sentiment** | Rating distribution (1–5★), positive/neutral/negative split, the "complaint-length" signal |
| **What Works** | Positive-theme frequency bars + real review excerpts + "DO more of this" rules |
| **What Hurts** | Negative-theme frequency bars + real review excerpts (the avoid-list) |
| **Action Plan** | A ready-to-use content-quality playbook + full methodology (honest about limitations) |

Every chart has **hover tooltips**; every theme comes with a **real review excerpt**.

## 🧠 How themes were extracted (transparent methodology)

1. **Data:** 107,018 public Coursera reviews, each with a 1–5★ label + free-text comment.
2. **Sentiment:** ratings bucketed → positive (4–5★), neutral (3★), negative (1–2★).
3. **Themes:** lexicon-based keyword matching against curated positive & negative word-lists (e.g. *"outdated"*, *"peer review"*, *"clear"*, *"practical"*), counted per review.
4. **Limitation (stated honestly):** keyword matching catches explicit mentions; nuanced sarcasm may be missed. A production version would add NLP/embedding classification.

*A Solution Expert shows their working — not just magic numbers.*

## 📦 Real data source

| Source | Records | Fields |
|--------|---------|--------|
| Coursera reviews dataset | 107,018 reviews | review text, 1–5 star rating |

All figures computed in Python from the raw CSV.

## 🛠️ How it's built

- **Pure HTML + CSS + vanilla JavaScript** — zero external libraries, zero CDNs.
- **Custom hand-drawn SVG charts** (bar, donut, line) with a warm terracotta/amber palette.
- Self-contained `index.html` — open directly or host on GitHub Pages.
- Data processing: `../process_data.py` (Python stdlib only).

## ▶️ Run it

```bash
open index.html
# or
python3 -m http.server 8000
```

## 💡 Why this impresses

It turns unstructured learner feedback into **actionable product rules** — the core of "analyse → recommend → document" that a Solution Expert does daily. And it's directly relevant to TechnoEdge's training-content business.

---
*Warm-coloured · hand-crafted · real data · zero dependencies*
