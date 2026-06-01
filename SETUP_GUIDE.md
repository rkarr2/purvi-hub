# Purvi's Learning Hub — Complete Setup Guide

This guide walks you through three short steps to launch the system. **Total time: about 20 minutes.** No coding required.

---

## What you're building

- **A web app** hosted at `https://rkarr2.github.io/purvi-hub/` that Purvi can open from any device, anywhere
- **A Google Form** for her weekly reflections that posts answers to a Google Sheet in your Drive
- **A Google Sheet** in your Drive where you review her reflections — from your own phone, any device, anywhere

---

## STEP 1 — Create the Google Form (5 minutes)

This is the journal Purvi will fill in each week. Her answers will land in a Sheet in your Drive that you can review remotely.

### 1.1 — Create the form

1. Open [forms.google.com](https://forms.google.com) on your computer or phone (signed into the same Google account as your Drive)
2. Click the big **`+ Blank form`** button
3. Title it: **Purvi's Weekly Reflection**
4. Add this description in the field below the title:
   > Your honest weekly reflection. Save your answers as you go — submit at the end of the week.

### 1.2 — Add the questions

Add each question below by clicking the **`+ Add question`** button on the right toolbar.

> Tip: copy the question text directly from this guide. For each one, pick the answer type listed and toggle "Required" if shown.

**Question 1** — Short answer, Required
> Which week are you reflecting on?
- Change type to **Multiple choice**
- Add options: Week 1, Week 2, Week 3, Week 4, Week 5, Week 6, Week 7, Week 8

**Question 2** — Paragraph
> The most surprising thing I learned this week was...

**Question 3** — Paragraph
> This week connected to my goal of becoming a psychiatrist because...

**Question 4** — Paragraph
> The hardest thing this week was... and here's what I'll do about it next week:

**Question 5** — Paragraph
> If I could ask one question to a professional in this field, it would be...

**Question 6** — Linear scale (1 to 5)
> Concept Clarity — I can explain the main ideas in my own words.

**Question 7** — Linear scale (1 to 5)
> Curiosity Sparked — This week made me want to learn more.

**Question 8** — Linear scale (1 to 5)
> Connection Making — I can connect this to psychiatry or other subjects.

**Question 9** — Linear scale (1 to 5)
> Application — I could explain a key concept to a friend.

**Question 10** — Linear scale (1 to 5)
> Effort & Consistency — I showed up fully every day.

**Question 11** — Linear scale (1 to 5)
> Growth Edge — I named what challenged me and have a plan.

**Question 12** — Linear scale (1 to 10)
> Curiosity Meter — how interesting was this week overall? (1 = not really, 10 = obsessed)

**Question 13** — Paragraph
> Anything else you want to share with your parent this week?

### 1.3 — Connect responses to a Google Sheet

1. At the top of the form, click the **Responses** tab
2. Click the green **Sheets icon** (Link to Sheets)
3. Choose **Create a new spreadsheet**, name it `Purvi's Reflection Journal`, click **Create**
4. A new tab will open showing the Sheet. **This is where you'll read all of Purvi's reflections** — bookmark it on your phone.

### 1.4 — Get the form URL to put in the app

1. Go back to the form tab
2. Click **Send** at the top right
3. Click the **link icon (🔗)** in the popup
4. Copy the URL shown (it looks like `https://docs.google.com/forms/d/e/XXXXXXXXX/viewform`)
5. **Paste it somewhere temporary** — you'll need it in Step 2

---

## STEP 2 — Put the form URL into the app (1 minute)

1. Open the file `index.html` in any text editor (Notepad, TextEdit, or even right in GitHub)
2. Find this line near the top of the script section (around line 240):
   ```
   journalFormUrl: "REPLACE_WITH_YOUR_FORM_URL",
   ```
3. Replace `REPLACE_WITH_YOUR_FORM_URL` with the form URL you copied (keep the quotes)
4. Save the file

That's it — the app now knows where to send Purvi's reflections.

---

## STEP 3 — Host the app on GitHub Pages (10 minutes)

This puts the site online for free at a permanent URL.

### 3.1 — Create the repository

1. Go to [github.com](https://github.com) and sign in as `rkarr2`
2. Click the **`+`** in the top right → **New repository**
3. Repository name: `purvi-hub`
4. Description: `Purvi's Summer Learning Hub 2026`
5. Set to **Public** (required for free GitHub Pages)
6. Check **Add a README file**
7. Click **Create repository**

### 3.2 — Upload the files

1. On the new repo page, click **Add file** → **Upload files**
2. Drag both files into the upload area:
   - `index.html` (the edited one with your form URL)
   - `SETUP_GUIDE.md` (this file)
3. Scroll down and click **Commit changes**

### 3.3 — Turn on GitHub Pages

1. Click the **Settings** tab at the top of the repo
2. In the left sidebar, click **Pages**
3. Under **Source**, choose **Deploy from a branch**
4. Under **Branch**, select **main** and the folder **`/ (root)`**
5. Click **Save**
6. Wait 1–2 minutes. The page will refresh and show: **"Your site is live at https://rkarr2.github.io/purvi-hub/"**

### 3.4 — Test it

1. Open `https://rkarr2.github.io/purvi-hub/` on your phone
2. You should see the home screen with "Hello, Purvi"
3. If today is before June 8, all weeks will be locked with a "Starts June 8" message — that's correct
4. After June 8, Week 1 unlocks. Each Monday thereafter, the next week unlocks automatically

### 3.5 — Add to phone home screen (one-tap access)

**On Purvi's phone:**
1. Open `https://rkarr2.github.io/purvi-hub/` in her browser (Chrome on Android, Safari on iPhone)
2. **Android:** tap menu (⋮) → **Add to Home screen**
3. **iPhone:** tap share (□↑) → **Add to Home Screen**
4. Now she has an app icon. Same on her tablet, laptop, anywhere she logs in.

---

## How weekly review works for you

Every time Purvi submits her weekly journal:
1. Her answers appear instantly in `Purvi's Reflection Journal` (the Google Sheet in your Drive)
2. You open the Sheet from your phone any time — at work, traveling, anywhere
3. Each row is one week's submission, with a timestamp, so you can see her growth over the summer

**Optional:** turn on Google Forms email notifications. In the form, go to Responses → vertical dots (⋮) → Get email notifications for new responses. You'll get an email every time Purvi submits.

---

## How the date-based gating works

- **Week 1:** unlocks on Monday, June 8, 2026
- **Week 2:** unlocks Monday, June 15
- **Week 3:** unlocks Monday, June 22
- **Week 4:** unlocks Monday, June 29
- **Week 5:** unlocks Monday, July 6
- **Week 6:** unlocks Monday, July 13
- **Week 7:** unlocks Monday, July 20
- **Week 8:** unlocks Monday, July 27 (capstone week)

These unlock identically on every device — no login, no sync, no setup. The same calendar = the same unlock.

---

## Updating the curriculum later

If you want to add resources, change activities, or fix anything:
1. Go to your `purvi-hub` repo on GitHub
2. Click on `index.html`
3. Click the **pencil icon** (Edit this file) in the top right
4. Make your changes and click **Commit changes**
5. The site updates automatically in about 1 minute

---

## Troubleshooting

**The form shows as a warning box instead of loading:**
You haven't completed Step 2. Make sure you replaced `REPLACE_WITH_YOUR_FORM_URL` with the actual form URL in `index.html`, saved the file, and uploaded it to GitHub.

**The site shows "404 — File not found":**
GitHub Pages needs a minute or two after first setup. Wait, then refresh. If still broken, go to Settings → Pages and check that it says "Your site is live."

**All weeks are locked:**
Today is before June 8. This is correct. Week 1 unlocks the morning of June 8.

**Purvi's phone shows old content:**
Pull down to refresh, or close and reopen the app icon.

**I want to change the start date:**
Edit `index.html`, find `startDate: "2026-06-08"`, change the date in YYYY-MM-DD format, save, upload to GitHub.

---

## What lives where

| Thing | Where |
|---|---|
| The learning app | `https://rkarr2.github.io/purvi-hub/` |
| The source code | `https://github.com/rkarr2/purvi-hub` |
| The journal form | Google Forms in your Drive |
| Purvi's reflections | `Purvi's Reflection Journal` Sheet in your Drive |
| This guide | Your Drive + GitHub repo |

You're done. The system runs itself for the rest of the summer.
