# Terputer: Cinnamaldehyde Variation in Cinnamon

Evidence-scoping package for comparing cinnamaldehyde across cinnamon types. The source repository contains narrative ranges but no sample-level assay dataset or machine-readable citation-level measurements. Accordingly this package records claims and research gaps; it does not treat those ranges as measured study results.

## Run

Install `requirements.txt` and open `notebooks/analysis.ipynb`. Notebook checks the scope of the source narrative and keeps reported ranges distinct from empirical data.


## Terpedia access

The optional client in `src/terpedia_access.py` calls the Terpedia Knowledge API at `/v1/tabular/search`. It reads `TERPEDIA_KNOWLEDGE_API_KEY` and `TERPEDIA_KB_API_URL` from the process environment and sends the key in the `x-knowledge-key` header. Copy `.env.example` as a configuration reference, then provide the real key through a local secret manager, Codespaces secret, or authorized GitHub Actions secret. Never commit `.env` or print the key in notebook output.
