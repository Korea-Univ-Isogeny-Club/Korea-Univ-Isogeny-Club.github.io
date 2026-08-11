# Korea University Isogeny Club

An open knowledge base for elliptic curves, isogenies, and post-quantum cryptography, built with MkDocs Material.

## Local development

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve
```

Open <http://127.0.0.1:8000> in a browser. GitHub Actions builds and deploys the site to GitHub Pages on every push to `main` or `master`.
