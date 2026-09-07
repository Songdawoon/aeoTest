# AI Citation Experiment #001

Target URL: https://aeo-test-hazel.vercel.app/

## Day 0 — 2026-08-27
- Public deployment: complete
- Google Search Console URL-prefix property: verified
- Google live URL test: passed (URL can be indexed)
- Dataset structured data: valid item detected
- sitemap.xml: discovered
- Google indexing request: submitted by site owner
- robots.txt: Googlebot, OAI-SearchBot, PerplexityBot allowed
- canonical: production URL
- Article + Dataset JSON-LD: deployed
- General web-search visibility at baseline: 0

## Day 1 — 2026-08-28 13:29 KST
### Discovery checks
- Exact domain search: no public search result found
- `site:aeo-test-hazel.vercel.app`: no result found in available web-search indexes
- Exact experiment phrase `AI Citation Experiment #001`: target page not found
- Domain-restricted queries for `2026 홈페이지 제작비용`, `회사소개 홈페이지 제작비용`, and `5~10페이지 기업 홈페이지 제작비용`: target page not found

### Generic-query citation/search baseline
Queries tested:
1. `2026년 회사소개 홈페이지 제작 비용 보통 얼마`
2. `5~10페이지 기업 홈페이지 제작비용`
3. `국내 홈페이지 제작비용 여러 업체 비교`
4. `홈페이지 제작 업체마다 견적 차이 이유`

Observed competing sources included IDC.KR, Webbird, Adall, WintzLab, Edstudio, 모두의사이트, Infoly, Magneticsoft and others. The target Vercel page was not returned as a source.

### Search Console status captured by site owner
- Google status: `URL이 Google에 등록되어 있지 않음`
- Indexing state: `크롤링됨 - 현재 색인이 생성되지 않음`
- Last crawl: 2026-08-27 18:00:30 KST
- Crawler: Googlebot Smartphone
- Crawl allowed: Yes
- Page fetch: Successful
- Indexing allowed: Yes
- User-declared canonical: https://aeo-test-hazel.vercel.app/
- Google-selected canonical: Inspected URL
- Sitemap: https://aeo-test-hazel.vercel.app/sitemap.xml

### Day 1 status
- Google has successfully crawled the page
- Technical crawl/index eligibility checks: passed
- Google chose not to index the page yet
- Public search discovery: not yet observed
- ChatGPT/web-search source retrieval: not yet observed
- AI citation: 0 observed

### Interpretation
This has progressed from discovery to an actual Google crawl. The current bottleneck is no longer crawling or canonical configuration; it is Google's decision not to include the page in the index yet.

## V2 — 2026-09-07
### Variable changed: content depth / source breadth only
To avoid mixing too many variables at once, the site remains a single primary HTML page. We changed the evidence quality and depth before testing site-page-count effects.

Changes:
- Expanded source set from 5 to 30 public sources
- 24 direct vendor pricing sources + 6 vendor/market guides
- Added the original source URL beside every row
- Added `website-cost-dataset-2026.csv` as downloadable raw data
- Added collection date, source type, scope, price, notes, methodology and limitations
- Updated Article/Dataset structured data and modified date
- Kept the canonical URL unchanged

### Hypothesis
If the reason for `Crawled - currently not indexed` is insufficient originality/value rather than a technical issue, increasing source breadth, transparency and reusability of the dataset may cause Google to re-evaluate the page after the next crawl.

### Next checkpoint
1. Confirm Vercel deployed commit `7aff101849ce21450d995f1add1546607afa1ea6`
2. Request/observe a new crawl
3. Record new last-crawl time and coverage state
4. Do not add extra site pages until this V2 result is measured
5. If still not indexed, test a multi-page topical structure as V3
