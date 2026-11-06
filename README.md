# C10 Decision Lab — Interactive Decision Webpage

A complete, dependency-free static dashboard aligned with **Grade 10 Term 1, Criterion 10**.

## Open locally

Double-click `index.html`, or serve the directory with `python -m http.server 8000` and visit `http://localhost:8000/`.

## Features

- Add, edit or remove alternatives and states, including payoff values and probabilities.
- Automatic scorecard with Maximax, Maximin, Minimax Regret and EMV/Bayes.
- All ties are included when scores differ by at most `1e-9`.
- Sequential filtering with editable ranking criterion and top-N cutoff for each stage, preserving ties and fixed original scores.
- Elimination log and matching SVG flow diagram, automatically updated.
- Three preloaded examples, including a tie-test example.
- Invalid-input detection, normalization button, JSON import/export, local auto-save, copyable results, print styles, responsive layout.

## Required last step: real AI development conversation link

The teacher requires a **public link to the actual AI conversation**. An AI cannot automatically create your ChatGPT share URL. In ChatGPT, open the Share menu and create a public link. Then:

**Option A — best for a clean public URL:** Edit the line `const AI_CONVERSATION_URL = '';` inside `index.html` to hold your real public share URL, for example `const AI_CONVERSATION_URL = 'https://chatgpt.com/share/<YOUR-REAL-ID>';`, then deploy.

**Option B — no file editing:** On the deployed site, paste your real `https://chatgpt.com/share/...` URL into the *AI development conversation* section. Click **Set link**, then **Copy submission URL**. Share **that complete resulting URL**, including the `?ai=...` parameter, with your teacher. The public URL itself carries the shared conversation link, so the teacher sees a working hyperlink even from a fresh device.

Option A is safer if the teacher may strip URL query parameters.

## Deploy free using GitHub Pages

1. Sign in to https://github.com/ and create a **Public** repository, for example `c10-decision-lab`.
2. Click **Add file → Upload files**, and upload `index.html` to the repository root. Commit changes.
3. Open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**; select `main` and `/(root)`; save.
4. Once GitHub Pages is enabled, the webpage URL typically has this shape: `https://YOUR-USERNAME.github.io/c10-decision-lab/`. Open it to verify it is public.
5. Add your real AI conversation link using Option A (commit the updated HTML) or Option B (copy the parameterized submission URL). Verify the AI development link in a private browser window.
6. **Submit only the deployed webpage URL**. Do not submit the zip, HTML or a separate report.

## Accuracy notes

For maximization criteria, equal scores within 1e-9 are tied; for Minimax Regret, the smallest maximum regret wins. Regret is calculated against the best payoff in each **original** column; it is never recalculated after filtering. Filtering rankings are based on the original scorecard; stages retain all candidates tied at the top-N cutoff in original input order.
"# Interactive-Decision-Webpage" 
"# Interactive-Decision-Webpage" 
"# Interactive-Decision-Webpage" 
