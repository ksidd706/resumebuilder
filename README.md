# AI Resume Builder Pro — ATS Optimized v2

A fully deployable, production-ready AI resume builder with deep ATS scoring,
keyword alignment, and one-click full resume optimisation powered by Claude.

---

## Deploy to Netlify (5 minutes)

### 1. Get your Anthropic API key
- Go to https://console.anthropic.com → API Keys → Create Key

### 2. Deploy
**Easiest:** Drag the `resume-builder-v2` folder to https://app.netlify.com/drop

**With GitHub (recommended):**
1. Push this folder to a GitHub repo
2. Go to https://app.netlify.com → Add new site → Import from Git
3. Select your repo — Netlify auto-detects `netlify.toml`
4. Click Deploy

### 3. Add API key
1. Netlify → your site → Site configuration → Environment variables
2. Add: `ANTHROPIC_API_KEY` = your key
3. Deploys → Trigger deploy → Deploy site

**Done!** Your site is live.

---

## Features

### ATS Intelligence
- 20-point structural checklist (name, contact, dates, bullets, metrics, action verbs...)
- Real-time ATS score out of 100 with breakdown by category
- Keyword gap analysis — see exactly which job keywords are missing
- Soft skill matching
- ATS formatting rules panel

### Job Role Alignment
- Paste any job description → AI extracts hard skills, soft skills, and key requirements
- "Full Optimize" rewrites your entire resume (headline, summary, bullets, skills) in one click
- Section-by-section AI tailoring
- Auto-add missing job keywords to skills

### Recruiter Appeal
- Recruiter appeal checklist (separate from ATS)
- AI Insights panel with Fix/Boost/Good items
- Weak phrase detection ("responsible for", "helped with")
- Metrics detection and suggestions

### Complete Resume Sections
- Basics (name, headline, contact, LinkedIn, GitHub)
- Professional summary
- Work experience (with employment type, location)
- Education (degree dropdown, GPA, honours, coursework)
- Skills (with keyword matching highlights)
- Certifications (issuer, date, credential ID)
- Projects
- Languages (with proficiency levels)
- Awards & Recognition

---

## File structure

```
resume-builder-v2/
├── index.html              # Full app (single file)
├── netlify.toml            # Netlify config
├── README.md               # This file
└── netlify/
    └── functions/
        └── claude.js       # Serverless API proxy (keeps key secure)
```

---

## Cost estimate

- Netlify free tier: 125,000 function calls/month
- Anthropic API: ~$0.01–0.05 per full optimize session
- Ideal for personal use or small teams
