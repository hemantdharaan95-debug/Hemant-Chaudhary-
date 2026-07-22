# Hemant Chaudhary — Personal Portfolio

A premium, single-file personal portfolio website. **All content is editable in one place** — no build tools, no npm, no terminal required.

---

## 🚀 How to Publish on GitHub Pages (Free Hosting)

### Step 1 — Create a GitHub account
Go to [github.com](https://github.com) and sign up (free).

### Step 2 — Create a new repository
1. Click the **+** icon → **New repository**
2. Name it exactly: `hemantchaudhary` (or `your-github-username.github.io` for a cleaner URL)
3. Set it to **Public**
4. Click **Create repository**

### Step 3 — Upload your files
1. On your new repository page, click **Add file → Upload files**
2. Drag and drop `index.html` (and `README.md` if you want)
3. Click **Commit changes**

### Step 4 — Enable GitHub Pages
1. Go to your repository → **Settings** tab
2. Scroll down to **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Branch: `main` | Folder: `/ (root)`
5. Click **Save**

### Step 5 — Your site is live!
After ~2 minutes, your site will be at:
```
https://YOUR-USERNAME.github.io/REPO-NAME/
```

---

## ✏️ How to Edit Content

**Everything lives in the `CONFIG` object** near the top of `index.html`.

### On GitHub (no code editor needed):
1. Open `index.html` in your repository
2. Click the **pencil icon ✏️** (Edit this file)
3. Find `const CONFIG = {` near the top
4. Edit the values between the quotes
5. Scroll down → **Commit changes** → **Commit directly to main branch**
6. Your site updates automatically in ~30 seconds

### What you can change:

| Field | What it controls |
|-------|-----------------|
| `name` | Your name everywhere on the site |
| `tagline` | Subtitle under your name |
| `location` | Location shown in hero |
| `email` | Email in contact section |
| `phone` | Phone number |
| `whatsapp` | WhatsApp number (without +) |
| `linkedin` | LinkedIn profile URL |
| `resumeLink` | Direct link to your resume PDF |
| `stats[]` | The counter numbers in the hero |
| `about` | Your about me text (use blank lines for paragraphs) |
| `career[]` | Each job role, bullets, skills |
| `education[]` | Degrees and institutions |
| `skills[]` | Skill names and percentages (0–100) |
| `certifications[]` | Certificate name, issuer, year, link |
| `projects[]` | Project cards with problem/solution/outcome |
| `sessions[]` | Coaching session types and prices |
| `testimonials[]` | Reviews and testimonials |
| `blog[]` | Blog post titles, summaries, links |
| `faqs[]` | FAQ questions and answers |

---

## 📧 Making the Contact Form Work Properly

The form currently opens your email client. To make it send emails directly:

### Option A — Formspree (free, 50 submissions/month)
1. Go to [formspree.io](https://formspree.io) → Create account
2. Create a new form → copy your form ID (looks like `xrgdwkpz`)
3. In `index.html`, find the `submitForm()` function
4. Replace the `window.open` line with:
```javascript
fetch('https://formspree.io/f/YOUR-FORM-ID', {
  method: 'POST',
  headers: {'Content-Type': 'application/json'},
  body: JSON.stringify({name, email, subject, message: msg})
});
```

---

## 🎨 Customization Tips

### Change accent color
Find `--accent:#6366f1;` and replace `#6366f1` with any color:
- Blue: `#3b82f6`
- Teal: `#14b8a6`
- Purple: `#8b5cf6`
- Gold: `#f59e0b`

### Add a profile photo
Replace the avatar initials with an `<img>` tag by editing the `.about-avatar` section.

### Add more blog posts
Copy one item in the `blog: []` array and update the title, summary, etc.

---

## 📱 What's Included

- ✅ Dark / Light mode (saves preference)
- ✅ Fully mobile responsive
- ✅ Animated hero with floating orbs
- ✅ Counter animations for stats
- ✅ Scroll reveal animations
- ✅ Animated skill bars
- ✅ Career timeline with promotion badges
- ✅ Project cards
- ✅ Session booking cards
- ✅ Testimonials
- ✅ Blog section
- ✅ FAQ accordion
- ✅ Contact form
- ✅ Back to top button
- ✅ SEO meta tags
- ✅ Zero dependencies (no npm, no build step)
- ✅ Single HTML file — works offline

---

Built for **Hemant Chaudhary** · Professional Lighting · B2B Sales · Karnataka
