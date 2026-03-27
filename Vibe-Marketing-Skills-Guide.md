# The Vibe Marketing Skills Pack
### Your Complete Guide to Setup, Usage, and What's Inside

---

## What Are The Vibe Marketing Skills?

The Vibe Marketing Skills are a set of instruction files that turn AI into a professional marketing team. Instead of writing prompts from scratch every time you need a landing page, email sequence, or SEO article, the skills give your AI the methodology, frameworks, and step-by-step processes that professional marketers use.

Think of it this way: AI is smart, but it doesn't know *your* marketing playbook. The skills are the playbook.

You install them once, and from that point on, you can say things like "write me a welcome email sequence" or "find positioning angles for my product" and get senior-level marketing output, not generic AI filler.

**One purchase. Lifetime updates. Works in 10 minutes.**

---

## What's Inside: Every Skill at a Glance

The skills are organized into four layers. Each layer builds on the one before it.

### Foundation Layer
*Run these first. They teach the system who you are.*

**Start Here (Orchestrator)**
The front door to the whole system. It scans your project, asks you two questions, builds your brand foundation, and routes you to the right skill. If you ever don't know what to do next, run this. It also chains skills together for complex workflows. Just say "build me a lead magnet funnel" and it handles the rest.

> Command: `/start-here`

**Brand Voice**
Defines how your brand sounds so every piece of content is consistent. Three modes: extract your voice from existing content you're proud of, build one from scratch through a guided process, or point it at a URL and let it analyze your brand's public presence. Creates a voice profile that every other skill references automatically.

> Command: `/brand-voice`

**Positioning Angles**
Finds the angle that makes your offer stand out. Uses 8 proven frameworks (from experts like April Dunford, Alex Hormozi, and Eugene Schwartz) and researches your competitors' messaging to find gaps. Gives you 3-5 distinct positioning options with a starred recommendation. This is the difference between "another project management tool" and "the only PM tool built for solo founders."

> Command: `/positioning-angles`

---

### Strategy Layer
*Plan what to create and who to create it for.*

**Keyword Research**
Maps your content territory using the "6 Circles Method." Starts with your business goals and audience, validates with live search data, and builds a prioritized content plan. No expensive SEO tools required. Outputs keyword clusters organized by topic, search intent, and priority so you know exactly what to write and in what order.

> Command: `/keyword-research`

**Lead Magnet**
Generates lead magnet concepts (checklists, guides, templates, quizzes) that actually bridge the gap between "interested" and "paying customer." Researches what competitors give away, then creates something better. After you pick a concept, it enters Build Mode and writes the full deliverable, not just the idea.

> Command: `/lead-magnet`

---

### Execution Layer
*Create the actual marketing assets.*

**Direct Response Copy**
Writes landing pages, sales pages, headlines, CTAs, and ads that convert. Built on the principles of Schwartz, Ogilvy, Halbert, and Sugarman, but the output reads like a smart friend explaining something, not a copywriter trying to impress other copywriters. Scores your copy on 7 dimensions and suggests A/B test variants.

> Command: `/direct-response-copy`

**SEO Content**
Produces long-form articles optimized for search that read like a human expert wrote them. Performs live SERP analysis, integrates "People Also Ask" questions, and generates proper schema markup. Also has a refresh mode for updating existing articles when search results change. The goal: content people actually bookmark and share.

> Command: `/seo-content`

**Email Sequences**
Builds the automated email paths between "subscribed" and "purchased." Covers welcome sequences, nurture sequences, launch sequences, re-engagement, and post-purchase. Each email comes with 3 subject line variants for A/B testing, timing recommendations, and full copy. Detects if you have Mailchimp, ConvertKit, or HubSpot connected and can set up the automation directly.

> Command: `/email-sequences`

**Newsletter**
Creates newsletter editions modeled on what works for top creators (Lenny Rachitsky, Morning Brew, Sahil Bloom, The Hustle). Supports 9 formats from curated roundups to deep-dive frameworks to personal essays. Uses live web search to pull current news and trends when relevant.

> Command: `/newsletter`

**Creative Engine**
AI-powered visual asset production. One engine with five modes:

| Mode | What It Produces |
|------|-----------------|
| Product Photos | Studio-quality product photography with controlled lighting and composition |
| Product Videos | Short-form product videos, demos, and motion content |
| Social Graphics | Platform-sized graphics for feeds, stories, covers, and carousels |
| Talking Head | Presenter-style video with lip sync from text or audio |
| Ad Creative | Performance ad variants with hook-format testing matrices |

Requires a Replicate API key for image/video generation. Without it, the skill produces detailed creative briefs and prompts you can use with any tool.

> Command: `/creative`

---

### Distribution Layer
*Get your content everywhere.*

**Content Atomizer**
Takes one piece of content (a blog post, newsletter, podcast, video) and transforms it into platform-optimized posts across LinkedIn, Twitter/X, Instagram, TikTok, YouTube, Threads, Bluesky, and Reddit. Not generic repurposing. Each piece is formatted for that platform's algorithm and audience expectations. One blog post becomes 15+ pieces of content.

> Command: `/content-atomizer`

---

## Getting Started

### What You Need

The skills work with multiple AI tools. Your setup steps depend on which one you use.

| Platform | How Skills Work | Setup |
|----------|----------------|-------|
| **Claude Code** | Full system with install script, brand memory, skill chaining | Run the installer (see below) |
| **Cursor** | Add skills to `.cursor/rules` | Copy skill files into your rules directory |
| **Codex CLI** | Use as `AGENTS.md` | Place skill files where Codex reads agent instructions |
| **Gemini CLI** | Use as `GEMINI.md` | Place skill files where Gemini reads instructions |
| **Claude Desktop** | Upload as project files | Add the `.md` files to a Claude project |
| **ChatGPT** | Paste into conversation or build a Custom GPT | Copy the skill text into your conversation or GPT instructions |
| **Any other LLM** | Copy and paste | Open the `.md` file for the skill you want and paste it in |

---

### Setup: Claude Code (Full Experience)

This is the recommended setup. It gives you the complete system with brand memory, skill chaining, and the orchestrator.

**Step 1: Download and unzip**
Download the skills pack and unzip it. You'll see a folder called `skills-v2/`.

**Step 2: Run the installer**
Open your terminal, navigate into the `skills-v2/` folder, and run:

```bash
bash _system/scripts/install.sh
```

This copies the skills into `~/.claude/skills/vibe-marketing/` where Claude Code can find them.

If you don't need the Creative Engine (image/video generation), you can run:

```bash
bash _system/scripts/install.sh --claude-only
```

**Step 3: Restart Claude Code (important!)**
Claude Code needs to be fully restarted to detect new skills. This is the most common setup issue.
   a. Quit Claude Code completely (not just close the chat window)
   b. Reopen Claude Code

If you skip this step, the `/slash` commands won't show up and it will look like the install didn't work. It did -- you just need to restart.

**Step 4: Verify the installation**
Run the doctor script to confirm everything is in place:

```bash
bash _system/scripts/doctor.sh
```

You can also ask Claude: "Can you check if the Vibe Marketing skills are installed and read the instructions?" This confirms Claude can see and load the skill files.

**Step 5: Run your first skill**
Open Claude Code in any project and type:

```
/start-here
```

The orchestrator will scan your project, ask you two questions about your business, and build your brand foundation. From there, it routes you to whatever skill you need. That's it.

> **Video walkthrough:** For a visual walkthrough of this setup process, watch the installation guide here: [Watch on YouTube](https://youtu.be/P2O3F-zu73s)

---

### Setup: Claude Desktop, ChatGPT, or Other Chat Tools

**Step 1: Download and unzip**
Download the skills pack and unzip it. You'll see a folder called `skills-v2/`.

**Step 2: Find the skill you want**
Each skill has its own folder with a `SKILL.md` file inside. For example:
- `skills-v2/brand-voice/SKILL.md`
- `skills-v2/direct-response-copy/SKILL.md`
- `skills-v2/lead-magnet/SKILL.md`

**Step 3: Use it**
- **Claude Desktop:** Create a new Project, then add the `SKILL.md` file(s) as project knowledge.
- **ChatGPT:** Open the `SKILL.md` file in a text editor, copy the contents, and paste it at the start of your conversation. Or create a Custom GPT with the skill text as its instructions.
- **Any LLM:** Same as ChatGPT. Copy, paste, use.

**Note:** When using skills in chat tools, each skill works as a standalone framework. You won't get the brand memory or automatic skill chaining (those features require Claude Code), but the marketing methodology inside each skill still works.

> **Video walkthrough:** For a visual walkthrough of the setup process, watch the installation guide here: [VIDEO LINK]

---

### Optional: Connect the Creative Engine

The Creative Engine uses Replicate for AI image and video generation. To enable it:

1. Create an account at [replicate.com](https://replicate.com)
2. Go to Account > API Tokens and create a new token
3. Add it to your project's `.env` file:
   ```
   REPLICATE_API_TOKEN=your-token-here
   ```

Without a Replicate key, the Creative skill still works. It produces detailed briefs and prompts you can use with any image/video generation tool.

### Optional: Connect Your Email Tool

If you use Mailchimp, ConvertKit, or HubSpot, the Email Sequences skill can set up automations directly. Add your API key to `.env`:

```
MAILCHIMP_API_KEY=your-key-here
```
or
```
CONVERTKIT_API_KEY=your-key-here
```

The skills detect connected tools automatically.

---

## How The System Works

Three features make the skills more than a collection of prompts.

### Brand Memory

The first time you run `/start-here`, the system creates a `./brand/` folder in your project with files that capture who you are:

- **voice-profile.md** -- How your brand sounds (tone, vocabulary, personality)
- **positioning.md** -- Your market angle and what makes you different
- **stack.md** -- Your connected tools and integrations
- **assets.md** -- A registry of everything the system has produced for you
- **learnings.md** -- Performance data and feedback that makes future output better

Every skill reads the brand files it needs before producing output. Your email sequence knows what your landing page said. Your social posts match your brand voice. You never have to re-explain your business.

### Skill Chaining

Skills pass context to each other. Instead of running one skill at a time and copy-pasting results, you can tell the orchestrator what you want in plain language:

- "Build me a lead magnet funnel" runs Lead Magnet, then Direct Response Copy (for the landing page), then Email Sequences (for the welcome series), then Content Atomizer (for social promotion).
- "Launch my product" chains Positioning, Copy, Email Sequences, and Creative together.
- "Create a content system" runs Keyword Research, SEO Content, Newsletter, and Content Atomizer.

The orchestrator figures out the right sequence and passes the right context between each step.

### Learning Loop

After major deliverables, skills ask for your feedback. What worked? What didn't? Your responses are saved to `learnings.md`, and future skill runs read those learnings to adjust their output. The more you use it, the sharper it gets.

---

## For Existing v1 Users: What Changed

If you purchased the skills before February 2026, you have v1. Here's what's different and how to upgrade.

### What's New in v2

| Feature | v1 | v2 |
|---------|----|----|
| **Skills count** | 10 marketing skills + orchestrator | 10 marketing skills + 1 creative engine (5 modes) |
| **Brand memory** | None. Each skill starts from scratch every time. | Persistent `./brand/` directory. Skills remember your voice, positioning, and past work across sessions. |
| **Skill chaining** | Run one skill at a time, manually. | Skills chain together automatically. Ask for a "lead magnet funnel" and four skills run in sequence. |
| **Orchestrator** | Basic router that recommends which skill to use. | Full project scanner that audits your situation, builds your brand foundation, and chains workflows. |
| **Email Sequences** | Standalone email copy generation. | ESP auto-detection (Mailchimp, ConvertKit, HubSpot, SendGrid, ActiveCampaign), two-mode operation ("Set it up" via API or "Just the copy" as .md files), JSON schema export for ESP import, MCP server integration. Always saves local .md files as source of truth. |
| **Creative Engine** | Separate "Creative Pack" add-on with 5 standalone skills. | Unified creative engine with 5 modes, shared brand kit, and model selection built in. |
| **Output formatting** | Varies by skill. | Consistent visual design system across every skill with structured headers, file saves, and next-step recommendations. |
| **Feedback loop** | None. | Skills ask for feedback and log it. Future runs read your learnings and adjust. |
| **JSON schemas** | None. | Structured data contracts for voice profiles, campaign briefs, keyword plans, and more (useful for downstream automation). |
| **Platform support** | Claude Code and copy-paste into chat tools. | 8+ AI platforms natively supported, including Claude Code, OpenClaw (native skills pack), Cursor, Codex CLI, Gemini CLI, Claude Desktop, ChatGPT, and any LLM via copy-paste. |

### Memory & Learning System

V2 introduced a persistent intelligence layer that didn't exist in v1:

- **Brand memory protocol** -- 9 persistent files in `./brand/` (voice, positioning, audience, competitors, creative-kit, stack, keywords, assets, learnings) with Context Matrix intelligence. Each skill loads only the files it needs to prevent attention dilution.
- **Self-improving feedback loop** -- Collects performance data after deliverables and appends it to `learnings.md`. Future runs auto-adapt based on what worked (e.g., "subject lines with numbers outperform questions by 21%").
- **Progressive enhancement** -- Works at zero context (just asks questions) all the way to Level 5 (fully personalized). Every level adds quality; none are required.

### System Architecture

- **Stateful and compounding** -- Every skill run builds brand memory, making future outputs better without re-work. 3-tier graceful degradation: standalone (no brand files), partial (some context), and full personalization.
- **Automation-ready** -- 6 JSON schemas enable direct handoffs between skills and external tools (keyword plan feeds SEO content, email sequence exports to ESP).
- **Parallel execution** -- Foundation skills dispatch simultaneously via task agents for 2x faster onboarding.

### New and Upgraded in v2

**New:**
- **Creative Engine** -- One master skill that routes to 5 production modes (product-photo, product-video, social-graphics, talking-head, ad-creative) via Replicate API with shared brand kit and smart model selection. Replaces the separate v1 Creative Pack. Benefits: consistent brand identity across all visual assets, campaign-scale batch generation, more control, and cost efficiency through direct API access.

**Rebuilt from scratch:**
- **Start Here (Orchestrator)** -- Smart project scanner that reads existing brand files, campaigns, and tools on every session. Two operating modes: first-run builds your foundation in parallel; returning mode identifies gaps and suggests the highest-impact next action. Includes 7 pre-built automated workflow chains (Starting from Zero, I Need Leads, Launching Something, and more) with time estimates and confirmation. Enforces 10 anti-patterns: never asks more than 2 questions, never dumps menus, never skips context, always checks dependencies.

**Major upgrades:**
- **Email Sequences** -- V1 generated email copy you'd paste into your ESP. V2 auto-detects your ESP credentials (Mailchimp, ConvertKit, HubSpot, SendGrid, ActiveCampaign), offers two modes ("Set it up" to create automation via API, or "Just the copy" for paste-ready .md files), exports JSON schema for ESP import, and integrates with MCP servers for email capabilities. Always saves local .md files as your source of truth regardless of ESP integration.

### How to Upgrade

**Step 1: Remove v1 skill files**
If you installed v1 into Claude Code, delete the old skill folder. The default location would be inside `~/.claude/skills/`. Remove the old skill files (they would be named things like `brand-voice`, `orchestrator`, `seo-content`, etc.).

If you were using v1 by pasting into Claude Desktop or ChatGPT, there's nothing to uninstall. Just start using the v2 files instead.

**Step 2: Install v2**
Follow the Getting Started instructions above.

**Step 3: Restart Claude Code**
Quit Claude Code completely (not just close the chat) and reopen it. The new skills won't appear until you do this.

**Step 4: Verify and rebuild your brand foundation**
Ask Claude: "Can you check if the Vibe Marketing skills are installed and read the instructions?" Once confirmed, run `/start-here`. Even if you've used the skills before, v2 needs to create your `./brand/` directory. The orchestrator will walk you through it. Takes about 5 minutes.

**Important:** Do not run v1 and v2 at the same time in Claude Code. The overlapping skill names will cause conflicts. V2 replaces v1 entirely. There's no reason to keep both installed, as v2 includes everything v1 had plus the new system layer.

---

## Quick Reference

| I want to... | Run this |
|--------------|----------|
| Get started / don't know what to do | `/start-here` |
| Define or update my brand voice | `/brand-voice` |
| Find my market angle | `/positioning-angles` |
| Plan my content strategy | `/keyword-research` |
| Create a lead magnet | `/lead-magnet` |
| Write a landing page or sales copy | `/direct-response-copy` |
| Write an SEO article | `/seo-content` |
| Build an email sequence | `/email-sequences` |
| Write a newsletter | `/newsletter` |
| Create images, video, or ad creative | `/creative` |
| Repurpose content across platforms | `/content-atomizer` |
| Run a full workflow (funnel, launch, etc.) | `/start-here` and describe what you need |

---

## FAQ

**How long does setup take?**
About 2 minutes to install. Another 5-10 minutes for your first `/start-here` run where it builds your brand foundation. After that, you're producing marketing assets.

**Do I need to be technical?**
No. If you can type a sentence describing what you need, the skills handle the rest. The Claude Code setup requires running a couple terminal commands, but they're copy-paste.

**What if I only use Claude Desktop or ChatGPT?**
The skills still work great as standalone frameworks. You'll miss the brand memory and skill chaining features (those require Claude Code), but the marketing methodology in each skill file is the same.

**Can I edit what the skills produce?**
Yes. Everything is saved as plain markdown files. Edit them however you want. Skills check for existing files before overwriting and will ask for confirmation before replacing anything.

**How does it get better over time?**
After major deliverables, skills ask for your feedback. Your responses are logged and referenced by future skill runs. The system learns what you like, what converts, and what your audience responds to.

**What if I want to start over?**
Run `/start-here` and tell it you want to reset. It guides you through removing your brand and campaign files. Nothing is deleted without your confirmation.

**I already have v1. Do I lose anything by upgrading?**
No. Every v1 capability is included in v2, improved. The upgrade adds brand memory, skill chaining, the creative engine, the learning loop, and major upgrades to the orchestrator and email sequences. Your old outputs (any content the v1 skills created) are still just files on your computer and won't be affected.

---

## Getting Updates

The skills pack includes lifetime updates. Whenever a new version is released, you'll receive an email notification.

To download the latest version:

1. Go to [thevibemarketer.com/portal](https://www.thevibemarketer.com/portal)
2. Enter the email address you used to purchase
3. A download link will be sent to your email

That's it. You can return to that link anytime to grab the newest version, whether it's a minor update or a major release. No extra cost, no subscription -- if you purchased once, you always have access to the latest.
