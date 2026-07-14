# Smog Alert Baseline Survey — Dashboard

Password-protected field-monitoring dashboard for the **Smog Alert Baseline Survey** (Shalamar Tehsil, Lahore), run by **Research Solutions (M&A Research Solutions LLC)** — www.rs.org.pk

- **Live URL:** https://smogalertbaselinesurvey.rs.org.pk
- **Fallback URL:** https://jawadahmad-star.github.io/Smog-Alert-Baseline-Survey-Dashboard/

## Contents

| File | Purpose |
|---|---|
| `index.html` | The complete dashboard (self-contained; charts via Chart.js CDN) |
| `CNAME` | Custom-domain binding for GitHub Pages |

The dashboard contains **aggregated statistics only** — no respondent-level data, phone numbers, GPS points or other PII are published in this repository.

## Updating the dashboard

The dashboard is regenerated locally with `build_dashboard.py` (kept outside this repo alongside the raw SurveyCTO exports):

```
python build_dashboard.py   # reads WIDE CSV + form + prefill, writes index.html
```

Then copy the fresh `index.html` here, commit and push — GitHub Pages redeploys automatically.
