# Digital Building Permits — System-of-Systems Toolkit

Interactive tools for understanding the **digital building permit (DBP)** as a *system of systems* — its six parts, the types of methods within each, how they connect, and the research literature (443 papers, 1978–2026) behind them.

## Open the tools

Once this repository is published with **GitHub Pages** (see below), the tools open in any browser:

| Tool | File | What it does |
|---|---|---|
| **Landing page** | `index.html` | Hub linking to everything |
| **System-of-Systems Framework** | `dbp_sos_framework.html` | Concept · The Parts · Relationships · Type Graph · Bicycle |
| **Literature Explorer** | `dbp_literature_explorer.html` | Dashboard (keyword/year filters) + knowledge graph |
| **Master corpus spreadsheet** | `DBP_master_corpus.xlsx` | All 443 papers with IDs, metadata, parts & types |

Every HTML file is **self-contained** (all code and data inlined) — no build step, no dependencies, works offline.

## The six parts

**N1 Data and Models · N2 Tools and Approaches · N3 Regulations and Compliance · N4 Governance and Processes · N5 People and Capabilities · N6 Purposes and Values.**
Each part is a cluster of **types** (distinct methods/strategies, each with requirements + solutions → enablers + challenges). Papers carry a stable ID (**P001–P443**) shared across every tool and the spreadsheet.

---

## How to publish on GitHub Pages

### Easiest — no command line (web browser only)

1. Go to <https://github.com/new> and create a repository (e.g. `dbp-toolkit`). Set it **Public**. Click **Create repository**.
2. On the new repo page click **uploading an existing file** (or **Add file → Upload files**).
3. Drag in all the files from this folder: `index.html`, `dbp_sos_framework.html`, `dbp_literature_explorer.html`, `dbp_sos_bicycle.html`, `DBP_master_corpus.xlsx`, `README.md`. Click **Commit changes**.
4. Go to **Settings → Pages**. Under *Build and deployment → Source* choose **Deploy from a branch**, pick branch **main** and folder **/ (root)**, then **Save**.
5. Wait ~1 minute. The page appears at:
   `https://<your-username>.github.io/dbp-toolkit/`
   Share that link — anyone can open the tools.

### Command line (if you use git)

```bash
cd path/to/this/folder
git init
git add .
git commit -m "DBP system-of-systems toolkit"
git branch -M main
git remote add origin https://github.com/<your-username>/dbp-toolkit.git
git push -u origin main
```

Then enable Pages as in step 4 above.

### Notes

- **Public repo** = anyone with the link can open the tools (free). GitHub Pages on a **private** repo requires a paid plan.
- Individual file size is fine (largest is ~1.2 MB, well under GitHub's 100 MB limit).
- To update a tool later, replace the file in the repo (drag-and-drop **Upload files** again, or `git push`) — the Pages site refreshes automatically.
