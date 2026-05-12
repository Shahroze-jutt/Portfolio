# Shahroze Afzal | Automation Engineer Portfolio

> Production-grade automation engineer specializing in n8n, AI voice agents (Retell AI), and workflow automation. Building systems that scale without hiring.

**Live Demo:** [yourname.com](https://your-domain.com) | **LinkedIn:** [@shahroze-afzal](https://linkedin.com/in/shahroze-afzal)

---

## About

I'm an automation engineer focused on solving one problem: **How do you scale a business without scaling headcount?**

My specialty areas:
- 🤖 **AI Voice Agents** – Building 24/7 outbound qualification and inbound booking systems using Retell AI
- 📄 **Document Automation** – Extracting data from invoices, forms, contracts (OCR + Claude API)
- ⚙️ **Workflow Optimization** – n8n pipelines that save teams 5-40 hours per week

Every project is **production-ready**, fully tested, and designed for immediate deployment.

---

## 🎯 Featured Projects

### Lead Qualification Agent (Olivia)
Automated outbound voice system that calls new leads, runs MEDDIC-Lite qualification, and books qualified leads directly into the calendar.

- **Tech Stack:** n8n, Retell AI, Twilio, Cal.com, Airtable
- **Impact:** Reduced qualification time from days to minutes, 24/7 auto-calling
- **Files:** `workflows/lead-qualification-agent.json`

### Invoice Processing Automation
Document extraction pipeline that parses invoices (PDF/image) using OCR + Claude API and auto-populates spreadsheets.

- **Tech Stack:** Google Drive, Mistral OCR, Claude API, Google Sheets
- **Impact:** 4+ hours → 5 minutes per batch, 0 manual data entry
- **Files:** `workflows/invoice-processing.json`

### AI Booking Agent
Inbound phone system answering every call 24/7, booking appointments, rescheduling, and handling cancellations automatically.

- **Tech Stack:** n8n, Retell AI, Calendar, Twilio
- **Impact:** Zero missed calls, instant appointment booking
- **Files:** `workflows/ai-booking-agent.json`

### Data Sorting Automation
Pipeline that watches Google Drive for uploads, sorts messy data into categorized files, and emails results automatically.

- **Tech Stack:** Google Drive, JavaScript, Email
- **Impact:** 4+ hours → 5 minutes, eliminated manual sorting
- **Files:** `workflows/data-sorting.json`

### Customer Support Email Agent
Automated email system answering customer support questions 24/7 using Claude API.

- **Tech Stack:** Email Node, Claude API, n8n
- **Impact:** Instant responses, 24/7 coverage
- **Files:** `workflows/support-email-agent.json`

### Vapi Booking Agent
Multi-tool inbound phone system integrating Vapi, Cal.com, and Airtable for seamless appointment booking with CRM tracking.

- **Tech Stack:** Vapi, Cal.com, Airtable, n8n
- **Impact:** Multi-channel booking, real-time CRM sync
- **Files:** `workflows/vapi-booking-agent.json`

---

## 📊 Key Skills

### Automation Platforms
- **n8n** (advanced) – Workflow design, webhooks, APIs, conditional logic
- **Make.com & Zapier** – Automation flows
- **GoHighLevel** – CRM automation

### AI & LLMs
- **Retell AI & Vapi** – Voice agent design and deployment
- **Claude API** – Document processing, content generation
- **Prompt Engineering** – System design for LLM workflows

### Integration & APIs
- REST APIs & Webhooks
- JSON data handling
- Custom JavaScript in automation platforms
- HTTP requests & authentication

### Databases & CRM
- Airtable (bases, records, API)
- PostgreSQL & Supabase
- Google Sheets integration
- Custom data mapping

### Tools
- **Twilio** – Phone integration
- **Cal.com** – Calendar sync & booking
- **Google Drive & Sheets** – File handling
- **Email automation**

---

## 🚀 Quick Start

### Option 1: Deploy to Vercel (Recommended – Free)
1. Fork this repository
2. Go to [vercel.com](https://vercel.com)
3. Click "New Project" → Select your forked repo
4. Click "Deploy" (no config needed)
5. Your portfolio is live in ~1 minute

### Option 2: Deploy to GitHub Pages (Free)
1. Fork this repository
2. Go to **Settings** → **Pages**
3. Under "Source," select `main` branch
4. Click "Save"
5. Your portfolio is live at `https://yourusername.github.io/portfolio`

### Option 3: Deploy to Netlify (Free)
1. Go to [netlify.com](https://netlify.com)
2. Click "New site from Git" → Select your repository
3. Click "Deploy"
4. Your portfolio is live

### Option 4: Self-Host
```bash
# Clone the repo
git clone https://github.com/yourusername/portfolio.git
cd portfolio

# Start a local server (Python)
python3 -m http.server 8000

# Visit http://localhost:8000
```

---

## 📁 File Structure

```
portfolio/
├── index.html                    # Main portfolio website
├── README.md                     # This file
├── workflows/                    # n8n workflow exports (JSON)
│   ├── lead-qualification-agent.json
│   ├── invoice-processing.json
│   ├── ai-booking-agent.json
│   ├── data-sorting.json
│   ├── support-email-agent.json
│   └── vapi-booking-agent.json
├── case-studies/                # Detailed case study documents
│   ├── lead-qualification.md
│   ├── invoice-processing.md
│   └── data-sorting.md
└── docs/                        # Implementation guides
    ├── n8n-setup.md
    ├── retell-ai-guide.md
    └── deployment.md
```

---

## 🔧 Customization

### Edit Your Portfolio
1. Open `index.html` in any text editor
2. Update these sections:
   - Line 11: Change `<title>` to your name
   - Line 34: Update `--primary` color (hex code)
   - Lines 200-250: Update header text and social links
   - Lines 350+: Update project descriptions
   - Footer: Update links and copyright year

### Add Your Own Projects
Find the **Projects Grid** section (~line 350) and duplicate a project card:

```html
<div class="project-card">
    <div class="project-header">
        <h3>Your Project Name</h3>
        <p>Short description</p>
    </div>
    <div class="project-body">
        <p>Full description here.</p>
        <div class="metrics">
            <span class="metric">Metric 1</span>
            <span class="metric">Metric 2</span>
        </div>
        <div class="tech-stack">
            <span class="tech-badge">Tool 1</span>
            <span class="tech-badge">Tool 2</span>
        </div>
    </div>
</div>
```

### Change Colors
Update the CSS variables at the top of `index.html` (lines 17-28):
```css
:root {
    --primary: #3B82F6;        /* Blue – change this */
    --secondary: #8B5CF6;      /* Purple – change this */
    --accent: #EC4899;         /* Pink – change this */
}
```

Use any hex color code. Examples:
- Professional blue: `#0066CC`
- Modern teal: `#06B6D4`
- Tech orange: `#FF6B35`
- AI purple: `#7C3AED`

---

## 💡 How to Use Workflow Files

All workflow files (`.json`) are exported from n8n and can be imported directly:

### Import to n8n
1. Go to [n8n.cloud](https://n8n.cloud) or self-hosted instance
2. Click **+** (New Workflow)
3. Click **File** → **Open**
4. Select a `.json` file from the `workflows/` folder
5. Click "Import"
6. Update credentials (API keys, auth tokens) for your tools
7. Test and deploy

### Example: Lead Qualification Agent
After import, you'll need to update:
- `Retell AI` node: Add your API key
- `Airtable` node: Link to your base
- `Cal.com` node: Add your calendar
- Phone numbers: Update `FromNumber` variable

---

## 📚 Implementation Guides

### Setting Up Retell AI Voice Agent
See `docs/retell-ai-guide.md` for step-by-step instructions on:
- Creating agent voices
- Writing conversation scripts
- Handling objections
- Testing before production

### n8n Workflow Design Patterns
See `docs/n8n-setup.md` for best practices on:
- Webhook triggers
- Error handling
- Conditional logic
- Database operations

---

## 🔗 Connect With Me

- **Email:** shahrozeafzal434@gmail.com
- **LinkedIn:** [linkedin.com/in/shahroze-afzal](https://linkedin.com/in/shahroze-afzal)
- **GitHub:** [github.com/shahrozeafzal434](https://github.com/shahrozeafzal434)
- **Twitter:** [@shahroze](https://x.com/shahroze)

---

## 💼 Hiring

I'm currently open to opportunities in:
- **Full-time automation engineer roles**
- **n8n specialist positions**
- **AI voice agent development**
- **Workflow automation consultant**

If you have a workflow that needs scaling, a team drowning in manual tasks, or an n8n project that needs expert help—let's talk.

---

## 📄 License

This portfolio is open source. Feel free to fork, modify, and use as a template for your own.

---

## 🙏 Credits

Built with:
- **HTML5 & CSS3** – Clean, responsive design
- **No JavaScript framework** – Pure vanilla JS (fast & lightweight)
- **System fonts** – Native typography for optimal performance
- **Dark mode support** – Automatic light/dark mode detection

---

## 📝 Changelog

**v1.0 (2026-05-12)**
- Initial portfolio launch
- 6 featured projects
- 3 detailed case studies
- Full deployment guides
- Dark mode support

---

**Last updated:** May 12, 2026 | **Status:** Active & Hiring ✅

