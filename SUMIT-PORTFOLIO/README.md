# Sumit Chandan Kapile – Portfolio Website

Built with HTML5, CSS3 and vanilla JavaScript (no frameworks). Made for **Assignment No. 3 – Web Analysis Using Google Analytics (GA4)**.

## Folder structure
```
SUMIT-PORTFOLIO/
├── index.html
├── style.css
├── script.js
├── README.md
└── assets/
    ├── images/   (profile.jpg, vehicle-rental.png, kapile-jewellers.png, certificates.jpg)
    └── icons/
```
Missing images show a placeholder automatically. Add your own files with the exact names above.

## Run in VS Code
1. Install VS Code and the **Live Server** extension (Ritwick Dey).
2. File > Open Folder > select `SUMIT-PORTFOLIO`.
3. Right-click `index.html` > **Open with Live Server**.

## Things to edit
- Email: search `YOUR_EMAIL@example.com` in `index.html` (2 places).
- Project "View Project" links: replace `href="#"` in the Projects section.
- Certificate details: add later; do not invent dates or IDs.

## Google Analytics 4 setup
1. Go to analytics.google.com, sign in, click **Start measuring** and create an account.
2. Create a **GA4 property** (name, time zone India, currency INR).
3. Choose **Web** platform and add a **Web data stream** with your Vercel URL (add this after deploying; you can edit it later).
4. Copy the **Measurement ID** (looks like `G-ABC123XYZ9`).
5. In `index.html`, replace both `G-XXXXXXXXXX` values inside the GA4 section in `<head>`. Save.

## Deploy on Vercel
1. Upload the folder to a GitHub repository (GitHub Desktop or `git push`).
2. Sign in at vercel.com with GitHub > **Add New > Project** > import the repo.
3. Framework Preset: **Other**. Leave build settings empty. Click **Deploy**.
4. Copy your `https://yourname.vercel.app` URL and put it in the GA4 data stream.

## Verify tracking
1. Open your live Vercel site (not Live Server) in a browser tab. Ad blockers can block GA, so disable them.
2. In GA4 go to **Reports > Realtime**. You should see yourself as 1 active user within a minute.
3. Visit the site on several days from different devices/friends to collect real data. Data in standard reports can take 24–48 hours.

## Reports to check
- **Active users** and **Views**: Reports > Life cycle/Engagement > Overview.
- **Traffic acquisition**: Reports > Acquisition > Traffic acquisition.
- **Engagement**: Reports > Engagement > Pages and screens (engagement time, engagement rate).

## Three screenshots for the assignment
1. **Realtime report** showing active users (include the date/time and the URL).
2. **Traffic acquisition** report (set the date range, show the table).
3. **Engagement overview** (views, active users, engagement time).

Windows: `Win + Shift + S`. Save as PNG and label them clearly. Use only your real data; never edit numbers.

## Note
The contact form only validates input. It does not send email until you connect a service such as Formspree or EmailJS.