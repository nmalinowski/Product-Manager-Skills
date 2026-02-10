# Marketplace Strategy — Product Manager Skills

**Last Updated:** February 10, 2026
**Status:** Quality Audit Complete ✅ | Ready for Submission
**Next Review:** February 17, 2026

## 🚀 Next Session Action Items (Feb 10, 2026)

**Priority 1: Get GitHub Stars (SkillsMP Requirement)**
- [ ] Share repo on LinkedIn with PM network
- [ ] Post to r/ProductManagement subreddit
- [ ] Share in PM Slack communities (Lenny's, Product School, Mind the Product)
- [ ] Email to Productside client list
- **Goal:** Achieve 2+ stars for SkillsMP auto-indexing

**Priority 2: Quick Wins (Low Effort, High Visibility)**
- [ ] Fork and submit PR to [Awesome Claude Skills](https://github.com/travisvn/awesome-claude-skills)
- [ ] Join ClaudeSkills.ai waitlist
- [ ] Add GitHub topics: `product-management`, `claude-skills`, `ai-agents`, `pm-frameworks`

**Priority 3: Strategic Decisions Needed**
- [x] Decide: Monetization approach (Free+Consulting vs. Freemium vs. PWYW)
- [x] Decide: Curate 5 "showcase" skills for Anthropic first (instead of submitting all 40+)
- [ ] Review: Do any 200-char descriptions need optimization for clarity?

---

## Overview

This document outlines AI skill marketplaces where Product Manager Skills can be listed, submission requirements, and a rollout plan to maximize discoverability and adoption.

---

## ✅ Quality Audit Results (Feb 6, 2026)

**Status:** All skills pass marketplace requirements

**Validation Script:** `scripts/check-skill-metadata.py`

### What Was Checked
- ✅ **YAML Frontmatter:** All 40+ skills have valid frontmatter
- ✅ **Name Field:** Present and ≤ 64 characters (all skills)
- ✅ **Description Field:** Present and ≤ 200 characters (all skills)
- ✅ **Folder Names:** Match frontmatter `name` values (all 40+ skills)

### Sample Validation Results
| Skill | Name Length | Description Length | Status |
|-------|-------------|-------------------|--------|
| ai-shaped-readiness-advisor | 27 chars | 123 chars | ✅ Pass |
| prioritization-advisor | 22 chars | 200 chars | ✅ Pass (at limit) |
| user-story | 10 chars | 199 chars | ✅ Pass (at limit) |
| discovery-process | 17 chars | 200 chars | ✅ Pass (at limit) |

### Marketplace Readiness
✅ **Ready for immediate submission:**
- SkillsMP (needs 2+ GitHub stars only)
- SkillHub (ready now)
- Anthropic official skills repo (ready now)
- Awesome Claude Skills (ready now)

⚠️ **Note:** 3 skills have descriptions at exactly 200 characters. Consider slight optimization for clarity if needed.

---

## 🎯 Goals

1. **Increase discoverability** — Help PMs find these skills when searching for product management frameworks
2. **Build credibility** — Leverage marketplace validation (stars, ratings, reviews) as social proof
3. **Drive adoption** — Make it frictionless for users to install and use these skills
4. **Generate revenue** (optional) — Some marketplaces support paid skills (90% creator revenue share)
5. **Community engagement** — Gather feedback, feature requests, and contributions

---

## 🔍 Assumptions to Verify (Before Submitting)

- [ ] Confirm SkillsMP current indexing rules (stars threshold, crawl cadence)
- [ ] Confirm SkillHub submission path (auto discovery vs. curated PR)
- [ ] Confirm ClaudeSkills.ai submission flow and paid-skill policy
- [ ] Confirm Anthropic skills repo requirements (tests/examples expectations)
- [ ] Confirm each marketplace accepts CC BY-NC-SA 4.0 or requires an alternate license

---

## 🧭 Marketplace Fit Matrix (Initial)

| Marketplace | PM Audience Fit | Submission Effort | License Compatibility | Monetization Support | Expected ROI | Notes |
|-------------|-----------------|-------------------|-----------------------|----------------------|--------------|-------|
| SkillsMP | High | Low | TBD | Unknown | High | Auto indexing from GitHub; star threshold applies |
| SkillHub | Medium | Medium | TBD | Unknown | Medium | AI scoring could amplify visibility |
| ClaudeSkills.ai | Medium | Medium | TBD | Yes | Medium | Waitlist; paid skills |
| Anthropic official skills | High | Medium | TBD | No | High | Official endorsement value |
| Awesome Claude Skills | Medium | Low | N/A | No | Medium | Community discovery via GitHub |
| Agent Skills Market | TBD | TBD | TBD | Unknown | TBD | Needs research |

---

## 🏪 Available Marketplaces (2026)

### Primary Targets

#### 1. **Skills.sh** — The Open Agent Skills Directory
- **URL:** https://skills.sh/
- **Status:** Active, 200+ skills indexed
- **Compatible With:** Claude Code, Codex, VS Code Copilot, Cursor, and 20+ agent platforms
- **Pricing Model:** Free (open ecosystem)
- **Submission Process:** None - GitHub is the registry (skills installable immediately)
- **Installation:** `npx skills add deanpeters/Product-Manager-Skills@<skill-name>`
- **Discovery Features:**
  - CLI-native discovery: `npx skills find <query>`
  - Direct installation from GitHub repos
  - Agent-agnostic (works across platforms)
  - Automatic leaderboard via anonymous telemetry

**Why This Matters:**
- **Already live** - All 40+ skills are installable right now
- **Zero friction** - No approval, no waiting, no submission
- **Foundation layer** - Other marketplaces use skills.sh for installation
- **Ecosystem standard** - The "npm for agent skills"

**Action Items:**
- ✅ Already live and installable (public repo = immediate availability)
- ✅ Documentation complete (installation covered in Claude/Codex docs)
- 📋 Share installation commands in announcements (LinkedIn, Substack)
- 📋 Monitor appearance on https://skills.sh/deanpeters/Product-Manager-Skills
- 📋 Organic discovery through community sharing and installs

**Positioning:**
"Several dozen production-ready PM skills, instantly installable via `npx skills add`"

---

#### 2. **SkillsMP** — Agent Skills Marketplace
- **URL:** https://skillsmp.com/
- **Status:** Active, 145,000+ skills indexed
- **Compatible With:** Claude Code, Codex CLI, ChatGPT
- **Pricing Model:** Free (aggregates from GitHub)
- **Submission Process:** Automatic discovery from public GitHub repos
- **Requirements:**
  - Public GitHub repository
  - Minimum 2 GitHub stars (quality filter)
  - Valid `SKILL.md` file following Anthropic open standard
  - Optional: `scripts/` and `template.md` files
- **Discovery Features:**
  - Smart search with semantic matching
  - Category filtering (Product Management, Software Engineering, etc.)
  - Quality indicators (stars, usage stats)
  - AI-powered skill recommendations

**Action Items:**
- ✅ Already meets requirements (public repo, SKILL.md format)
- ⏳ Get to 2+ GitHub stars (currently unknown)
- ⏳ Wait for automatic indexing by SkillsMP crawler
- 📋 Monitor when skills appear on platform

---

#### 3. **SkillHub** — Claude Skills & Agent Skills Marketplace
- **URL:** https://www.skillhub.club/
- **Status:** Active, 7,000+ AI-evaluated skills
- **Compatible With:** Claude, Codex, Gemini, OpenCode
- **Pricing Model:** Free (aggregates from GitHub)
- **Evaluation System:** AI rates skills on 5 dimensions:
  1. **Practicality** — Real-world usefulness
  2. **Clarity** — Documentation quality
  3. **Automation** — Efficiency gains
  4. **Quality** — Code/instruction quality
  5. **Impact** — Strategic value
- **Rating Scale:** S-rank (9.0+), A-rank, B-rank, etc.
- **Submission Process:** Appears to be automatic discovery (details unclear)
- **Requirements:**
  - Public GitHub repository
  - Valid `SKILL.md` format
  - GitHub repository: `github.com/keyuyuan/skillhub-awesome-skills` (curated list)

**Action Items:**
- 📋 Investigate submission process (contact SkillHub or check docs)
- 📋 Submit to curated `skillhub-awesome-skills` GitHub repo
- 🎯 Optimize skills for AI evaluation criteria (practicality, clarity, impact)

---

#### 4. **ClaudeSkills.ai** — The Marketplace for Claude AI Skills
- **URL:** https://claudeskills.ai/
- **Status:** Waitlist / Early Access
- **Compatible With:** Claude AI (all platforms)
- **Pricing Model:** Paid skills supported
  - Creators keep 90%
  - Payouts via Stripe Connect
- **Submission Process:** TBD (platform in development)
- **Requirements:** Unknown (likely standard SKILL.md format)

**Action Items:**
- 📋 Join waitlist at https://claudeskills.ai/
- 📋 Monitor for platform launch announcements
- 💡 Consider monetization strategy:
  - **Option A:** All skills free (maximize adoption)
  - **Option B:** Basic skills free, premium bundles paid (e.g., "AI PM Pro Pack")
  - **Option C:** Free skills + consulting/training upsell

---

#### 5. **Anthropic Official Skills Repository**
- **URL:** https://github.com/anthropics/skills
- **Status:** Active (official Anthropic repo)
- **Compatible With:** Claude Code, Claude AI
- **Pricing Model:** Free (community contributions)
- **Submission Process:** Pull request to public repo
- **Requirements:**
  - Follow Anthropic SKILL.md specification
  - Pass quality review by Anthropic maintainers
  - Include tests/examples when applicable

**Action Items:**
- 📋 Review Anthropic's contribution guidelines
- 📋 Select 3-5 "showcase" skills to submit (highest quality, most useful)
- 📋 Submit PR with selected skills
- 🎯 Goal: Get official Anthropic endorsement

**Recommended Skills to Submit:**
1. `user-story` — Fundamental, widely applicable
2. `prioritization-advisor` — Interactive, high-value
3. `discovery-process` — Complete workflow, demonstrates sophistication
4. `pol-probe-advisor` — Unique, based on Dean's proprietary framework
5. `context-engineering-advisor` — Cutting-edge, aligns with Anthropic's focus

---

### Secondary Targets

#### 6. **Agent Skills Market**
- **URL:** https://www.agentskillsmarket.space/
- **Status:** Active (#1 Agent Skills Library for Claude AI & LLMs 2025)
- **Action Items:** 📋 Research submission process

#### 7. **Awesome Claude Skills (GitHub)**
- **URL:** https://github.com/travisvn/awesome-claude-skills
- **Status:** Active (3,200+ stars)
- **Submission Process:** Pull request to add link
- **Action Items:**
  - ✅ Fork repo
  - 📋 Add Product Manager Skills to relevant category
  - 📋 Submit PR with description and link

#### 8. **ChatPRD** — AI Platform for Product Managers
- **URL:** https://www.chatprd.ai/
- **Status:** Active (popular PM-specific tool)
- **Action Items:** 📋 Explore partnership/integration opportunities

---

## 📋 Rollout Plan

### Phase 0: Skills.sh (Already Live) ✅
**Goal:** Leverage the already-live installation channel

- [x] **Immediate Availability** ✅ COMPLETE
  - [x] All 40+ skills installable via `npx skills add deanpeters/Product-Manager-Skills@<skill-name>`
  - [x] CLI discovery working: `npx skills find product management`
  - [x] Documentation complete in Claude/Codex guides
  - [x] GitHub is the registry (no submission needed)

- [ ] **Community Activation** (This Week)
  - [ ] Include CLI install commands in LinkedIn announcement
  - [ ] Add CLI install examples to Substack article
  - [ ] Share in PM communities (Reddit, Slack) with install commands
  - [ ] Monitor skills.sh leaderboard for appearance

**Positioning Message:**
"Several dozen production-ready PM skills, instantly installable for Claude Code, Codex, and 20+ agent platforms via `npx skills add`"

---

### Phase 1: Preparation (Week 1)
**Goal:** Optimize for additional marketplace discovery

- [x] **Quality Audit** ✅ COMPLETE (Feb 6, 2026)
  - [x] Run `scripts/check-skill-metadata.py` on all skills — All 40+ pass
  - [x] Verify all skills have proper YAML frontmatter — Validated
  - [x] Ensure `name` ≤ 64 chars, `description` ≤ 200 chars — Confirmed
  - [ ] Validate all cross-references between skills — TODO

- [ ] **Documentation Enhancement**
  - Add "Featured Skills" section to README.md
  - Create `/docs/Marketplace Listings.md` (this file)
  - Add badges to README for marketplace presence

- [ ] **GitHub Optimization**
  - Add relevant tags: `product-management`, `claude-skills`, `ai-agents`, `pm-frameworks`
  - Ensure GitHub description is compelling
  - Add social preview image (repo settings)
  - Request stars from early users/testers

- [ ] **Create Showcase Materials**
  - Record demo video (3-5 min) showing skills in action
  - Create screenshot gallery for each skill type (Component, Interactive, Workflow)
  - Write "Getting Started in 60 Seconds" guide

---

## ✅ Submission Checklist & Standard Listing Blurb

**Checklist**
- [ ] Repo URL
- [ ] One-paragraph description (PM-focused)
- [ ] Top 3 featured skills (with one-line value props)
- [ ] License statement (CC BY-NC-SA 4.0)
- [ ] Contact email
- [ ] Demo link (video or screenshots)
- [ ] Tags/keywords (product management, discovery, roadmap, PRD, metrics, GTM)

**Standard Listing Blurb (Updated)**
```md
Product Manager Skills — Several dozen production-ready PM frameworks for AI agents.

Install instantly via `npx skills add deanpeters/Product-Manager-Skills@<skill-name>` or browse at
https://github.com/deanpeters/Product-Manager-Skills

Includes discovery workflows, prioritization advisors, finance metrics, roadmap planning, PRD templates,
and interactive decision frameworks. All skills are open-source (CC BY-NC-SA 4.0) and work with Claude Code,
Codex, VS Code Copilot, Cursor, and 20+ agent platforms.

Featured: finance-metrics-quickref, discovery-process, context-engineering-advisor, pol-probe-advisor
```

**Short Version (for limited-character listings):**
```md
Several dozen production-ready PM skills for AI agents. Discovery workflows, prioritization frameworks,
finance metrics, roadmap planning. Instantly installable via npx skills add. Works with Claude Code,
Codex, and 20+ platforms.
```

---

### Phase 2: Primary Marketplace Submissions (Week 2)
**Goal:** Get listed on major skill marketplaces

- [ ] **SkillsMP (Automatic)**
  - Achieve 2+ GitHub stars (quality threshold)
  - Monitor for automatic indexing
  - Once indexed, optimize skill descriptions for search
  - Share SkillsMP links in README.md

- [ ] **SkillHub (Manual Submission)**
  - Contact SkillHub via https://www.skillhub.club/
  - Submit to `skillhub-awesome-skills` GitHub repo
  - Request AI evaluation
  - Track rating scores (target: S-rank or A-rank)

- [ ] **Anthropic Official Skills (Curated PR)**
  - Select 3-5 showcase skills
  - Prepare high-quality PR with:
    - Clear descriptions
    - Usage examples
    - Tests/validation
  - Submit PR and engage with maintainer feedback
  - Promote official listing in marketing materials

- [ ] **Awesome Claude Skills (Community)**
  - Fork `travisvn/awesome-claude-skills`
  - Add entry under "Product Management" category (create if needed)
  - Write compelling 2-sentence description
  - Submit PR

---

### Phase 3: Secondary Platforms & Promotion (Week 3)
**Goal:** Expand reach and build community

- [ ] **Additional Marketplaces**
  - Research and submit to Agent Skills Market
  - Join ClaudeSkills.ai waitlist
  - Explore ChatPRD partnership opportunities

- [ ] **Community Outreach**
  - Post on r/ProductManagement (Reddit)
  - Share on Product Hunt (as "launch")
  - Write LinkedIn post with demo
  - Post on X/Twitter with #ProductManagement #AI hashtags
  - Cross-post to relevant Slack/Discord communities (Lenny's, Product School, etc.)

- [ ] **Content Marketing**
  - Write Substack article: "Several Dozen AI Skills Every PM Should Have"
  - Create YouTube tutorial (or partner with PM influencer)
  - Guest post on PM blogs (Mind the Product, Product Coalition, etc.)

---

### Phase 4: Monitoring & Optimization (Ongoing)
**Goal:** Track performance and iterate

- [ ] **Analytics Tracking**
  - Set up GitHub traffic monitoring
  - Track marketplace listing views (where available)
  - Monitor stars, forks, issues, PRs
  - Survey users: "How did you discover these skills?"

- [ ] **Feedback Loop**
  - Create GitHub Discussions for Q&A
  - Set up issue templates for:
    - Bug reports
    - Feature requests
    - New skill suggestions
  - Monthly review of user feedback
  - Quarterly skill quality audit

- [ ] **Marketplace Optimization**
  - A/B test skill descriptions (if platform allows)
  - Update skills based on user feedback
  - Add new skills based on demand
  - Maintain top ratings on SkillHub (target: S-rank)

---

## 🛠️ Maintenance & Ownership

- Assign a single owner for marketplace updates and PR submissions
- Define update cadence (monthly sync, quarterly quality audit)
- Track where updates are manual vs. auto-synced
- Keep a changelog of marketplace listings and dates submitted

---

## ⚠️ Risks & Mitigations

- **License mismatch:** Some marketplaces may not accept CC BY-NC-SA  
  Mitigation: Confirm policy up front; consider dual-licensing if needed
- **Low AI evaluation scores:** Poor ratings reduce visibility  
  Mitigation: Optimize clarity, examples, and practical framing
- **Slow auto-indexing:** Discovery delays impact momentum  
  Mitigation: Reach out to maintainers and include in curated lists
- **PRs stalled in curation repos:** Review queues can be slow  
  Mitigation: Submit early and follow up politely

---

## 🎯 Success Metrics

### Quantitative
- **GitHub Stars:** Target 100+ in first 3 months
- **Marketplace Views:** Track when data available
- **Installation/Usage:** Monitor via GitHub traffic (clone/download stats)
- **Community Growth:** Contributors, issues filed, discussions started

### Qualitative
- **Ratings:** Achieve S-rank or A-rank on SkillHub
- **Official Recognition:** Get accepted into Anthropic official skills repo
- **Testimonials:** Collect user success stories
- **Media Mentions:** Coverage in PM blogs, newsletters, podcasts

---

## 💰 Monetization Strategy (Optional)

### License Compatibility Note

- CC BY-NC-SA 4.0 limits commercial use; confirm each marketplace’s paid-skill policy
- If monetization is required, consider dual-licensing or a separate paid bundle with a commercial-friendly license

### Option A: Free + Consulting (Recommended)
- All 40+ skills remain **free and open-source**
- Use as lead generation for Productside consulting
- Offer paid workshops: "Mastering AI-Assisted Product Management"
- Premium support tier: $99/month (priority support, custom skill development)

### Option B: Freemium Model
- **Free Tier:** 20 core skills (user-story, positioning-statement, etc.)
- **Pro Tier:** All 40+ skills + future additions ($19/month or $149/year)
- **Enterprise Tier:** Custom skills, team training, white-label ($499/month)

### Option C: Pay-What-You-Want
- All skills free by default
- "Support this project" link (GitHub Sponsors, Buy Me a Coffee)
- Suggested donation: $20 (covers cost of 1 hour consulting)

**Recommendation:** Start with Option A (Free + Consulting) to maximize adoption and brand building.

---

## 📚 Resources for Submission

### Required Files (Already Have)
- ✅ Individual `SKILL.md` files (40+ skills)
- ✅ YAML frontmatter with `name`, `description`, `type`
- ✅ Templates and examples separated (recent refactor)
- ✅ Optional scripts (deterministic, documented)
- ✅ LICENSE.md (CC BY-NC-SA 4.0)
- ✅ CONTRIBUTING.md
- ✅ README.md with comprehensive catalog

### Optional Enhancements
- 📋 Demo videos (Loom or YouTube)
- 📋 Social preview image (1200x630px)
- 📋 Skill showcase page (GitHub Pages)
- 📋 Badge system (e.g., "Featured on SkillHub")

---

## 🔗 References

### Marketplace Research
- [Skills.sh — The Open Agent Skills Directory](https://skills.sh/)
- [Skills.sh Documentation](https://skills.sh/docs)
- [Agent Skills Standard (agentskills.io)](https://agentskills.io/)
- [SkillsMP — Agent Skills Marketplace](https://skillsmp.com/)
- [SkillHub — Claude Skills Marketplace](https://www.skillhub.club/)
- [ClaudeSkills.ai](https://claudeskills.ai/)
- [Anthropic Official Skills Repository](https://github.com/anthropics/skills)
- [Awesome Claude Skills](https://github.com/travisvn/awesome-claude-skills)
- [SkillsMP Complete Guide 2026](https://smartscope.blog/en/blog/skillsmp-marketplace-guide/)
- [Claude Code Has a Skills Marketplace Now](https://medium.com/@markchen69/claude-code-has-a-skills-marketplace-now-a-beginner-friendly-walkthrough-8adeb67cdc89)

### PM Tools & Marketplaces
- [ChatPRD — AI Platform for Product Managers](https://www.chatprd.ai/)
- [18 Best AI Product Management Tools Reviewed in 2026](https://cpoclub.com/tools/best-ai-product-management-tools/)
- [HBR: To Drive AI Adoption, Build Your Team's Product Management Skills](https://hbr.org/2026/02/to-drive-ai-adoption-build-your-teams-product-management-skills)

---

## 📞 Next Steps

**Phase 0 is Live** ✅
- All 40+ skills already installable via skills.sh
- No submission, approval, or waiting required
- Focus: community activation and sharing

**Immediate Actions (This Week):**
1. ✅ Quality audit complete (`scripts/check-skill-metadata.py`)
2. 📋 Launch announcement with CLI install commands (LinkedIn, Substack)
3. 📋 Share in PM communities with `npx skills add` examples
4. 📋 Fork and PR to `awesome-claude-skills`
5. 📋 Achieve 2+ GitHub stars (unlocks SkillsMP auto-indexing)
6. 📋 Join ClaudeSkills.ai waitlist

**Strategic Decisions:**
- ✅ Monetization: Free + Consulting (lead gen for Productside)
- 📋 Anthropic submission: Curate 5 showcase skills (user-story, prioritization-advisor, discovery-process, pol-probe-advisor, context-engineering-advisor)
- ✅ Brand positioning: "Production-ready PM skills for agent-assisted workflows"

---

## 📊 Summary

### What We Have
✅ **40+ marketplace-ready skills** (all validated, Feb 6, 2026)
✅ **Phase 0 LIVE** - Skills.sh installation working right now
✅ **Comprehensive rollout plan** (Phase 0-4 over 3 weeks)
✅ **6 target marketplaces identified** (Skills.sh, SkillsMP, SkillHub, Anthropic, Awesome Claude Skills, ClaudeSkills.ai)
✅ **Quality audit complete** (all metadata requirements met)
✅ **Documentation complete** (installation covered in Claude/Codex guides)

### What We're Activating
🚀 **Skills.sh ecosystem** - Already installable, needs community sharing
⏳ **2+ GitHub stars** - Unlocks SkillsMP auto-indexing
📋 **PR to Awesome Claude Skills** - Quick visibility win
📋 **Anthropic curated submission** - 5 showcase skills for official repo

### Recommended Path Forward (Feb 10, 2026)
1. **Launch announcement** - Include `npx skills add` commands in LinkedIn/Substack
2. **Community sharing** - Reddit, PM Slack communities, with install examples
3. **Quick wins** - Awesome Claude Skills PR, GitHub stars campaign
4. **Curated submission** - Prepare 5 showcase skills for Anthropic repo

**Timeline:** Phase 0 live now, additional listings within 7-10 days

**Positioning:** "Several dozen production-ready PM skills, instantly installable for Claude Code, Codex, and 20+ agent platforms"

---

**Ready to execute when you are. See you tomorrow!**
