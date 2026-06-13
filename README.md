# Saurabh Chaturvedi Portfolio — Rebuild & Edit Master Prompt

> Keep this document saved. Whenever you need to edit or fully rebuild the portfolio, paste the relevant section below into Claude along with the required files.

---

## 🔗 Important URLs

| What | URL |
|------|-----|
| Live Portfolio | https://saurabh-chaturvedi-portfolio.netlify.app |
| Netlify Dashboard | https://app.netlify.com/projects/saurabh-chaturvedi-portfolio |

---

## 🛠️ Tech Stack

- **Frontend:** Single HTML file — vanilla JS + CSS, no frameworks
- **Fonts:** Google Fonts — Cormorant Garamond + DM Sans
- **Hosting:** Netlify Drop
- **Charts:** No external libraries — replaced with CSS stat bar rows
- **Assets:** All images and videos embedded as base64 inside the HTML file

---

## 🎨 Design System

| Element | Value |
|---------|-------|
| Primary font | Cormorant Garamond (serif, display) |
| Body font | DM Sans |
| Gold accent | #C4A35A |
| Background | #0a0a0a (dark sections) |
| Light sections | #F7F6F3 |
| Border colour | rgba(255,255,255,0.06) |

---

## 📁 What's Inside the Current HTML File

### Images (16 total — all base64 embedded)
1. Faucek — Write Stories. Shape Minds.
2. Faucek — Without Digital Marketing, No One Will
3. Faucek — Content Matters. But Why?
4. Faucek — Without Marketing, Ads Are Noise
5. Faucek — Creativity Is Built, Not Born
6. Faucek — Blank Pages Are Opportunities
7. Faucek — Build Apps That Users Love
8. Faucek — Think Less Rules. More Resonance.
9. Faucek — Visual Identity Post
10. Faucek — Brand Awareness Post
11. Faucek — Engagement Creative
12. Faucek — Campaign Visual
13. SharpEagle — Eid-Al-Fitr Mubarak
14. Studio 52 — Capture. Create. Communicate. (CEO video post)
15. SharpEagle — International Labour Day
16. SharpEagle — Forklift Alert Systems

### Videos (6 MP4 — base64 embedded, preload="metadata" for fast load)
1. Faucek — Brand Campaign Video
2. Faucek — Content Creator Series
3. CreateX Agency — Internship Journey
4. Studio 52 — Brand Video
5. AIMT — Guest Session Coverage
6. AIMT — Podcast Session

### YouTube Videos (3 — TRITENT channel, load from YouTube servers)
- `zR4OYxYUVtk` — Medusa: The Curse of Athena (Mystery & The Unexplained)
- `M8KrdjQFewA` — The Immortal Ashwathama (Forgotten History)
- `P_XBsfGO34U` — The Mystery of a Little Girl (Horror Stories)

### Blog Articles (4 — full text embedded, open in overlay)
1. Udaan Raises $114M — Faucek (Fintech / Startup Analysis)
2. Slikk Raises $10M — Faucek (Quick Commerce / Consumer Tech)
3. Cabinets To Go vs Home Depot — CreateX Agency (SEO / Home Improvement)
4. 30 Funky Painted Furniture Ideas — CreateX Agency (SEO / Lifestyle)

---

## 📊 Current Content Data

| Metric | Value |
|--------|-------|
| Total emails deployed | 74,449 |
| Campaigns run | 56 |
| Avg open rate (Studio 52) | 26.9% |
| Avg open rate (SharpEagle) | 26.2% |
| Industry avg open rate | ~21% |
| Total qualified replies | 38 (22 S52 + 16 SE) |
| LinkedIn prospects | 241 |
| LinkedIn accepted | 25 |
| LinkedIn acceptance rate | 10.4% |
| Content pieces produced | 250+ |
| YouTube videos (TRITENT) | 33 |
| Portfolio images | 16 |
| Portfolio videos (MP4) | 6 |

---

## 🔑 Personal Details

| Field | Value |
|-------|-------|
| Name | Saurabh Chaturvedi |
| Email | schaturvedi472@gmail.com |
| Phone | +91-7879151506 |
| LinkedIn | linkedin.com/in/saurabh-chaturvedi-7a4666190 |
| YouTube | @mysterioustritent581 |
| Location | MP, India · Open to Relocation |
| MBA | Army Institute of Management & Technology · CGPA 8.2 |
| B.Pharm | Jiwaji University · 76.58% |

---

## ⚠️ Known Considerations

| # | Note | Detail |
|---|------|--------|
| 1 | File size is ~63MB | Because all videos are embedded as base64. Normal for self-contained portfolio. |
| 2 | GitHub 25MB limit | Cannot upload directly to GitHub. Use Netlify Drop only. |
| 3 | Videos use preload="metadata" | Only loads a tiny thumbnail frame on page load — not the full video. Same method as v2 which runs fast. |
| 4 | YouTube thumbnails need internet | They load from img.youtube.com, not embedded locally. |
| 5 | No Chart.js | Removed to fix page lag. All campaign data shown as CSS stat bar rows instead. |
| 6 | Custom cursor disabled on mobile | Correct — mobile has no cursor. Portfolio is fully responsive. |

---

---

# ✏️ HOW TO EDIT THE PORTFOLIO

## Quick Text Edits (no rebuild needed)

For simple text changes — open the HTML file in VS Code, use `Ctrl+F`, find the text, change it, save, and re-upload to Netlify.

**Update hero stats:**
Search `hstat-n` — four stat blocks. Edit the numbers directly.

**Update contact details:**
- Search `schaturvedi472@gmail.com` — appears 3 times, update all
- Search `7879151506` for phone
- Search `saurabh-chaturvedi-7a4666190` for LinkedIn

**Update experience bullets:**
Search for the company name (e.g. `Studio 52`) inside the `id="experience"` section and edit the `<li>` items directly.

**Add a new certification:**
Search for `Certifications` and add a new row:
```html
<div class="cr2">
  <span class="cn">Your Certification Name</span>
  <span class="ci">Issuer · Year</span>
</div>
```

**Add a new LinkedIn outreach card:**
Search for `id="linkedin"` and copy an existing `.li-card` block. Update the person name, role, company, page visited, connection note, and DM text.

---

---

# 🔄 FULL REBUILD / MAJOR UPDATE — PASTE THIS INTO CLAUDE

> Use this prompt when you want Claude to do a proper rebuild with new content, new images, new videos, or structural changes. Upload the required files listed below before pasting the prompt.

---

## 📂 FILES TO UPLOAD BEFORE PASTING THE PROMPT

Upload these files to Claude before sending the rebuild prompt. The more files you provide, the more complete the rebuild.

### Always Required
- [ ] **Current portfolio HTML file** — `saurabh_portfolio_v5_final.html` (so Claude can extract all existing base64 assets and CSS)
- [ ] **Resume PDF** — `Resume_Saurabh_Chaturvedi.pdf` (for the resume download button)

### Required for Campaign Data Updates
- [ ] `EMAIL_TRACKER.xlsx` — campaign-level open rate and CTR data
- [ ] `EMAIL_REPLY_TRACKER.xlsx` — reply counts and priority flags
- [ ] `LINKEDIN_OUTREACH_TRACKER.xlsx` — prospect, accepted, message counts

### Required for Writing Sample Updates
- [ ] `FAUCEK.docx` — contains Udaan, Slikk, and other startup articles
- [ ] `cabinets_to_go_vs_home_depot.docx` — full SEO article
- [ ] `funky_painted_furniture_ideas.docx` — full SEO article

### Required for Email/LinkedIn Draft Updates
- [ ] `Draft_-_Sharpeagle.docx` — SharpEagle email campaign drafts
- [ ] `Drafts_Studio_52_Mails.docx` — Studio 52 email campaign drafts
- [ ] `LinkedIn_Outreach_Dec2025_Studio52.docx` — LinkedIn outreach messages

### For New Social Media Images (if updating the masonry grid)
- [ ] Upload new JPG/PNG images — Claude will embed them as base64

### For New Videos (if adding new MP4 videos)
- [ ] Upload new MP4 files — Claude will embed them as base64 using `preload="metadata"`

---

## 📋 THE REBUILD PROMPT

> Copy everything below this line and paste it into Claude after uploading your files.

---

I need you to rebuild / update my personal marketing portfolio as a single self-contained HTML file. The current portfolio file is attached — please extract all existing base64 images, videos, and the resume PDF from it so we don't lose any assets.

**My name:** Saurabh Chaturvedi
**Live URL:** https://saurabh-chaturvedi-portfolio.netlify.app

---

### DESIGN — Keep exactly as-is

- Apple × editorial dark aesthetic
- Cormorant Garamond (display) + DM Sans (body)
- Gold accent: #C4A35A
- Dark background: #0a0a0a (dark sections), off-white for light sections
- Custom gold cursor with smooth follower
- Animated scroll-triggered fade reveals (.rev / .revl classes with IntersectionObserver)
- Scrolling marquee ticker
- Nav: SC logo + links to sections, scrolled class on scroll
- Modal popup for: full-size images (click masonry), YouTube embed, MP4 video playback
- Article overlay for: 4 full blog articles (openArticle / closeArticle functions)
- Mobile responsive
- No Chart.js — use CSS stat bar rows for all campaign data

---

### SECTIONS — Keep all of these, in this order

1. **Hero** — name, title, 4 hero stats, Explore Work CTA, Resume download button (embedded PDF)
2. **Marquee** — scrolling ticker of skills/keywords
3. **Featured Work** — 6 cards linking to: Campaigns, LinkedIn, Creative (×3), Creator
4. **About (01)** — bio, education, skill tags, TRITENT YouTube card
5. **Experience (02)** — 4 roles: Studio 52, CreateX Agency, Faucek, GMH Organics
6. **Creative Work (03)** — masonry grid of 16 images + 4 blog article cards below
7. **Highlights** — 5 stat number blocks
8. **Campaigns (05)** — 4 metric strip stats + stat bar rows for campaign data + 4 tabbed email templates
9. **LinkedIn Outreach (06)** — 3 stat blocks + funnel bar display + 5 LinkedIn cards + strategy card
10. **Creator / Netflix dark (07)** — TRITENT feature card + 3 YouTube thumbnail cards + 6 MP4 video cards
11. **Tools (07)** — 8 tool blocks + certifications list
12. **Strategy (08)** — quote, 4 pillars, research papers stack
13. **Contact (09)** — contact details, availability block, what I bring list
14. **Footer** — one line
15. **Modal** — image/video/YouTube popup
16. **Article overlays** — 4 full articles (Udaan, Slikk, Cabinets, Funky) as hidden full-page overlays

---

### CONTENT — Use this data exactly

**Hero stats:**
- 74K+ Emails Deployed
- 56 Campaigns Run
- 241 B2B Prospects
- 250+ Content Pieces

**Experience:**

Studio 52 Media & Tech Group · Digital Marketing Executive · Feb 2026 – Present · Indore, India
- Executed 56 email campaigns deploying 74,449+ emails across GCC & UK markets
- Achieved avg open rate of 26.9% (Studio 52) and 26.2% (SharpEagle) — above 21% industry benchmark
- Identified & outreached 241 LinkedIn prospects — 10.4% cold connection acceptance rate
- Wrote multi-sequence B2B cold email campaigns for petroleum, manufacturing & safety sectors
- Managed WhatsApp marketing, press releases, and client communications
Tags: Email Marketing, LinkedIn Outreach, B2B Lead Gen, GCC & UK, Press Release

CreateX Agency · Content Marketer · Jun–Sep 2025 · Noida, India
- Produced 150 content pieces — 50 manual + 100 AI-assisted across multiple client verticals
- Boosted audience engagement by 25% through targeted content strategy
- Improved search visibility by 20% via SEO strategy and SERP monitoring
- Designed Canva visual assets; consistently delivered 15% ahead of deadlines
Tags: SEO Content, Blog Writing, AI Workflows, Canva, Content Strategy

Faucek · Digital Marketing Intern · May–Aug 2025 · Remote
- Wrote ~100 blogs and newsletters increasing content engagement by 20%
- Improved organic traffic by 25% via keyword research & on-page SEO
- Created 16+ social posts & videos published on Faucek's official LinkedIn brand page
- Analysed startup funding: Slikk ($10M), Udaan ($114M), Stable Money ($20M)
Tags: Blog Writing, On-page SEO, Social Media, Video Editing, Official Brand Content

GMH Organics · Marketing & Operations Intern · Apr–May 2021 · Baddi, India
- Supported market research and competitive landscape analysis
- Assisted in social media content creation and brand communications

**Campaign stat bar data (for CSS bar rows, no Chart.js):**

Studio 52 Open Rates:
- Food & Drink Expo: 40.6%
- PIE 2026 Follow-up: 39.2%
- Corporate Video: 37.6%
- UK Database: 36.2%
- Construction 1: 25.7%
- Construction 2: 25.1%
- Safety Videos: 25.1%
- UK Database 2: 21.8%
- Industry Average: ~21%

SharpEagle Open Rates:
- Day 3 Exproof: 46.3%
- Exproof PTZ: 43.9%
- Intersec Follow-up: 27.7%
- Ramadan 2026: 27.5%
- Eid Al-Fitr: 23.4%
- Crane Safety: 20.9%
- AI Forklift: 20.2%
- Exproof CCTV: 18.2%
- Industry Average: ~21%

Studio 52 CTR:
- PIE 2026 Follow-up: 26.0%
- Food & Drink Expo: 8.2%
- Construction: 5.7%
- Safety Videos: 5.6%
- Corporate Video: 4.7%
- Industry Average: ~2.5%

Reply breakdown:
- Studio 52 Replies: 22
- SharpEagle Replies: 16
- High-Priority Replies: 27
- Total Qualified Replies: 38

LinkedIn funnel:
- Identified: 241
- Requests Sent: 241
- Accepted (10.4%): 25
- Notes Sent: 16
- Messages Sent: 9
- Replied: 1

**Email tab campaigns (4 tabs):**

Tab 1 — SharpEagle · AI Forklift
From: Yash Malik <yash@mail-sharpeagle.com>
To: Warehouse & Logistics Decision-Makers · GCC + UK
Date: 24 Apr 2026 · Sent: 2,370 · Open: 20.21% · CTR: 6.74%
Subject: "AI is doing magic with Forklift Safety. Have you adopted?"
Body: Hi [First Name], Greetings from Yash. I work for SharpEagle Technology, one of the leaders in Industrial Safety solutions. SharpEagle's AI Forklift CCTV Solutions are designed to improve safety in high-risk environments like warehouses, logistics hubs, and manufacturing sites. With AI pedestrian detection, wide-angle cameras, and real-time monitoring, the system reduces blind spots, supports safer forklift movement, and helps operators respond quickly to surrounding activity. Here is the link to our different options — [LINK]. How about a short call to discuss further? Best regards, Yash · SharpEagle Technology
Tags: AI Forklift CCTV, 2,370 Contacts, GCC + UK, 20.21% Open Rate, 6.74% CTR

Tab 2 — SharpEagle · Exproof PTZ
From: Yash Malik <yash@mail-sharpeagle.com>
To: Oil & Gas, Exproof Sector · GCC + UK (787+ contacts)
Date: 25 Feb 2026 · Open: 43.90% · CTR: 9.76%
Subject: "Can your PTZ Camera handle Explosive Industrial Environments?"
Body: Dear [First Name], Greetings from Yash. I work for SharpEagle Technology, one of the leaders in Industrial Safety solutions. SharpEagle's Explosion Proof PTZ Camera is an ATEX & IECEx-certified solution built for hazardous industrial environments. With pan, tilt, and zoom capabilities, it delivers real-time, wide-area surveillance in areas where standard cameras simply cannot operate safely. Here is the link — [LINK]. How about a short call? Best regards, Yash Malik · SharpEagle Technology
Tags: ATEX & IECEx Certified, 787+ Contacts, GCC + UK, 43.90% Open Rate, 9.76% CTR

Tab 3 — Studio 52 · Petroleum GCC (3-email sequence)
From: Mike Brown <mike@mail-studio52.com>
To: Petroleum & Energy Decision-Makers · GCC (248 contacts)
Date: 25 May 2026 · 3-Email Sequence · MOFU
Subject: "Is your field team trained with the right content?"
Email 1: Hi [First Name], Greetings from Studio 52, one of the leading media production companies in the GCC. We work with petroleum and energy companies to produce safety training films, operational procedure videos, and internal communication content. Would love to get on a short call. Best regards, Mike · Studio 52
Email 2 subject: "Safety & training videos for your field teams" — Dear [First Name], I wanted to circle back. We have worked with several leading energy companies across the GCC and would love to discuss how we can do the same for your organisation.
Email 3 subject: "One last note regarding your training videos" — Dear [First Name], If producing professional video content for your team is on your radar, we would love to be the ones to help.
Tags: 3-Email Sequence, 248 Contacts, Petroleum GCC, Studio 52

Tab 4 — Studio 52 · Safety Animation UK (3-email sequence)
From: Mike Brown <mike@mail-studio52.com>
To: Safety & Training Decision-Makers · UK (311 contacts)
Date: 26 May 2026 · 3-Email Sequence · MOFU
Subject: "Making safety training easier to understand"
Email 1: Hi [First Name], Greetings from Studio 52, a media production company specialising in safety and training video production. We work with UK organisations to create safety animation content that simplifies complex procedures and improves training retention. Would love to get on a short call. Best regards, Mike · Studio 52
Email 2 subject: "Is your team actually retaining safety training?" — Dear [First Name], Just circling back. We have helped several organisations across the UK produce safety content that is HSE-compliant and built for multilingual teams.
Email 3 subject: "Ready to improve your safety training experience?" — Dear [First Name], If safety animation is something your organisation is looking to invest in, we would love to help.
Tags: 3-Email Sequence, 311 Contacts UK, HSE-Compliant, Studio 52

**LinkedIn outreach cards (5 cards + 1 strategy card):**

Card 1 — Ismail Shilleh, General Manager Qatar, Al-Bahar · Page: Video Production
Note (76 chars): "Hi Ismail, saw you visited our video production page. Would love to connect!"
DM: Hi Ismail, I'm Muneera from Studio 52. I noticed you visited our video production page recently. We create clean, professional, result-oriented videos for UAE companies. Can I share recent examples if you're working on anything video-related? Best, Muneera

Card 2 — Omar Talal Hariri, CEO, SAL · Page: Drone Filming
Note (71 chars): "Hi Omar, saw you visited our drone filming page. Would love to connect!"
DM: Hi Omar, I'm Muneera from Studio 52. I noticed you visited our drone filming page recently. We create high-quality drone videos and aerial content for companies in Saudi Arabia. Happy to share examples if you have any drone projects in the pipeline. Best, Muneera

Card 3 — Aya Medhat Moustafa, Director of Arabic Content Acquisitions, MBC Group / Shahid · Page: Arabic Voiceover
Note (73 chars): "Hi Aya, saw you visited our Arabic voiceover page. Would love to connect!"
DM: Hi Aya, I'm Muneera from Studio 52. I noticed you visited our Arabic voiceover page recently. We create natural, broadcast-quality Arabic voiceovers. Can I share recent examples? Best, Muneera

Card 4 — Kristy Markel, Director of Marketing and Operations, Realty Austin · Page: On-Hold Messages
Note (75 chars): "Hi Kristy, saw you visited our on-hold message page. Would love to connect!"
DM: Hi Kristy, I'm Muneera from Studio 52. I noticed you visited our on-hold messages page recently. We create professional, branded on-hold audio content. Happy to share examples. Best, Muneera

Card 5 — Fatih Bahadir Guner, Head of Digital Transformation, Al-Bahar Dubai · Page: Video Production
Note (75 chars): "Hi Fatih, saw you visited our video production page. Would love to connect!"
DM: Hi Fatih, I'm Muneera from Studio 52. I noticed you visited our video production page recently. We create clean, professional videos for UAE companies. Happy to share examples. Best, Muneera

Strategy card: Dec 2025: 146 requests → 16 accepted (10.96%) · Jan 2026: 95 → 9 accepted (9.47%) · Overall: 10.4% cold acceptance rate vs LinkedIn cold avg of 5–8%
Steps: Identified page visitors via Lead Forensics → Matched company visitor data to LinkedIn profiles → Wrote personalised connection note referencing the exact page visited (under 100 chars) → Sent DM post-acceptance with relevant service angle and CTA

**YouTube cards (3 — TRITENT):**
- Mystery & The Unexplained · youtube.com/watch?v=zR4OYxYUVtk
- Forgotten History · youtube.com/watch?v=M8KrdjQFewA
- Horror Stories · youtube.com/watch?v=P_XBsfGO34U
(Use img.youtube.com/vi/VIDEO_ID/maxresdefault.jpg for thumbnails with onerror fallback)

**MP4 video card labels (6 cards — extract base64 from current HTML):**
1. Faucek · Official Content — Brand Campaign Video
2. Faucek · Social Media — Content Creator Series
3. CreateX Agency — Internship Journey
4. Studio 52 · Media Production — Brand Video
5. AIMT · Official LinkedIn — Guest Session Coverage
6. AIMT · Official LinkedIn — Podcast Session

**Tools (8):** ChatGPT (AI Content), Claude (AI Strategy), Gemini (AI Research), Perplexity (AI Search), Canva (Visual Design), Google Analytics (Data & Insights), Google Ads (Paid Media), MS Excel (Data Analysis)

**Certifications:** Google Analytics · Google Ads Apps · HubSpot Marketing · Microsoft Excel Specialist · AI in Marketing · Social Media Marketing · E-Business · Business Analytics with Excel · NPTEL Certifications (IIT India · Multiple)

**Research papers (4):**
- Streaming Platforms & Global Entertainment Transformation · Feb–May 2026
- Consumer Perception Towards Influencer Collaboration · Aug–Nov 2025
- Impact of Online Reviews on Consumer Purchase Decision · Jan–May 2025
- Video content for AIMT's official LinkedIn page · Convocation · Guest Sessions · Podcast · 2024

**Contact:**
- Email: schaturvedi472@gmail.com
- Phone: +91-7879151506
- LinkedIn: linkedin.com/in/saurabh-chaturvedi-7a4666190
- YouTube: @mysterioustritent581 · TRITENT
- Location: MP, India · Open to Relocation
- Open to: growth marketing, content strategy, and digital marketing roles. Graduating MBA 2026. Immediate joining available.

---

### IMAGES — Extract all 16 from the current HTML file
(All are already base64-embedded. Re-use them in the same order in the masonry grid.)

Labels in order:
1. Faucek · Brand Campaign — Write Stories. Shape Minds.
2. Faucek · Official LinkedIn — Without Digital Marketing, No One Will
3. Faucek · Educational Content — Content Matters. But Why?
4. Faucek · Brand Messaging — Without Marketing, Ads Are Noise
5. Faucek · Personal Brand Post — Creativity Is Built, Not Born
6. Faucek · Editorial Design — Blank Pages Are Opportunities
7. Faucek · Product Campaign — Build Apps That Users Love
8. Faucek · Quote Card — Think Less Rules. More Resonance.
9. Faucek · Social Media — Visual Identity Post
10. Faucek · Social Media — Brand Awareness Post
11. Faucek · Social Media — Engagement Creative
12. Faucek · Social Media — Campaign Visual
13. SharpEagle · Brand Campaign — Eid-Al-Fitr Mubarak
14. Studio 52 · Brand Content — Capture. Create. Communicate.
15. SharpEagle · Brand Awareness — International Labour Day
16. SharpEagle · Product Campaign — Forklift Alert Systems

### VIDEOS — Extract all 6 from the current HTML file
(All are already base64-embedded. Re-use them with preload="metadata" and data-src for fast page load.)

### RESUME — Extract the PDF base64 from the current HTML file
(It's already embedded. Re-use it for the Download Resume button in the hero.)

### BLOG ARTICLES — Embed full text of all 4 articles
(Extract the full article content from the current article overlay divs in the HTML. Keep all headings, paragraphs, tables, and FAQs.)

---

### TECHNICAL REQUIREMENTS

- **Single HTML file** — everything embedded, no external dependencies except Google Fonts CDN
- **No Chart.js** — use CSS horizontal bar rows for all campaign data (the `.sr`, `.sr-bar`, `.sr-val` pattern)
- **Video loading** — use `preload="metadata"` + `data-src` attribute on all MP4 videos. Do NOT put video base64 in any `<script>` tag — this causes lag. The `openM('mp4', this.dataset.src, '')` onclick pattern is correct.
- **Image loading** — use `loading="lazy"` on all masonry images
- **Performance** — the page should render instantly. Videos are heavy (total ~59MB) but preload=metadata ensures only a tiny frame loads. The rendered page weight should be under 1MB.
- **Hosting** — output must be uploadable to Netlify Drop as a single file

---

> After Claude builds the file, download it and drag-and-drop to https://app.netlify.com/projects/saurabh-chaturvedi-portfolio — live in 30 seconds.
