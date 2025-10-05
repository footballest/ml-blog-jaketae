# ML Blog – Jake Tae Replications

This repository hosts my hands-on implementations and notes based on posts from **Jake Tae’s blog**. I’m building everything in **Google Colab** and publishing write-ups via **GitHub Pages**.

## Folder structure
```
.
├── docs/                # GitHub Pages site (Settings → Pages → Branch: main, Folder: /docs)
│   └── index.md
├── notebooks/           # Colab notebooks (one per post)
├── data/                # Datasets (do NOT commit large files)
└── images/              # Figures used by notebooks and docs
```
> Tip: create `data/` and `images/` when you need them.

## Workflow (short)
1. Create/clone this repo.
2. In Colab, open `notebooks/template.ipynb` → File → **Save a copy in GitHub** to this repo.
3. Update `docs/index.md` with a new row for your notebook (use the “Open in Colab” badge link below).
4. Commit & push. GitHub Pages will publish `/docs` automatically.

## Open in Colab badge (replace placeholders)
```markdown
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](
https://colab.research.google.com/github/<your-username>/<your-repo>/blob/main/notebooks/<file>.ipynb)
```

## Mount Drive in Colab
```python
from google.colab import drive
drive.mount('/content/drive')
BASE_DIR = '/content/drive/MyDrive/ml-blog'
!mkdir -p "$BASE_DIR"/{data,images,artifacts}
```

## Publish checklist
- [ ] Notebook runs end-to-end
- [ ] Small datasets only (or download code)
- [ ] Add screenshots/figures to `images/` (if needed)
- [ ] Add entry on `docs/index.md`
- [ ] Push to `main`
