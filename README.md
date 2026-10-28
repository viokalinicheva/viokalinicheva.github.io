# Violetta Kalinicheva — Applied Data Science Portfolio

A lightweight, accessible, one-page public portfolio for data scientist and applied machine learning opportunities. The site uses plain HTML and CSS with no build step, external fonts, tracking, or runtime dependencies.

- Portfolio: https://viokalinicheva.github.io/
- Site repository: https://github.com/viokalinicheva/viokalinicheva.github.io

## Content

- A complete About section describing analytical interests and working approach.
- Ten project case studies with a practical question, method, verified finding, decision boundary, repository link, executed notebook, and complete README.
- A keyboard-accessible project directory so readers can jump directly to a domain or method without reading the entire page.
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

Projects 01–02 were clean-run verified on **October 2, 2026**. Projects 03–10 were independently rerun from raw inputs on **October 28, 2026**, with source and dependency checks documented in their release evidence. The site update does not change those analytical verification dates. Homepage findings were checked against the completed project README files and actual validation records; no result is inferred from the original saved notebook alone.

The initial two project presentations and their visual evidence panels are retained. The eight additional projects use a compact question → method → finding → decision-boundary structure, with responsive layouts and direct repository/notebook/README links. No raw project data are copied into this website repository. Repository URLs must be verified after the corresponding releases are published and before the homepage is deployed.

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

### Completed projects 03–10

| Project repository | Homepage evidence | Boundary kept visible |
|---|---|---|
| [MovieLens recommender](https://github.com/viokalinicheva/movielens-recommender) | 32,000,204 ratings; validation-selected 64 factors; supported-test HR@10 8.99% versus 3.16%, 9,769 cases | Transductive held-interaction benchmark; not a prospective global-time evaluation |
| [TSA complaint quality](https://github.com/viokalinicheva/tsa-complaint-quality) | 1,021,281 complaints; 42.9% unassigned airport and 47.4% imputed/ambiguous subcategory | Counts without passenger denominators are not airport-performance rates |
| [Childcare affordability](https://github.com/viokalinicheva/childcare-affordability) | Fixed panel of 1,273 counties; household-weighted county ratio 18.52% → 19.92%, 2008–2018 | Historical county price-to-income ratios, not current family spending or a national median |
| [Vehicle theft early warning](https://github.com/viokalinicheva/vehicle-theft-early-warning) | Nine complete cities: 2,315 → 12,592 reported Kia/Hyundai thefts, 2021–2022 | Not per-vehicle risk, a national rate, a causal social-media effect, or a deployed alert |
| [Retail sales forecasting](https://github.com/viokalinicheva/retail-sales-forecasting) | 354 months; test RMSE 66,433 million nominal USD; all twelve months underestimated | Fixed July 2021 revision vintage; retrospective, not real-time historical forecasting |
| [Lottery pattern trap](https://github.com/viokalinicheva/lottery-pattern-trap) | 17,472 source drawings; three snapshot marginal-frequency p-values 0.460/0.475/0.503; current-reference Powerball 0.407 | No rejection is not proof of randomness or predictive power; source versions are distinct |
| [White House visitor operations](https://github.com/viokalinicheva/white-house-visitor-operations) | 1,207,458 source rows; 1,202 within-release duplicates removed; 1,206,256 disclosed records | Appointment-access records are not actual attendance, political influence, or staffing hours |
| [Netflix content strategy](https://github.com/viokalinicheva/netflix-content-strategy) | 741 title-season units across 44 common views-era weeks; 2.97 versus 1.98 observed chart weeks | Chart persistence is not retention, unique viewers, profitability, or a causal language effect |

The source and evaluation limitations are substantive parts of these projects, not unfinished project placeholders. Historical dates and explicit denominators should remain with each figure or result when copied elsewhere. The Lottery repository maintains native Tableau validation separately from its independently executed Python story; the homepage does not infer workbook rendering from Python checks.

## Maintenance checklist

1. Preserve professional titles and decision-oriented summaries; avoid unverified employment or outcome claims.
2. Check every featured metric against the notebook and README before revising it.
3. Verify repository, notebook, and README links after any rename or branch change.
4. Change a project result only after source/license review, a clean reproducibility run, and reconciliation with the published release evidence. Record its actual verification date rather than refreshing a date for a cosmetic site edit.
5. Keep raw or licensed inputs, private files, credentials, local paths, and unrelated materials out of this repository.
6. Retest keyboard navigation, all ten project-directory links, repository/notebook/README links, contrast, and horizontal overflow at desktop and mobile widths. Check long project titles and the three-column desktop notes after any content change.
7. Keep contact limited to the GitHub profile unless additional public contact information is explicitly approved.

## Data attribution

O*NET analysis descriptions refer to the O*NET 31.0 database from the U.S. Department of Labor, Employment and Training Administration, used under CC BY 4.0. O*NET is a trademark of USDOL/ETA. The analysis includes filtering, standardization, PCA, ranking, and clustering and is not endorsed by USDOL/ETA. See the featured project README for complete attribution and the [official database license](https://www.onetcenter.org/license_db.html).

The attrition analysis uses the fictional IBM HR Analytics Employee Attrition and Performance dataset distributed on Kaggle. The featured repository links to the authoritative source and does not redistribute the CSV.

Projects 03–10 identify their full primary sources, permissions, historical versions, and acquisition instructions in their repository READMEs. These include GroupLens MovieLens research/noncommercial terms; Data Liberation Project–standardized TSA data and attribution/share-alike conditions; Department of Labor childcare data; USAFacts/VICE vehicle-theft sources; original Census retail archives; New York State Open Data lottery snapshots and official-record disclaimers; official White House archive disclosure policies; and Netflix's chart methodology. Project-level data conditions are not replaced by this site's presentation. The site includes summaries only, with no raw data downloads, visitor records, third-party tracking, external fonts, forms, or additional personal contact information.
