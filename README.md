# 🏋️ Multi-User Interactive Fitness Command Portal (2026 - 2027)

A fully responsive, client-side fitness tracking ecosystem designed to run 100% free on GitHub Pages. This portal delivers highly customized blueprints configured with advanced biomechanical safety filters, condition-focused workout matrices, and a custom browser-caching CSV engine built specifically for fast, app-like performance on mobile web interfaces.

---

## 📂 Core Repository Architecture

For the portal to function seamlessly, keep all project assets located directly at the root level of your repository using this exact layout:
```bash
├── index.html            # Portal Gateway Selector Page
├── style.css             # Central Layout Stylesheet & Dynamic Color Tokens
├── vaibhav.html          # Profile Dashboard: Vaibhav (Lean Muscle bulking / Pre-Gym Dinner)
├── akash.html            # Profile Dashboard: Akash (Fat Loss / Ultra Budget Eggitarian)
├── shalini.html          # Profile Dashboard: Shalini (Fat Loss / Post C-Section Core Rehab)
├── vaibhav_data.csv      # Metrics Database Log: Vaibhav
├── akash_data.csv        # Metrics Database Log: Akash
└── shalini_data.csv      # Metrics Database Log: Shalini
```
---

## 🚀 Instant Deployment Guide (Zero-Cost Hosting)

1. Create a Public repository on your GitHub account named exactly "fitness-handbooks".
2. Upload the dashboard code files (.html, .css, .csv, .md) directly into your repository root folder.
3. Click the Settings tab (gear icon) on the top horizontal menu bar of your repository.
4. Scroll down the left sidebar menu to the "Code and automation" section and click on Pages.
5. Under the "Build and deployment -> Branch" configuration, click the dropdown that says None, change it to main (or master), and click Save.
6. Wait 60 seconds. Refresh the page, and your production-live portal URL will be generated at the top of the Pages screen:
   https://<YOUR-GITHUB-USERNAME>.github.io/fitness-handbooks/

📲 Smart Phone Optimization Tip: Open your live web link inside your smartphone's browser (Safari or Chrome), tap the browser option settings menu, and select "Add to Home Screen". This creates an app shortcut icon on your phone for immediate full-screen tracking access.

---

## 🛠️ Step-by-Step Developer Guide: Adding New Profiles

This portal uses an adaptive, modular infrastructure. You can add a new person to the network at any time by executing these 4 clear steps:

### Step 1: Initialize the Profile Database
Create a new blank CSV sheet file in the root directory named after the user profile (e.g., rohit_data.csv). Populate the first line with these structural logging headers:
Date,Weight_kg,Daily_Steps,Sleep_Hours,Constraint_Pain_Level

### Step 2: Define Theme Tokens in style.css
Open style.css, scroll to the bottom, and assign a unique color style class theme hook for the new individual.
Example layout configuration for a purple/violet variant:
```css
body.rohit-theme {
    --primary: #a855f7;
    --primary-hover: #9333ea;
    --header-gradient: linear-gradient(135deg, #6b21a8, #1e293b);
    --table-th-bg: #6b21a8;
    --table-th-text: #f3e8ff;
}
.profile-card.rohit { border-top: 5px solid #a855f7; }
.badge-rohit { background: #581c87; color: #f3e8ff; }
.btn-rohit { background: #a855f7; } .btn-rohit:hover { background: #9333ea; }
```
### Step 3: Append Gateway Card in index.html
Open index.html, locate the <div class="portal-grid"> block container, and paste the selector card interface before the final closing div tag:
```html
<div class="profile-card rohit">
    <h2>Rohit</h2>
    <span class="badge badge-rohit">Body Recomp Framework</span>
    <div class="card-specs">
        <p><strong>Target:</strong> 85kg → 78kg</p>
        <p><strong>Energy Budget:</strong> 1900 kcal</p>
    </div>
    <a href="rohit.html" class="btn btn-rohit">Launch Engine →</a>
</div>
```
### Step 4: Create the Dashboard File (newuser.html)
1. Duplicate one of the existing dashboard files (e.g., akash.html) and rename it exactly to match your gateway page target (e.g., rohit.html).
2. Update the dynamic class hook signature located on the opening <body> tag: Change it to read <body class="rohit-theme">.
3. Scroll down into the <script> layer and adjust the initialization variables to reflect the new baseline weight metrics:
   const BASELINE_MASS = 85.0; // Change to match initial baseline mass scale
   const cache = localStorage.getItem('rohit_fitness_logs'); // Update local keys
4. Customize the HTML view panels with their distinct calculated nutritional splits, pre/post workout arrangements, and targeted physical activity charts. Commit the file changes to your repository to push the new profile live.

---

## 🔄 The 30-Second Mobile Data Sync Loop

Because static web hosts like GitHub Pages do not run server-side databases and cannot edit files directly, your data entries are safely captured inside your browser's localized localStorage cache. Follow this rapid loop to lock in your long-term progress forever:

[Log Daily Metrics] ➔ [Tap 'Copy Raw CSV Text'] ➔ [Open GitHub Web Editor] ➔ [Paste & Commit]

1. Access your tracking manual from your smartphone home screen link.
2. Go to Tab 4: Analytics & CSV Storage Engine, fill out your variables, and tap Commit Data Entry (your dashboard tables will recalculate immediately).
3. Tap Copy Raw CSV Text to instantly copy your clean history data string to your device clipboard.
4. Open your public GitHub repo inside the mobile browser, select your personal data sheet (e.g., vaibhav_data.csv), click the Pencil icon to edit, clear the old lines, paste your clipboard contents, and hit Commit changes. Your metrics are now permanently backed up to the cloud!
