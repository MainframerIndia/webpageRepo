# Mainframers India Website

A modern, professional static website for the Mainframe community in India.

## 🚀 Quick Start - Hosting on GitHub Pages (FREE)

### Step 1: Create a GitHub Account
1. Go to https://github.com
2. Click "Sign up" and create a free account
3. Verify your email address

### Step 2: Create a New Repository
1. Click the "+" icon in the top right corner
2. Select "New repository"
3. Name it: `mainframers-india` (or any name you prefer)
4. Make it **Public**
5. Click "Create repository"

### Step 3: Upload Your Website Files
You have two options:

#### Option A: Upload via Web Interface (Easiest)
1. In your new repository, click "uploading an existing file"
2. Drag and drop these files:
   - `index.html`
   - `styles.css`
   - `script.js`
3. Scroll down and click "Commit changes"

#### Option B: Using Git (If you're comfortable with command line)
```bash
git init
git add index.html styles.css script.js
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/mainframers-india.git
git push -u origin main
```

### Step 4: Enable GitHub Pages
1. In your repository, click "Settings"
2. Scroll down to "Pages" in the left sidebar
3. Under "Source", select "main" branch
4. Click "Save"
5. GitHub will show you a URL like: `https://YOUR-USERNAME.github.io/mainframers-india/`
6. Wait 2-3 minutes for your site to deploy

Your website is now live! 🎉

---

## 🌐 Connect Your Custom Domain (mainframerindia.in)

### Step 5: Configure GitHub Pages for Custom Domain
1. Still in Settings → Pages
2. Under "Custom domain", enter: `mainframerindia.in`
3. Click "Save"
4. Check the "Enforce HTTPS" box (you may need to wait a few minutes for this option to appear)

### Step 6: Update DNS Settings at Your Domain Registrar
You need to add DNS records where you registered mainframerindia.in

#### A Records (Point to GitHub's servers)
Add these **4 A records**:
```
Type: A
Name: @ (or leave blank for root domain)
Value: 185.199.108.153

Type: A  
Name: @ 
Value: 185.199.109.153

Type: A
Name: @
Value: 185.199.110.153

Type: A
Name: @
Value: 185.199.111.153
```

#### CNAME Record (for www subdomain)
```
Type: CNAME
Name: www
Value: YOUR-USERNAME.github.io
```

#### Where to add these records:
- If you registered with **GoDaddy**: Domain Settings → DNS Management
- If you registered with **Namecheap**: Dashboard → Domain List → Manage → Advanced DNS
- If you registered with **Google Domains**: DNS → Custom records
- Other registrars: Look for "DNS Settings" or "DNS Management"

### Step 7: Wait for DNS Propagation
- DNS changes can take **1-48 hours** to propagate worldwide
- Usually happens within 1-4 hours
- You can check status at: https://www.whatsmydns.net

---

## 📝 Updating Your Website Content

### To Update Content:
1. Go to your GitHub repository
2. Click on the file you want to edit (e.g., `index.html`)
3. Click the pencil icon (✏️) to edit
4. Make your changes
5. Scroll down and click "Commit changes"
6. Your website will update automatically in 1-2 minutes!

### Key Sections to Customize:

#### Update About Section
In `index.html`, find the `<section id="about">` and edit:
- Community description
- Member count in stats cards
- Cities represented

#### Add Real Events
In `index.html`, find `<section id="events">` and:
- Update event titles, dates, and descriptions
- Add registration links by replacing `href="#"` with your actual link

#### Connect Substack Blog
In `index.html`, find `<section id="blog">` and:
- Replace the placeholder blog cards with actual blog post previews
- Add link to your Substack: Replace `href="#"` with your Substack URL

#### Add Slack Join Link
In `index.html`, find `<section id="join">`:
- Replace `<a href="#" class="btn btn-primary">Join Slack</a>`
- With: `<a href="YOUR-SLACK-INVITE-LINK" class="btn btn-primary">Join Slack</a>`

---

## 🎨 Customization Options

### Change Colors
Edit `styles.css` at the top (`:root` section):
```css
:root {
    --accent-primary: #00ff9f;      /* Main green color */
    --accent-secondary: #00d4ff;    /* Blue accent */
    --bg-primary: #0a0e27;          /* Dark background */
    /* Change these values to customize */
}
```

### Add Your Logo
1. Upload logo image to GitHub repository
2. In `index.html`, find `.nav-brand` section
3. Add: `<img src="your-logo.png" alt="Logo" style="height: 30px;">`

---

## 💡 Advanced: Import Blog Posts from Substack

To automatically show your latest Substack posts, you can:

1. **Option 1: Manual** - Copy paste blog post links and descriptions
2. **Option 2: RSS Feed** - Use a free service like RSS2JSON:
   - Get your Substack RSS feed: `https://yoursubstack.substack.com/feed`
   - Use https://rss2json.com to convert to JSON
   - Add JavaScript to fetch and display posts

Would you like me to create the JavaScript code for automatic Substack integration?

---

## 📱 Mobile Friendly
The website is fully responsive and works great on mobile devices!

---

## 🆘 Troubleshooting

### Website not showing after DNS change?
- Wait longer (up to 48 hours)
- Clear your browser cache
- Try in incognito/private mode
- Check DNS propagation at https://www.whatsmydns.net

### GitHub Pages not working?
- Make sure repository is **Public**
- Check that files are in the root directory (not in a folder)
- Verify the main file is named exactly `index.html`

### Changes not appearing?
- Wait 1-2 minutes after commit
- Hard refresh: Ctrl+F5 (Windows) or Cmd+Shift+R (Mac)
- Clear browser cache

---

## 📞 Need Help?

If you get stuck:
1. Check GitHub Pages documentation: https://docs.github.com/pages
2. Ask in your Slack community - someone might have experience!
3. GitHub has great community forums

---

## 🎉 You Did It!

Congratulations on launching your community website! Here's what you've accomplished:
- ✅ Created a professional website with zero coding knowledge
- ✅ Hosted it completely FREE on GitHub Pages
- ✅ Connected your custom domain
- ✅ Have a site that's easy to update anytime

Share it with your community! 🚀

---

## 📄 License

Feel free to use and modify this website for your community!

---

**Built with ❤️ for the Mainframe Community in India**
