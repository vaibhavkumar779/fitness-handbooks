# 🏋️ Multi-User Interactive Fitness Command Portal (2026 - 2027)

A fully responsive, client-side fitness tracking ecosystem designed to run 100% free on GitHub Pages. This portal delivers highly customized blueprints configured with advanced biomechanical safety filters, condition-focused workout matrices, and a localized caching system built specifically for smooth, app-like performance on mobile web browsers.

---

## 🔒 Security & Access Control Architecture

Because this ecosystem runs entirely as a static frontend on GitHub Pages with no dedicated backend server, data safety and validation utilize **Client-Side Cryptographic Gating**:

1. **SHA-256 Hashing Integration:** User passcodes are never stored in plain text inside the source code. The core gateway running inside `index.html` leverages the browser's native Web Crypto API (`crypto.subtle.digest`) to hash user input string vectors on the fly, matching them against immutable encrypted lookup keys.
2. **Session Authorization Clearance:** Successful password verification injects an active single-session token (`authorized_clearance_granted`) directly into the browser's temporary context memory (`sessionStorage`).
3. **Direct URL Bypassing Guard Hooks:** If an unauthorized user attempts to bypass the login portal by typing a subpage address directly (e.g., `vaibhav.html`), a script hook checking `sessionStorage` instantly denies access, issues an alert popup, and redirects the browser back to `index.html`.
4. **Privacy-First Telemetry Logging:** All plain text evaluation statements have been scrubbed from production console operations to secure input metrics. Operational logging prints anonymous status events, ensuring zero tracking profile line leaks during active field entry loops.

---

## 📂 Core Repository Architecture

For the portal to function seamlessly, keep all project assets located directly at the root level of your repository using this exact structural layout:
```bash
├── index.html            # Secure Portal Gateway & Cryptographic Validator
├── style.css             # Fluid Responsive Stylesheet & Dynamic Palette Tokens
├── vaibhav.html          # Profile: Vaibhav (Lean Bulk Focus / Pre-Workout Dinner Engine)
├── akash.html            # Profile: Akash (Deficit Plan / Tempo Home Calisthenics)
├── shalini.html          # Profile: Shalini (Adaptive Dual-Track / Shared Child Nutrition)
├── vaibhav_data.csv      # Local Data Sync Template: Vaibhav
├── akash_data.csv        # Local Data Sync Template: Akash
└── shalini_data.csv      # Local Data Sync Template: Shalini
```
---

## 🚀 Instant Deployment Guide (Zero-Cost Hosting)

1. Create a **Public** repository on your GitHub account named exactly `fitness-handbooks`.
2. Upload your updated project files (`index.html`, `style.css`, dashboard files, and template `.csv` files) directly into your repository's root folder.
3. Click the **Settings** tab (gear icon) on the top horizontal menu bar of your repository.
4. Scroll down the left sidebar menu to the "Code and automation" section and click on **Pages**.
5. Under the "Build and deployment -> Branch" configuration, click the dropdown that says **None**, change it to **main** (or *master*), and click **Save**.
6. Wait 60 seconds. Refresh the page, and your production-live portal URL will be generated at the top of the Pages screen:
   `https://<YOUR-GITHUB-USERNAME>.github.io/fitness-handbooks/`

📲 **Smartphone Optimization Tip:** Open your live web link inside your smartphone's browser (Safari or Chrome), tap the browser option settings menu, and select **"Add to Home Screen"**. This creates an app icon on your phone for immediate full-screen tracking access without address bar crowding.

---

## 📱 Mobile-First UI/UX & Native PDF Engines

*   **Responsive Vector Spacing:** Layout configurations utilize CSS `clamp()` and viewport calculation tracking rules to adjust typography and card padding dynamically on smaller displays. Long data tracking matrices auto-wrap smoothly to prevent boundary clipping.
*   **Anti-Overflow Table Viewports:** Data entry grids are packaged inside specialized touch-scroll containers (`-webkit-overflow-scrolling: touch`), ensuring deep historical tables slide seamlessly under standard swipe mechanics on narrow smartphone viewports.
*   **Native Browser Print Engine:** Every profile features custom `@media print` definitions mapped to standard A4 printing bounds. Pressing **"Export PDF / Print Report"** instantly strips navigation links, interactive tabs, buttons, and dark background fill patterns, rendering clean, high-contrast black-and-white print documents optimized for permanent paper archiving or PDF generation.

---

## 🛠️ Step-by-Step Developer Guide: Adding New Profiles

This portal uses an adaptive, modular infrastructure. You can add a new person to the network at any time by executing these 4 clear steps:

### Step 1: Initialize the Profile Database
Create a new blank CSV sheet file in the root directory named after the user profile (e.g., `rohit_data.csv`). Populate the first line with these structural logging headers:
`Date,Weight_kg,Daily_Steps,Sleep_Hours,Workout_Location,Condition_Level`

### Step 2: Define Theme Tokens in style.css
Open `style.css`, scroll to the bottom, and assign a unique color style class theme hook for the new individual.
```css
body.rohit-theme {
    --primary: #a855f7;
    --primary-hover: #9333ea;
    --header-gradient: linear-gradient(135deg, #6b21a8, #1e293b);
    --table-th-bg: #6b21a8;
    --table-th-text: #f3e8ff;
}
.profile-card.rohit:hover { border-color: #a855f7; }
.badge-rohit { background: #581c87; color: #f3e8ff; }
.btn-rohit { background: #a855f7 !important; }
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
