# Data and reproducibility storage

No research data have been acquired yet.

Keep the following in GitHub:
- Acquisition manifests and data dictionaries.
- Small, redistributable derived tables and their generation code.
- Quality-control summaries, figures, diagnostic presentations and run metadata.
- Exact product/version citations, processing settings, checksums and persistent download references.

Do not commit global raw swath archives, credentials, API keys or restricted/licensed data. Large redistributable raw and processed datasets should go to an appropriate research-data archive such as Zenodo or an institution-approved store, with checksums and persistent links in this repository. This preserves reproducibility without exceeding GitHub limits. A data-provider license may require readers to obtain an input from its official source.

The manifest template contains a header only. Each acquired object needs its own honest status; a planned URL is not a successful download.

Recommended local organization:
- data/raw/: original provider files, immutable.
- data/interim/: collocated/subset intermediates.
- data/processed/: compact analysis-ready outputs, versioned or archived as appropriate.
- results/: generated figures/tables and diagnostic reports.
- notebooks/ and src/: future analysis code, created after data access and pilot specifications are known.

Every future run should record the Git commit, software environment, input manifest/checksums, command or notebook execution order, filtering counts, random seeds where relevant, and output checksums. Store original and adjusted/null/sensitivity results; never replace unfavorable results with a selected successful subset.
