# Lab 5 — Applied Data Distributions (DSARM 1)

This repo mirrors Labs 3–4 but swaps in **Lab5.ipynb** and the shared **L4L5dataset.csv**.  
It is **Codespaces-ready**, includes a devcontainer that auto-installs **GitHub Copilot** and key VS Code extensions, and keeps notebook diffs clean.

## Contents
- `Lab5.ipynb` — notebook covering: QQ plots & Normality, decile plot interpretation, Binomial “at least one”, Poisson rates→counts.
- `L4L5dataset.csv` — working dataset shared across Labs 4 & 5.
- `.devcontainer/devcontainer.json` — Codespaces config (Python + extensions incl. Copilot).
- `.vscode/extensions.json` — extension recommendations (for local VS Code).
- `requirements.txt` — lightweight scientific Python + Jupyter stack.
- `.gitattributes` — enables clean notebook diffs with `nbstripout`.
- `.gitignore` — ignores checkpoints, OS clutter, and exported images.
- `figures/` — export images here (kept with `.gitkeep`, images ignored by Git).

## Quick start (GitHub Codespaces)
1. Click the green **Code** button → **Open with Codespaces**.
2. The container builds and runs `pip install -r requirements.txt` automatically.
3. Open **`Lab5.ipynb`** and run cells **top → bottom**.
4. Save figures to the `./figures/` folder, e.g.:
   ```python
   plt.savefig("figures/decile_plot.png", dpi=150, bbox_inches="tight")
   ```
5. **Commit & Push** your work so it persists:
   ```bash
   git add -A && git commit -m "Lab 5 work" && git push
   ```

## Notes
- **Clean diffs:** `nbstripout` strips output on commit; you can also run `nbstripout --install` locally if needed.
- **Reproducibility:** Restart kernel and run all before exporting figures.
- **Troubleshooting:** If imports fail, rerun `pip install -r requirements.txt`. If saves fail, ensure `figures/` exists.

---
© 2025 DSARM. Educational use only.
