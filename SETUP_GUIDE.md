# Las Primas Cleaning - Quick Setup Guide

## 🚀 5-Minute Setup

### Step 1: Get Web3Forms Access Key
1. Go to https://web3forms.com
2. Enter the business email (e.g., info@lasprimascleaning.com or your mom's email)
3. Check email for access key
4. Update line 747 in index.html: Replace `YOUR_ACCESS_KEY_HERE` with the key

### Step 2: Update Contact Information
Edit these in index.html:
- Line 221: Phone number `(773) 555-0123`
- Line 1011: Email `info@lasprimascleaning.com`
- Update service areas if not Chicago-based

### Step 3: Create GitHub Repository
```bash
# In terminal, navigate to the lasprimascleaning folder
cd /Users/davidortiz/Obsidian-Main-Branch/Main-Branches/lasprimascleaning

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: Las Primas Cleaning website"

# Add your GitHub repository (replace USERNAME)
git remote add origin https://github.com/USERNAME/lasprimascleaning.git

# Push to GitHub
git push -u origin main
```

### Step 4: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click Settings → Pages
3. Source: Deploy from a branch
4. Branch: main, folder: / (root)
5. Click Save

### Step 5: Configure Domain (at Namecheap)
Add these DNS records in Namecheap:

| Type | Host | Value |
|------|------|-------|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | USERNAME.github.io |

### Step 6: Wait for DNS
- GitHub will show "DNS check in progress"
- Usually takes 10-30 minutes
- Once ready, site will be live at https://lasprimascleaning.com

## 📱 Mobile Test
The site is fully responsive. Test on phone to ensure it looks good.

## 🎨 Future Customizations
- Add real photos of the cleaning team
- Update testimonials with real reviews
- Add Spanish language toggle
- Connect social media accounts
- Add online booking system (later)

## ⚡ Quick Changes
To make quick text changes:
1. Edit index.html
2. Commit and push to GitHub
3. Changes appear in 1-2 minutes

```bash
git add index.html
git commit -m "Update phone number"
git push
```