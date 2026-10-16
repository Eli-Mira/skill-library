# Skill Library - 2026-10-03 review

Source: the 57-item list Eli sent. Every item reviewed; full evidence in the consolidated JSON.

## Installed and verified

| Skill | Category | Source | Notes |
|---|---|---|---|
| `anti-koshary` | software-development | https://github.com/ismail9k/skills | Installed with --force. Scanner said BLOCKED/CAUTION on one hit: references/security-checks.md:45 listing os.environ/process.env reads as a secret-scan false positive. Read the file in full - it is documentation, not code. |
| `pricing-strategy` | business | https://github.com/emotixco/claude-skills-founder | Your link was a v1 stub; live skill moved to skills/pricing-strategy/SKILL.md. Claude-plugin file paths do not exist in Hermes so the founder/ folder discipline degrades, core instructions work. |
| `better-interface` | ui | https://github.com/trycompai/crm | Orchestrator for the seven better-* design skills. Reviewer had reported the path as apps/agent/agent/skills/ - that is 404. Correct path is .agents/skills/. |
| `better-accessibility` | ui | https://github.com/trycompai/crm |  |
| `better-layout` | ui | https://github.com/trycompai/crm |  |
| `better-typography` | ui | https://github.com/trycompai/crm |  |
| `better-colors` | ui | https://github.com/trycompai/crm |  |
| `better-writing` | ui | https://github.com/trycompai/crm |  |
| `better-ui` | ui | https://github.com/trycompai/crm |  |
| `aria-icons` | ui | https://github.com/LeulAria/Aria-Icons | Icon catalog count verified from hosted icons-meta.json: 409,882 icons / 265 sets. README says 400+, CLI says 340k+, your link said 380,000+ - the docs disagree with each other. |
| `convert-documents-to-markdown` | productivity | https://github.com/firecrawl/anydoc | Overlaps Hermes native doc reading. Useful as a pipeline path for legacy formats. Hosted OCR would upload whole documents - needs your approval for client material. |
| `multicam` | media | https://github.com/aipauloshimas/multicam | Installed as `media/main` because the upstream SKILL.md has no `name:` field; renamed to `multicam` after install. Its frontmatter `name: multicam` means the internal name was right but the directory was wrong. Confirm Gemini Omni subscription before the render step. |

## Saved as reference, not installed

| Item | Verdict | Why |
|---|---|---|
| 2 · openworker | already-covered | Generic agent skills duplicate installed Hermes ones; beta with unsigned Windows builds. |
| 5 · hydradb | save-reference | No SKILL.md. Good data-eng architecture reference. |
| 6 · Graft | save-reference | Graphify already covers code-graph context. Skill fights Hermes verification habits; telemetry on by default. |
| 8 · open-kritt | save-reference | Trust-boundary study worth reading. Unauthenticated backend + root containers. |
| 9 · Echo-Music | skip | Unofficial YouTube client, credential-like constants in build file, no skill. |
| 10 · heyform | save-reference | Real freelance intake value later. Self-hosted form builder. |
| 12 · pocketbase | save-reference | No skill. Solid backend reference. |
| 14 · Compositor | skip | macOS-native, impossible on Windows. |
| 15 · openbot | save-reference | OPENBOT_SINGLE_USER=true admits everyone as admin. No skill installable. |
| 17 · svix-webhooks | save-reference | No skill. Webhook delivery reference. |
| 18 · alphai-tui | save-reference | No skill. TUI reference. |
| 20 · uptimepage | save-reference | Compose is explicitly non-production: no TLS, open metrics, dev DB creds. AGPL-3.0. |
| 21 · capd | skip | macOS-native, impossible on Windows. |
| 22 · ocis | skip | Zero SKILL.md. Windows removed from CI/releases. |
| 23 · llama.cpp | save-reference | Skills target llama.cpp contributions, not daily Python/SQL work. |
| 24 · hindsight | save-reference | Another memory system on top of Hermes/Obsidian. Backend-bound. |
| 25 · magpie | already-covered | No skill. Provider proxy - changes credentials and routing. |
| 31 · orca | already-covered | Most skills are runtime discovery stubs. Another orchestration layer you declined. PostHog telemetry. |
| 32 · hackingtool | save-reference | Unusable on Windows by its own README. Kept for its anti-fabrication / untrusted-tool-output rules. |
| 33 · ahmia.fi | skip | Tor search engine for illegal content. Out of scope. |
| 34 · emailosint.org | skip | Person-targeted breach/infostealer lookups. Out of scope. |
| 35 · leakix.net | save-reference | One genuinely useful defensive service - own assets only, key in env. |
| 36 · argus | skip | Mixed offensive modules: email harvesting, form grabber, WAF bypass, session hijacking. |
| 37 · gitgraber | save-reference | Secret-pattern checklist only. Never run its GitHub-wide sweep. GPL-3.0. |
| 40 · arcads-claude-code | saved-reference | Paid Arcads API + metered credits, bash-only scripts, affiliate signup links. |
| 44 · claude-watch | save-reference | Method is good (scene frames, pacing metrics, hook microscope). Hardcodes author vault paths and rm -rf inside it. |
| 45 · screenshot-to-code | save-reference | Screenshot-to-code reference. Worth it when a visual target matters. |
| 47 · lukegarvai.gumroad.com | save-reference | Gumroad storefront, no inspectable skill. |
| 48 · docs.prismml.com | save-reference | Bonsai 2 27B needs PrismML llama.cpp fork; stock builds refuse PQ2_0/PTQ1_0. |
| 49 · zerasoftwarestudio.com | skip | Paid masterclass. Scarcity claim and revenue testimonials unverified. |
| 51 · maidz.itch.io | save-reference | Game. AJESTREMIA. |
| 53 · Foreman | save-reference | Foreman - supervises Jev agents. Defaults to heavy GPU paths. Reference-first, no local-orchestration lead. |
| 54 · Open-glean | save-reference | Open-glean - searchable AI workspace on Hydra DB (Next.js 16). Reference-first. |
| 55 · Openjev | save-reference | Openjev - typed probabilities/confidence. Needs >=24GB NVIDIA; MLX is Apple-only. Reference-first. |
| 56 · Aria-Icons | install-skill | Aria-Icons. |
| 57 · Repolyze | already-covered | Repolyze is selected-file analysis, not a full audit. Already covered. |

## Saved to references/ for manual install

- `img2threejs__SKILL.md` — image to procedural Three.js. Install only with the full forge/grimoire/docs bundle; the markdown alone is not runnable.
- `iFixAi__ifixai__SKILL.md` — behavioral agent auditing. Stage only; no plugin hooks. Require sandbox + budget preview + approval.
- `fframes__fframes-video__SKILL.md` — video. Windows needs FFmpeg shared build, FFMPEG_DIR, LLVM, LIBCLANG_PATH. Low priority.
- `brigade__lead-scout__SKILL.md` — lead prospecting for freelancing. MUST EDIT: it treats failed searches as proof of "no website"; change to "no independent site found", log queries/date/confidence.
- `brigade__openai-whisper__SKILL.md` — local transcription/SRT. Homebrew-only install metadata must be replaced. `--task translate` is non-English to ENGLISH only, never `turbo`/`.en`.
- `paperclip__design-critique__SKILL.md` — prioritized UX/a11y critique.
- `brag__brag-slim__SKILL.md` — OpenMontage already covers HyperFrames video production.
- `diffusionstudio editor/watch` — Mac app-bundle paths (`Diffusion Studio.app/Contents/Resources/docs`), Windows resource paths unresolved. Not usable yet.

## Corrections made during review

- Reviewer 1 reported the design skills at `apps/agent/agent/skills/` — that path is 404. Real path is `.agents/skills/`.
- `multicam` shipped with no frontmatter `name:`, so Hermes named the directory `main`. Renamed to `multicam`.
- Aria-Icons count: README says 400+, CLI says 340k+, your list said 380,000+, hosted metadata says 409,882. Four different numbers; the hosted one is measured.
- Source typo: your list said "DiffusionGamma" for Openjev. The repo actually uses NVIDIA/Google **DiffusionGemma 26B-A4B**. Recorded, not silently fixed.

## Second pass - overlaps resolved and held-back items installed

### Overlap: kept both, scoped so they cannot collide
| Both installed | Split |
|---|---|
| `better-interface` (+6) vs `design-critique` | `better-interface` for audits and full cross-discipline reviews. `design-critique` for one fast 9-point pass on one screen. A scope note at the top of `design-critique/SKILL.md` says pick one; better-interface wins on "audit" or "full review". |
| `brag-slim` vs `openmontage` | `brag-slim` = zero-dependency single-file launch video from a project dir or URL. `openmontage` = full HyperFrames production pipeline. Scope note added. |
| `openai-whisper` vs `youtube-content` | Different inputs. Whisper = your own local audio files, produces SRT/VTT. youtube-content = a YouTube URL, produces text artifacts. No conflict. |
| `openai-whisper` vs `songsee` | songsee analyses audio, whisper transcribes it. Complementary. |
| `anti-koshary` vs `project-full-refactor` | anti-koshary = audit-first, nothing changes without approval, consequence-based findings, refuses to say "safe" without tests. project-full-refactor = fixes immediately, parallel subagents, POS/PySide6 specifics. Different contracts; keep both. |

### Overlap: rejected in favour of what Eli already had
| Rejected | Because |
|---|---|
| llama.cpp `code-review` / `add-new-model` | Targets llama.cpp contributions. Eli's day job is Python/SQL/DE. |
| Hindsight memory skills | Another memory layer on top of Hermes memory + Obsidian vault. |
| Graft | `graphify` already provides code-graph context. |
| Repolyze | Selected-file analysis with an OpenRouter call, not a full audit. `anti-koshary` and `requesting-code-review` are better and local. |
| iFixAi's "audit your agent" idea vs `strix-security-testing` | Different: Strix scans code, iFixAi probes a running agent's behaviour. Both installed, no conflict. |

### Installed in this pass (6 of 7)
`ifixai` (software-development) - `lead-scout` (business) - `openai-whisper` (media) - `design-critique` (ui) - `brag-slim` (creative) - `img2threejs` (creative)

Two were patched before use, not just installed:
- `lead-scout`: upstream treats "only social/aggregator results" as proof of no website. Changed to "no independent site found", requires logging queries + date + confidence, and a second confirmation method before acting.
- `openai-whisper`: replaced Homebrew-only install metadata with pip/winget, and documented that `--task translate` outputs ENGLISH only - it cannot produce Arabic.

### Blocked, and it is not overridable
`fframes-video` returned verdict **DANGEROUS**, 4 findings:
- CRITICAL supply_chain - `curl -fsSL <url> | bash` at SKILL.md:48
- HIGH privilege_escalation - `sudo apt-get install` at :35, `sudo pacman -S` at :37
- MEDIUM execution - backtick subshell at :255

Hermes refuses `--force` on a dangerous verdict ("Hermes never installs unverified skills with high-risk findings, even with --force"). anti-koshary was overridable because it was CAUTION; DANGEROUS is a different tier. Left un-installed deliberately - the curl-pipe-bash is a real supply-chain risk and fframes needs a Rust + LLVM + FFmpeg toolchain on Windows that Eli does not have. The markdown is kept in `references/fframes__fframes-video__SKILL.md` for manual install.

### img2threejs needs its repo
The installed SKILL.md is a router. It calls `forge/next.py`, `forge/state.py`, and files under `grimoire/` and `docs/` that are NOT bundled. A note at the top of the installed file says to clone the repo before use.

## Third pass - installed what is useful AND unique (2026-10-03)

Rule applied: a skill had to be genuinely additive to what Eli already has. "Exists and is good" was not enough.

### Installed (+3, now 21 total)
| Skill | Category | Why it is unique here |
|---|---|---|
| `wireframe` | creative | Low-fi B/W SVG wireframes with a locked house style (1.5px black stroke, 8px grid, fixed type scale). Nothing installed did structural mockups. All 6 companion files came down: `references/components.md`, `references/grid-system.md`, `references/examples.md`, `assets/template.svg`, `assets/template-mobile.svg`, `assets/site-template.html`. |
| `release-announcement` | communication | Per-surface shapes - a changelog entry is not a blog post is not a social card - leading with user impact. Not covered by any writing skill Eli has. Paperclip Cases API block removed as dead weight for Hermes. |
| `reliability-concurrency` | software-development | Advisory locks, idempotent job handlers, race-safe replace-writes, fail-loudly. Written for ChatbotX but the *patterns* are generic and directly relevant to Eli's data-engineering path. Origin caveat recorded in the file. |

### Deliberately NOT installed despite being installable
| Candidate | Why not |
|---|---|
| `shadcn` (shadcn-ui/ui) | Scanned CAUTION - overridable - but it fails the uniqueness bar anyway. React + Tailwind component library; Eli is on Python/SQL/DE with no web project. Installed only if he builds a Next.js app. |
| `simplified-english` | Collides with `humanizer` (already installed, 34 patterns, far deeper) and with `better-writing`. ASD-STE100 is an aerospace-documentation standard, not what Eli writes. The reviewer flagged that claiming STE100 compliance without the full controlled vocabulary is a false claim. |
| `business-data-access` | Real skill, but 100% ChatbotX-specific: `@chatbotx.io/business`, `apps/builder`, their cache-tag API. Would misfire on Eli's Python repos. Eli's own `data-access-layer-consistency` (SQLAlchemy) is the relevant one. |
| `worker-development`, `contact-filter`, `integration-channel`, `drizzle-database` | All hardcode ChatbotX internals - BullMQ queue names, their file paths, their Zod schemas. Useless outside that repo. |

**Total installed: 21. Hermes now reports 139 enabled.**
