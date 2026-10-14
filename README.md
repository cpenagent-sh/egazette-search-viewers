# eGazette search viewers

Browsable results of full-text searches on egazette.gov.in. Each document is shown with its metadata next to its PDF.

- `gst/`: "Goods and Services Tax", 811 documents
- `fem/`: "Foreign Exchange Management", 410 documents
- `data/`: the same results as CSV

Every PDF link was checked to return a real PDF. Every document is matched to the workbench by its eGazette PDF URL (one by Gazette ID where the year folder differs). No PDFs are hosted in this repo; the viewers load the stored copies and link to the eGazette originals.

Rebuild: `build_viewer.py` and `template.html` in the egazette_search_viewers workspace; searches come from `egazette_parallel_search.py` and `finalize_rows.py`.
