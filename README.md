# 📊 GSC Skills for Claude Code

> **Turn Google Search Console data into strategic growth insights.** AI agent skills for SEO analysis, content strategy, and paid search planning—built for startup founders and marketing leaders.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Skills](https://img.shields.io/badge/skills-1-green.svg)](#skills)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-compatible-purple.svg)](https://claude.ai/claude-code)

---

## Why This Exists

Google Search Console has valuable data, but turning it into strategic decisions is painful:

- ❌ Exporting CSVs and building spreadsheets
- ❌ Manually classifying brand vs. non-brand keywords
- ❌ No revenue impact estimates for opportunities
- ❌ Hard to prioritize what actually matters

**GSC Skills fixes this.** Drop in a GSC export, and get:

- ✅ Brand vs. non-brand analysis with health scores
- ✅ SEO quick wins sized by revenue potential
- ✅ Content gap analysis with funnel mapping
- ✅ Paid search strategy with budget allocation
- ✅ Prioritized action plans you can execute on

---

## 🚀 Quick Start

### Install via npx (Recommended)

```bash
npx skills add coreyrab/gsc-skills
```

### Manual Installation

```bash
# Clone the repo
git clone https://github.com/coreyrab/gsc-skills.git

# Copy skills to your Claude Code directory
cp -r gsc-skills/skills/* ~/.agents/skills/
```

### Git Submodule (for teams)

```bash
git submodule add https://github.com/coreyrab/gsc-skills.git .skills/gsc
```

---

## 📋 Skills

| Skill | Description | Trigger Examples |
|-------|-------------|------------------|
| **[gsc-analyzer](skills/gsc-analyzer/)** | Strategic GSC analysis with revenue impact, brand segmentation, and prioritized recommendations | "Analyze this GSC export", "How much SEO revenue are we missing?", "What should we focus on this quarter?" |

---

## 💡 What You Can Do

### Brand vs. Non-Brand Analysis
```
"Here's our GSC data. What's our brand dependency and is it healthy?"
```
→ Get traffic composition, brand health scores, and trend analysis

### SEO Opportunities with Revenue Impact
```
"Find quick win keywords and tell me how much revenue we're leaving on the table"
```
→ Prioritized keyword list with estimated monthly revenue per opportunity

### Content Gap Analysis
```
"What content should we create based on search demand?"
```
→ Topic clusters, question-based content ideas, comparison opportunities

### Paid Search Strategy
```
"Which keywords should we run Google Ads for?"
```
→ High-intent targets, SERP domination opportunities, budget allocation

### Strategic Summary
```
"Give me the TL;DR on our organic search performance"
```
→ Headline metrics, key risks, opportunities with revenue estimates, what to do next

---

## 📊 Analysis Modes

### Mode 1: Brand vs. Non-Brand
- Brand dependency score (healthy: 20-40%)
- Traffic composition breakdown
- CTR and position benchmarks
- Risk assessment for high brand dependency

### Mode 2: SEO Analyst
- Quick wins: Position 4-10 keywords ready for top 3
- Striking distance: Position 11-20 keywords
- CTR optimization opportunities
- Cannibalization detection

### Mode 3: Content Strategist
- Topic clusters without dedicated content
- Question-based content opportunities
- Comparison/alternative content gaps
- International/multilingual opportunities

### Mode 4: Paid Search Specialist
- High-intent keywords not ranking organically
- SERP domination candidates
- Competitor conquesting targets
- Budget allocation recommendations

### Mode 5: Strategic Summary
- Headline metrics with status indicators
- Key risks with business impact
- Opportunities with revenue estimates
- 90-day priorities

---

## 🔧 How It Works

1. **Export GSC data** from Google Search Console (Performance → Export)
2. **Provide the file** to Claude Code (zip or folder of CSVs)
3. **Confirm brand terms** when prompted
4. **Choose analysis modes** or run full analysis
5. **Get actionable insights** with revenue estimates

### Supported Formats
- GSC zip exports
- Individual CSV files (Queries.csv, Pages.csv, etc.)
- Folders containing GSC CSV exports

---

## 📈 Example Output

```markdown
# Acme Corp Organic Search Performance - Q4 2025

## Headline Metrics
| KPI | Value | Trend | Status |
|-----|-------|-------|--------|
| Monthly Organic Clicks | 277K | ↓ 15% | ⚠️ Warning |
| Brand Dependency | 72% | → Flat | 🔴 Critical |
| Non-Brand Position | 5.4 | → Flat | 🟡 Needs work |

## Key Opportunities
1. **Quick Win Keywords** - $168K-420K ARR potential
   - 10 keywords in position 4-10 with high volume
   - Action: Title/meta optimization, 30-day sprint

2. **Content Gaps** - $50K-100K ARR potential
   - No dedicated pages for "best AI for X" queries
   - Action: Create 5 SEO landing pages

## What To Do Next
- 1 FTE content marketer for SEO content
- $5-10K/month PPC budget for non-brand acquisition
```

---

## 🤝 Contributing

Contributions welcome! Ideas for improvement:

- [ ] Additional industry benchmarks (e-commerce, B2B, etc.)
- [ ] Integration with other data sources (GA4, Ahrefs, etc.)
- [ ] Automated anomaly detection refinements
- [ ] More summary templates

### File Structure

```
gsc-skills/
├── README.md
├── LICENSE
└── skills/
    └── gsc-analyzer/
        ├── SKILL.md              # Main skill instructions
        ├── scripts/
        │   └── parse_gsc_data.py # GSC parser with brand classification
        └── references/
            ├── brand_analysis.md
            ├── seo_analysis.md
            ├── content_opportunities.md
            ├── paid_search.md
            └── strategic_frameworks.md
```

---

## 📄 License

MIT License - see [LICENSE](LICENSE) for details.

---

## 🔗 Links

- **Creator**: [Corey Haines](https://twitter.com/coreyhainesco)
- **More Skills**: [marketingskills](https://github.com/coreyhaines31/marketingskills)
- **Claude Code**: [claude.ai/claude-code](https://claude.ai/claude-code)

---

<p align="center">
  <b>Stop wrestling with spreadsheets. Start making strategic decisions.</b>
</p>
