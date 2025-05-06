# LLM Sentiment‑Analysis Comparative Experiment

> ChatGPT (gpt‑3.5‑turbo) · Llama 3.2 (8 B, Ollama) · DeepSeek‑R1 1.5 B (Ollama)

![Comparison](./ChatGPT%20vs.%20Llama3.2%20vs.%20DeepSeek%20image.png)

### 📌 Goal
Measure accuracy, qualitative depth, and latency when the **same financial‑news feed** is processed by three different LLM stacks. 
The financial news will be sourced from feeds.finance.yahoo.com.

### 🔧 Tech stack
| Layer | Tool |
|-------|------|
| Scraper | `feedparser` + `BeautifulSoup` |
| Local models | `Ollama` (Llama 3.2 Q4_0 · DeepSeek‑R1 1.5 B Q4_0) |
| Cloud model | OpenAI `gpt‑3.5‑turbo` |

### 🗂 Findings

![Comparison Results](./Comparison%20Results.JPG)

### 📝 Take‑aways

- For quick dashboards, ChatGPT 3.5 offers the best latency‑to‑cost ratio.
- DeepSeek returns richer narratives yet is still faster than Llama 3.2 on 8 GB RAM.
- Local models shine where privacy is key or token limits blow up costs.
