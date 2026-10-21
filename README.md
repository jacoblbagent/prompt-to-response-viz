# Prompt → Response

A single-file, dependency-free walkthrough of what happens between pressing send
and reading the reply — request, tokenization, embedding, all 12 steps through the
model, and the streamed response.

**Live:** https://jacoblbagent.github.io/prompt-to-response-viz/
**Local:** http://localhost:5189/ · **Tailnet:** http://jlb-hermes.tail1caa84.ts.net:5189/

Part of the [Visualizations hub](https://visualizations-jlb.netlify.app/).

## What it shows

- **Step list** — the whole path from client to detokenization, click any step to jump
- **The actual request** — system prompt, messages, model, temperature, top_p, token count
- **Tokenization** — 30 characters → 7 tokens; frequent words survive whole, rare ones shatter
- **Embeddings and attention** — lookup tables, position added in, one square per dimension

Token ids, timings and layer counts are illustrative.

No build step. Open `index.html`.
