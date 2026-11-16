# Awesome-Free-SaaS-Financial-Metrics-Benchmarking

# Top Free SaaS Financial Metrics & Benchmarking Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on MRR/Churn Analytics, Benchmarking & Self-Hosted Subscription Intelligence*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Free SaaS Financial Metrics & Benchmarking**. These tools help founders and finance teams track MRR, churn, LTV, and acquisition efficiency—covering everything from freemium hosted analytics with free tiers to self-hosted open-source dashboards that calculate SaaS metrics without per-customer pricing.

**Examples** include ProfitWell Metrics (Paddle), ChartMogul, Baremetrics, ChurnLens, OpenProfit, and Revenut (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted SaaS metrics, open-source MRR dashboards, and community-driven subscription analytics—ideal for bootstrapped founders and privacy-conscious teams seeking full data ownership without per-subscriber fees. The open-source landscape is genuinely thin but emerging: **ChurnLens** calculates MRR, churn, and LTV from Stripe or CSV , **OpenProfit** extends analytics to include AI and hosting costs alongside revenue , and **Revenut** focuses on accurate Stripe revenue forecasting by excluding fraudulent transactions .

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[ProfitWell Metrics (Paddle)](https://www.profitwell.com/)** | **The free standard for SaaS subscription analytics.** Tracks MRR, churn, LTV, and benchmark data across 30,000+ companies. Acquired by Paddle; the core metrics product remains **free forever**—monetization comes from Paddle's payment processing and Retain services . | **Free** (core metrics) | **Free forever**: MRR, churn, LTV, benchmarking, and cohort retention |
| **[ChartMogul](https://chartmogul.com/)** | Subscription analytics and revenue reporting. **Pro: $1,188–$14,388/year**; Enterprise from **$19,900/year** . Positioned for SaaS teams wanting deeper segmentation and reporting than free tools provide. | Pro: **$1,188/year** (up to $10K MRR); Enterprise: **$19,900/year** | Free trial available; no permanent free tier |
| **[Baremetrics](https://baremetrics.com/)** | Subscription analytics with MRR, churn, LTV, and forecasting. Positioned as the original Stripe analytics tool. | Quote-only | Free trial available |
| **[Stripe Sigma](https://stripe.com/sigma)** | SQL-based analytics over Stripe data. **$0.03 per query** beyond included allowance; requires Stripe account . Positioned for teams wanting raw data access without a dedicated analytics platform. | **$0.03/query** | No free tier; included query allowance varies |
| **[Databox SaaS Metrics](https://databox.com/)** | Dashboard builder with pre-built SaaS metric templates. Connects to Stripe, ChartMogul, and other sources. | Free tier available; paid plans via sales | **Free tier** available with limited data sources |
| **[Geckoboard](https://www.geckoboard.com/)** | TV dashboard builder for SaaS metrics. Pre-built integrations with Stripe and subscription platforms. | Quote-only | **14-day free trial**; no permanent free tier |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[ChurnLens](https://github.com/cognis-digital/churnlens)** | [![Stars](https://img.shields.io/github/stars/cognis-digital/churnlens?style=social&color=white)](https://github.com/cognis-digital/churnlens/stargazers) | **The most focused open-source SaaS metrics calculator.** **Self-hosted MRR, churn, and LTV from Stripe or CSV**—no SaaS bill, no heavyweight setup. **Single-purpose and scriptable**: `churnlens scan . --format json` for CI gates, `churnlens mcp` for AI agent integration . **Built in the spirit of Baremetrics** but reframed as a single-purpose, MCP-native tool . **Critical licensing caveat**: **COCL v1.0**—free for personal, internal-evaluation, research, and educational use; **commercial/production use requires a license** . **Best for developers wanting a scriptable, CI-friendly metrics calculator** for internal evaluation—not for commercial production without licensing . |
| **[OpenProfit](https://alternativeto.net/software/openprofit/about/)** | — | **The most ambitious open-source alternative to Baremetrics, ChartMogul, and ProfitWell Metrics.** **MIT licensed** . Reads payment processor data **plus billing APIs of OpenAI, Anthropic, Vercel, and other infrastructure providers**—calculates **profit per product** after AI and hosting costs, not just revenue . **Self-hosted or SaaS**; Docker deployment . **Best for AI-era SaaS founders** whose margins depend on API bills and who want to see profitability per product, not just MRR . |
| **[Revenut](https://github.com/hbcondo/revenut-app)** | [![Stars](https://img.shields.io/github/stars/hbcondo/revenut-app?style=social&color=white)](https://github.com/hbcondo/revenut-app/stargazers) | **Open-source Stripe revenue forecasting that fixes a real problem.** Built after the author's SaaS was hit by card testing fraud—**Revenut excludes disputed and refunded transactions** for accurate revenue reporting, unlike Stripe's own mobile app . **Calculates unrealized ("paper") revenue** from trialing customers and scheduled upcoming invoices, plus realized revenue from paid invoices . **FastAPI/Python + React Native PWA**; Apache 2.0 licensed . **Best for Stripe-based founders** wanting accurate revenue metrics that don't include fraudulent transactions . |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[SimpleStats](https://github.com/simplestats-io/app)** | [![Stars](https://img.shields.io/github/stars/simplestats-io/app?style=social&color=white)](https://github.com/simplestats-io/app/stargazers) | **Server-side analytics that follows the full funnel from visit to payment.** **MRR/ARR, churn, and retention** for subscription apps, plus **ROAS/CAC/LTV:CAC** once ad spend is entered. **Attribution back to UTM source**—connects acquisition channels to revenue, not just traffic . **Trade-off**: Laravel-focused; not a pure SaaS metrics tool but broader product analytics with revenue attribution . **Best for Laravel teams** wanting funnel analytics alongside subscription metrics . |
| **[Metabase (SaaS Metrics Templates)](https://github.com/metabase/metabase)** | [![Stars](https://img.shields.io/github/stars/metabase/metabase?style=social&color=white)](https://github.com/metabase/metabase/stargazers) | **General-purpose open-source BI that can be modeled into a SaaS metrics dashboard.** **Free open-source edition with unlimited users** . Connect to your billing database or Stripe data and build MRR/churn reports with the Question builder . **Trade-off**: **not a pre-built SaaS metrics tool**—you define the metrics and queries yourself . **Best for teams wanting maximum flexibility** and willing to own metric definitions . |
| **[Apache Superset](https://github.com/apache/superset)** | [![Stars](https://img.shields.io/github/stars/apache/superset?style=social&color=white)](https://github.com/apache/superset/stargazers) | **Enterprise-grade open-source BI with SQL flexibility.** **75K+ stars** . Suitable for building custom SaaS metric dashboards from billing data . **Trade-off**: **not a SaaS-specific tool**—requires SQL and dashboard design work . **Best for data teams** wanting a powerful, self-hosted BI platform without per-user fees . |

**Frameworks for building custom systems**: Choose **ChurnLens** for a scriptable MRR/churn/LTV calculator from Stripe or CSV (internal evaluation) , **OpenProfit** for profit-per-product metrics that include AI and hosting costs , or **Revenut** for fraud-aware Stripe revenue forecasting —all self-hosted without per-customer fees. For teams wanting a general BI foundation, **Metabase** can be modeled into a SaaS metrics dashboard.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- SaaS metrics tools handle revenue data, customer subscription records, and potentially payment information; enforce access controls and compliance with financial data protection regulations.
- **Open-source SaaS metrics is genuinely thin and carries important caveats.** **ChurnLens is source-available under COCL v1.0**—free for evaluation but **commercial/production use requires a license**; do not deploy it in production without reviewing the terms . **OpenProfit is MIT-licensed** and uniquely calculates profit after AI/hosting costs, but is newer and less proven than commercial tools . **Revenut is Apache 2.0** and solves the specific problem of fraudulent transactions inflating Stripe revenue . **Most general-purpose BI tools (Metabase, Superset) are not pre-built SaaS metrics dashboards**—you define MRR, churn, and cohort retention logic yourself, including edge cases like proration and annual plan handling . **Validate whether you need a focused calculator (ChurnLens, Revenut) or a flexible BI foundation (Metabase)** and confirm licensing before committing.

---

**Made for bootstrapped founders, finance teams, and developers building subscription analytics.**  
Let's make SaaS financial metrics and benchmarking more open, accurate, and cost-predictable.
