<!--
  SEO META — not rendered on GitHub but indexed by crawlers
  --------------------------------------------------------
  keywords: EME International documentation, Prometheus Sypec docs, Echo SaaS, travel consultancy platform, import export Belgium Lebanon China, ESG reporting guide, accessible tourism, AI code quality platform
  description: Central documentation hub for E.M.E International SARL covering travel services, consultancy, trading operations, and in‑house SaaS products – Prometheus Sypec & Echo. Includes FAQs, how‑to guides, API references, and ESG disclosures.
-->
![logo](https://github.com/user-attachments/assets/30d35f55-1e7e-4d0b-b58a-16b145eb16fb)



# 📚 E.M.E International Documentation Repository

**The single source of truth for our travel‑tech, trading, and consultancy ecosystem.**

> This repo hosts the markdown/LaTeX sources that power <https://emetour.com/docs> and our internal Confluence knowledge base.

---

## ✨ What you’ll find here

| Section | Purpose |
|---------|---------|
| `guides/` | Step‑by‑step HOW TOs (bookings, VAT filings, deploying Echo) |
| `reference/` | API & CLI reference for Prometheus – Sypec, Echo, and internal micro‑services |
| `esg/` | ESG policy, KPI dictionary, latest sustainability report |
| `handbooks/` | HR, Ops, Accessibility, and D&I manuals |
| `faqs/` | Source of our public FAQ (see below) |

All content is written in **Markdown + Mermaid** and converted to HTML via MkDocs & GitHub Pages.

---

## 🚀 Quick Start (internal)

```bash
# clone via SSH – HTTPS is disabled for this private repo
$ git clone git@github.com:EME-International-BVBA/docs.git
$ cd docs
# launch live preview
$ mkdocs serve
```

Deployed documentation is automatically rebuilt on push to `main` by **GitHub Actions → Cloudflare Pages**.

---

## 🤔 Frequently Asked Questions {#faq}

> Below is a subset. Full list lives in [`faqs/`](faqs/) and is embedded in `schema.org` so Google can surface rich‑results.

<details>
<summary>What do “愛來” characters in the logo mean?</summary>
They are Chinese calligraphy for “Love comes” – capturing our mission of bringing cultures together.
</details>

<details>
<summary>Can I use Prometheus – Sypec to audit private GitLab repos?</summary>
Yes. See **GUIDE 014** in [`guides/prometheus/gitlab.md`](guides/prometheus/gitlab.md).
</details>

<details>
<summary>Where do I request access to Echo’s REST API?</summary>
Open a Jira ticket in *SCRUM* project with the component **echo‑api**.
</details>

#### JSON‑LD for FAQ rich‑results

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "What do “愛來” characters in the logo mean?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "They are Chinese calligraphy for ‘Love comes’, capturing our mission of bringing cultures together."
      }
    },
    {
      "@type": "Question",
      "name": "Can I use Prometheus – Sypec to audit private GitLab repos?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Yes. See GUIDE 014 in the Prometheus integration docs."
      }
    },
    {
      "@type": "Question",
      "name": "Where do I request access to Echo’s REST API?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Open a Jira ticket in SCRUM project with the component echo‑api."
      }
    }
  ]
}
</script>
```

---

## 🛠 Documentation Stack

- **MkDocs + Material theme** (static site generator)
- **Mermaid.js** for diagrams
- **PanDocs** filters for LaTeX → PDF
- **GitHub Actions** workflow `docs-publish.yml` handles lint → build → deploy

---

## 🤝 Contributing

1. Create a branch: `docs/feat/<topic>`
2. Write in Markdown (avoid absolute links; use relative paths).
3. Run `npm run lint:docs` and `mkdocs build --strict`.
4. Open a PR → 1 approval + CI green ✔️.

### Style guidelines
- Sentence‑case headings
- One sentence per line (easier diffs)
- American English spelling

---

## 📜 License & Copyright

Documentation © \the\year{} **E.M.E International SARL**.  
Published under the **Creative Commons Attribution‑NonCommercial‑NoDerivatives 4.0** licence unless stated otherwise.

---

## 🔗 Follow & Contact

- 🌐 Website: <https://emetour.com/>
- 💼 LinkedIn: <https://www.linkedin.com/company/106476437/>
- 🐙 Org home: <https://github.com/EME-International-BVBA/>
- 🛠 Jira Board: <https://miguel-ibrahim.atlassian.net/jira/software/projects/SCRUM/boards/1>

