# Nails by Hoor — Public Website 🌸

A beautiful, soft & dreamy website for showcasing your custom press-on nail business and accepting orders.

## Features

- 🏠 **Homepage** with hero, intro, featured work, process, and CTAs
- 🖼️ **Gallery** with category filters (Bridal, Glam, Minimal, French, Themed, Eid)
- 📋 **How to Order** — clear 6-step process
- 📏 **Sizing Guide** — saves you hours of DM back-and-forth
- 💰 **Pricing** — 3 transparent tiers + add-ons
- 💖 **About** page with your story
- ❓ **FAQs** with smooth accordion
- ✉️ **Contact form** that opens WhatsApp with order details pre-filled
- 🌸 Soft pink dreamy aesthetic
- ✨ Smooth animations, floating petals, scroll reveals
- 📱 Fully mobile responsive

## How to View Locally

Just double-click `index.html` and it opens in your browser! No server needed for the public site.

OR open the folder in VS Code and use the **Live Server** extension for a smoother experience with auto-refresh.

---

## Files in This Project

```
nails-by-hoor-website/
├── index.html          # Homepage
├── gallery.html        # Portfolio gallery with filters
├── how-to-order.html   # Ordering process explained
├── sizing.html         # Nail sizing guide
├── pricing.html        # Pricing tiers
├── about.html          # Your story
├── faq.html            # Common questions
├── contact.html        # Contact + order form
├── css/
│   └── style.css       # All styling (pink dreamy theme)
├── js/
│   └── main.js         # Interactivity
└── images/             # Put your nail photos here
```

---

## ⚠️ IMPORTANT: Before You Launch

You need to customize a few things to make it truly yours:

### 1. Add Your WhatsApp Number

Open `js/main.js` and find this line (around line 70):
```javascript
const whatsappNumber = '923XXXXXXXXX';
```
Replace `923XXXXXXXXX` with your actual WhatsApp number in international format:
- If your number is `0300-1234567`
- Replace with: `923001234567` (remove the 0, add 92 for Pakistan)

### 2. Update Contact Info

Open `contact.html` and find the "Reach out anytime" section. Replace:
- `+92 XXX XXXXXXX` → your real WhatsApp number
- `nailsbyhoor@gmail.com` → your real email if different

### 3. Add Your Nail Photos

Currently the site uses pretty pink placeholder boxes. To add real photos:

**For each photo placeholder:**

1. Save your photo in the `images/` folder (e.g., `images/bridal-pearl-lace.jpg`)
2. In the HTML file, find the placeholder like:
   ```html
   <div class="featured-img placeholder-img">
     <span class="placeholder-text">Add your hero nail photo</span>
   </div>
   ```
3. Replace it with:
   ```html
   <div class="featured-img" style="background-image: url('images/bridal-pearl-lace.jpg')"></div>
   ```

**Tip:** For Instagram photos, save them, crop them to be roughly square (1:1) or portrait (4:5), and resize to about 800x800px for fast loading.

### 4. Update Pricing (if needed)

Open `pricing.html` and adjust the prices to match your actual rates.

### 5. Update About Page

Open `about.html` and personalize the "Hi, I'm Hoor" story with your real journey, why you started, what makes your work special.

### 6. Replace Placeholder Names

The featured nail set names like "Pearl & Lace", "Crystal Drama", etc. are placeholders. Replace with names that match your actual portfolio!

---

## 🚀 Deploying Online (Free)

### Option 1: Vercel (Recommended)

1. Go to https://vercel.com and sign up (free)
2. Click **"Add New Project"**
3. Import your project (you can upload the folder or connect GitHub)
4. Click **Deploy** — takes 30 seconds!
5. Get a free URL like `nailsbyhoor.vercel.app` ✨

### Option 2: Netlify

1. Go to https://netlify.com and sign up
2. Drag and drop your `nails-by-hoor-website` folder onto the dashboard
3. Site goes live instantly with a URL like `nailsbyhoor.netlify.app`

### Option 3: Github Pages

1. Push your code to GitHub
2. Settings → Pages → Deploy from branch `main`
3. Get URL `yourusername.github.io/nails-by-hoor-website`

---

## 📱 Connecting a Custom Domain (Later)

When you're ready to upgrade from `nailsbyhoor.vercel.app` to `nailsbyhoor.com`:

1. Buy domain from Namecheap/GoDaddy (~PKR 3,500/year)
2. In Vercel/Netlify dashboard → Domain Settings → Add Custom Domain
3. Update DNS records (they show you exactly what to do)
4. Wait 24 hours for it to propagate
5. Done! Your site is now at `nailsbyhoor.com` 🎉

---

## 🎨 Customizing Colors

Want to tweak the pink shade? Open `css/style.css` and find the `:root` section at the top. Change these:

```css
--rose: #D4537E;       /* Main pink */
--rose-deep: #B23A65;  /* Darker pink */
--petal: #FFE4ED;      /* Lightest pink */
--blush: #F5C4D1;      /* Soft blush */
--burgundy: #5A1730;   /* Deep dark text */
```

---

## ✏️ Quick Edits

- **Change tagline** → in `index.html` look for "Where every nail tells a story"
- **Change quote** → in `index.html` find `class="quote-text"`
- **Add/remove gallery categories** → in `gallery.html`, add new `<button class="filter-btn">` and items with matching `data-category`
- **Add more FAQs** → in `faq.html`, copy any existing `<div class="faq-item">` block

---

## Made with 💖

This site was built especially for Hoor's press-on nail business. May it bring lots of beautiful orders and happy customers! 🌸

If you need help adding features, deploying, or customizing — just ask!
