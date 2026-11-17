# Nikhil Natesh — Portfolio

A responsive, futuristic portfolio built for free GitHub Pages hosting. No build step, dependencies, API keys, or paid backend.

## Publish with GitHub Pages
1. Sign in at https://github.com and create a **public** repository named `nikhilnatesh.github.io` under NikhilNatesh.
2. Extract this ZIP. Upload the **contents** of this folder to the repository root (index.html must be at the top level, not inside another portfolio folder). Include the assets folder, app.js, style.css, and resume-data.js.
3. Commit the files to the main branch.
4. Open repository Settings → Pages. Select Deploy from a branch, main, /(root), then Save.
5. Wait for deployment. The portfolio address is https://nikhilnatesh.github.io/ . It is not live until this step completes.

## Resume assistant
This is a local, extractive resume-search assistant, NOT a generative LLM. It matches question keywords and common aliases against the full supplied resume, returns exact passages with section labels, and handles overview, education, contact, and certificate questions. It may return partial matches and does not infer undocumented experience, years per tool, salary, visa, or availability. Recruiters can ask arbitrary questions, but nuanced reasoning and conversational follow-ups require a future server-backed LLM integration. Do not put an API key in these public files.

## Content
- The experience chronology and claims follow the uploaded resume, including its current-role label.
- Six unique supplied certificate screenshots are included. The duplicate prompt-engineering certificate is omitted.
- The original resume is downloadable as DOCX. Certificate viewers crop out the phone interface and black margins using an SVG viewport, preserving the original certificate text and image pixels.
- Case studies summarize resume-listed work; no confidential implementation or invented metrics are included.
- Email, phone (in the resume/chat), employment, education, and certificate details will be public on deployment.
- Google Fonts is optional: the site uses system fallbacks offline. No analytics or chat logging is installed; messages remain in the current browser page only.

## Edit
Update visible career summaries and certificate metadata in app.js. Update resume-data.js when replacing the original resume in assets. Update headings in index.html and visual styling in style.css. Everything works as static files.

## Local preview
Open index.html directly, or run `python3 -m http.server 8000` from this folder and visit http://localhost:8000.

## Company logo sources
Logos identify employers listed in the supplied resume; trademarks belong to their respective owners.
- Capital One: SVG from https://www.capitalone.com/
- Express Scripts: https://www.express-scripts.com/modules/shared/evernorth_sdc/components/unity-navigation/assets/logo.svg
- Dell Technologies: https://i.dell.com/sites/csimages/Legal_Imagery/all/DellTech_Logo_Prm_Blue_rgb.png
- Ramco Systems: https://www.ramco.com/hubfs/website-assets/ramco-logo.png
Logo files are bundled locally for reliable rendering.
