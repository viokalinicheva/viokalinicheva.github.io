# Violetta Kalinicheva — Applied Data Science Portfolio

A lightweight, accessible, one-page public portfolio for data scientist and applied machine learning opportunities. The site uses plain HTML and CSS with no build step, external fonts, tracking, or runtime dependencies.

- Portfolio: https://viokalinicheva.github.io/
- Site repository: https://github.com/viokalinicheva/viokalinicheva.github.io

## Content

- A complete About section describing analytical interests and working approach.
- Two featured projects with their question, method, verified result, limitations, public repository, executed notebook, and complete README.
- Eight additional selected analyses in an explicitly in-preparation section. These are not represented as reproducible public releases and have no invented repository links.
- Contact through the approved GitHub profile only.

## Files

```text
.
├── index.html
├── styles.css
├── .nojekyll
└── README.md
```

Publish these files at the repository root. `.nojekyll` keeps the site buildless on GitHub Pages. Configure GitHub Pages to deploy `main` from `/ (root)`.

## Local preview

```bash
python3 -m http.server 8000 --bind 127.0.0.1
```

Open `http://127.0.0.1:8000/` from this folder. No package installation is required.

## Evidence and status

The featured analyses were clean-run verified on **October 2, 2026**. The site preparation on October 28, 2026 does not constitute a new analytical rerun. Claims were transcribed from the current public-project README versions, not the earlier draft documents.

### Beyond the Job Title

- Repository: https://github.com/viokalinicheva/dsc680-project1-onet-career-map
- Evidence reference commit: `7d87c86bfaa723c1bddcb8172d0b96d9e669d6a2`
- 882 occupations and 109 standardized features; 46.3% variation in two principal components, 14 components for 80%; silhouette 0.209.
- Nearest-ten overlap: 9/10 when retaining flagged estimates; 8/10 for cosine distance; 8/10 with equal domain weighting. The CSS bars share a ten-occupation denominator.
- Occupational description is not an individual assessment or hiring prediction.

### Employee Attrition Early Warning

- Repository: https://github.com/viokalinicheva/employee-attrition-early-warning
- Evidence reference commit: `5855392ebfd0318fb4555f8fe357bc5702048d02`
- Fictional data, 1,470 records; training/test split 1,176/294; test ROC-AUC 0.802, PR-AUC 0.557.
- At threshold 0.50: 30 true alerts, 17 missed departures, 56 false alerts. Thus, 47 actual departures and 86 alerts. Recall is 30/47 = 63.8%; precision is 30/86 = 34.9% (rounded to one decimal place).
- The two stacked bars intentionally have **different denominators**, stated above each bar and in the caption. They are not a whole-population comparison.
- Do not present fictional predictive associations as causal findings or deployment validation.

## Maintenance checklist

1. Preserve professional titles and decision-oriented summaries; avoid unverified employment or outcome claims.
2. Check every featured metric against the notebook and README before revising it.
3. Verify repository, notebook, and README links after any rename or branch change.
4. Promote an in-preparation project only after source/license review, neutral packaging, complete documentation, and a clean reproducibility run. Replace its pending status with the actual verification date.
5. Keep raw or licensed inputs, private files, credentials, local paths, and unrelated materials out of this repository.
6. Retest keyboard navigation, the expandable project list, anchor links, contrast, and horizontal overflow at desktop and mobile widths.
7. Keep contact limited to the GitHub profile unless additional public contact information is explicitly approved.

## Data attribution

O*NET analysis descriptions refer to the O*NET 31.0 database from the U.S. Department of Labor, Employment and Training Administration, used under CC BY 4.0. O*NET is a trademark of USDOL/ETA. The analysis includes filtering, standardization, PCA, ranking, and clustering and is not endorsed by USDOL/ETA. See the featured project README for complete attribution and the [official database license](https://www.onetcenter.org/license_db.html).

The attrition analysis uses the fictional IBM HR Analytics Employee Attrition and Performance dataset distributed on Kaggle. The featured repository links to the authoritative source and does not redistribute the CSV.
