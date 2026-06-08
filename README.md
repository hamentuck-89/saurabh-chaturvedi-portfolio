Saurabh Chaturvedi Portfolio 🗂️
A premium personal portfolio website built as a single HTML file with all assets embedded.
🔗 Important URLs
WhatURLLive Portfoliohttps://saurabh-chaturvedi-portfolio.netlify.appNetlify Dashboardhttps://app.netlify.com/projects/saurabh-chaturvedi-portfolio
🛠️ Tech Stack

Frontend: Single HTML file (vanilla JS + CSS, no frameworks)
Fonts: Google Fonts — Cormorant Garamond + DM Sans
Hosting: Netlify Drop
Assets: All images and videos embedded as base64 inside the HTML file

✨ Features

Custom gold cursor with smooth follower
Animated scrolling marquee ticker
Full-bleed masonry image grid (click → fullscreen modal)
Video popup player (YouTube embed + MP4 playback)
Scroll-triggered fade animations
Mac-style email campaign preview mockup
8 sections: Hero, About, Experience, Creative, Campaigns, Videos, Tools, Strategy, Contact
Fully responsive (mobile + desktop)

📁 What's Inside the HTML File
All of the following are base64-encoded directly inside index.html:
Images (13 total — Faucek social media posts):

Writing Stories That Matter
Write Bold Think Deep
Create Like No One's Scrolling
Your Weirdest Ideas
Creativity Doesn't Need Permission
Creativity Is a Vibe
Blank Pages Are Opportunities
Creativity Thrives in Chaos
Think Less Rules More Resonance
Write Stories Shape Minds
Some Days Flow I Still Create
Creativity Is Built Not Born
Content Matters But Why
Without Digital Marketing No One Will
Without Marketing Ads Are Noise
Build Apps That Users Love

Videos (7 embedded + 3 YouTube):

faucek_1.mp4 — Faucek brand campaign video
faucek_2.mp4 — Faucek content creator series
createx.mp4 — CreateX Agency internship journey
studio52.mp4 — Studio 52 brand video
aimt_2.mp4 — AIMT guest session coverage
aimt_3.mp4 — AIMT podcast session
YouTube: zR4OYxYUVtk, M8KrdjQFewA, P_XBsfGO34U (TRITENT channel)

🚀 How to Update the Portfolio
To update text content (job title, bio, achievements, new role):

Download index.html from Netlify or keep a local copy
Open in any text editor (VS Code recommended)
Use Ctrl+F to search for the exact text you want to change
Edit and save
Go to app.netlify.com/projects/saurabh-chaturvedi-portfolio
Drag and drop the updated file in the "drag and drop" box
Live in 30 seconds

To add a new job/experience:

Search for <!-- EXPERIENCE --> in the file
Copy an existing .erow block and paste below the last one
Update company name, role, period, bullets, and tags

To add new images:

Convert image to base64: go to base64.guru/converter/encode/image
Upload your image → copy the base64 output
Add to the images section: <img src="data:image/jpeg;base64,PASTE_HERE">
Add it as a new .mi2 block inside the masonry grid

To add new videos:
YouTube video:

Find an existing YouTube .vc block in the Videos section
Copy it, change the video ID to your new YouTube video ID
Update the thumbnail URL: https://img.youtube.com/vi/YOUR_VIDEO_ID/maxresdefault.jpg

MP4 video:

Convert to base64: use Python locally:

pythonimport base64
with open('your_video.mp4','rb') as f:
    print('data:video/mp4;base64,' + base64.b64encode(f.read()).decode())

Paste the output as the src in a new .vc block and data-src attribute

To add a new certification:

Search for Certifications in the file
Add a new .cr2 row:

html<div class="cr2">
  <span class="cn">Your Certification Name</span>
  <span class="ci">Issuer · Certified</span>
</div>
To update stats on the hero (250+, 6K+, etc.):

Search for hstat-n in the file
Four stat blocks — edit the numbers directly

To change contact details:

Search for schaturvedi472@gmail.com — appears 3 times, update all
Search for 7879151506 for phone
Search for saurabh-chaturvedi-7a4666190 for LinkedIn

🔄 Full Rebuild Instructions
If you ever need to rebuild this from scratch (new laptop, lost the file, major redesign), paste this into Claude:

"I need to rebuild my marketing portfolio. Here is my full profile data: [paste your resume]. My name is Saurabh Chaturvedi. The portfolio should have: premium luxury aesthetic, black background hero, gold accents (#C4A35A), Cormorant Garamond + DM Sans fonts, custom cursor, marquee ticker, masonry image grid, video popup player, scroll animations. Sections: Hero, About, Experience, Creative Work, Campaigns, Videos, Tools & Certs, Brand Strategy, Contact. All as a single self-contained HTML file."

Then upload all your image and video files and ask Claude to embed them as base64.
🎨 Design System
ElementValuePrimary fontCormorant Garamond (serif, display)Body fontDM SansGold accent#C4A35AGold light#E8D5A3Background#080808 (hero), #FAFAF8 (sections)Light section#F2F0EBBorder#E2DED6
📊 Content Data
MetricValueTotal content pieces250+Emails deployed6,000+LinkedIn prospects241LinkedIn accept rate10.4%Campaigns managed70+Brands served4YouTube videos33Portfolio images13Portfolio videos10
🐛 Known Considerations
#NoteDetail1File size is ~60MBBecause all videos are embedded. Normal for a portfolio with video.2GitHub 25MB limitCan't upload directly to GitHub. Use Netlify Drop instead.3AIMT video 1 not embeddedFile was 17MB — too large. Not included to keep size manageable.4YouTube videos need internetThey load from YouTube's servers, not embedded locally.5Custom cursor disabled on mobileCorrect — mobile has no cursor. Portfolio is still fully responsive.
🔑 Personal Details
FieldValueNameSaurabh ChaturvediEmailschaturvedi472@gmail.comPhone+91-7879151506LinkedInlinkedin.com/in/saurabh-chaturvedi-7a4666190YouTube@mysterioustritent581LocationMP, India · Open to RelocationMBAArmy Institute of Management & Technology · CGPA 8.2B.PharmJiwaji University · 76.58%
