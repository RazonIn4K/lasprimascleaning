# Las Primas Cleaning Website

Professional house cleaning services website for Las Primas Cleaning in Chicago.

## Features

- Modern, responsive design optimized for all devices
- Interactive pricing calculator
- Instant quote form with Web3Forms integration
- Bilingual support (English/Spanish)
- SEO optimized for local search
- Fast loading with Tailwind CSS
- Professional testimonials section
- Service area coverage map

## Setup Instructions

### 1. Create GitHub Repository

1. Go to https://github.com/new
2. Name it `lasprimascleaning`
3. Make it public
4. Don't initialize with README (we already have one)

### 2. Push Code to GitHub

```bash
cd lasprimascleaning
git init
git add .
git commit -m "Initial commit: Las Primas Cleaning website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/lasprimascleaning.git
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to repository Settings
2. Navigate to Pages section
3. Source: Deploy from a branch
4. Branch: main
5. Folder: / (root)
6. Save

### 4. Configure Custom Domain

1. In GitHub Pages settings, add custom domain: `lasprimascleaning.com`
2. Create CNAME file in repository

### 5. DNS Configuration (at your domain registrar)

Add these DNS records:

```
Type: A      | Name: @   | Value: 185.199.108.153
Type: A      | Name: @   | Value: 185.199.109.153
Type: A      | Name: @   | Value: 185.199.110.153
Type: A      | Name: @   | Value: 185.199.111.153
Type: CNAME  | Name: www | Value: YOUR_USERNAME.github.io
```

### 6. Set Up Form Backend (Web3Forms)

1. Visit https://web3forms.com
2. Enter your email address
3. Get your access key
4. Replace `YOUR_ACCESS_KEY_HERE` in index.html (line 747)

## Website Details

- **Framework**: Tailwind CSS (CDN)
- **Icons**: Font Awesome
- **Fonts**: Poppins & Playfair Display
- **Form Backend**: Web3Forms
- **Hosting**: GitHub Pages
- **SSL**: Automatic via GitHub Pages

## Customization

### Colors
- Primary: Green (#22c55e)
- Primary Dark: (#16a34a)
- Accent: Yellow (#facc15)

### Contact Information
Update these in index.html:
- Phone number (currently placeholder: 773-555-0123)
- Email (currently placeholder: info@lasprimascleaning.com)
- Service areas
- Social media links

### Images
Replace the Unsplash placeholder images with actual photos:
- Team photo
- Before/after cleaning photos
- Service showcase images

## SEO Optimization

The website includes:
- Meta descriptions
- Semantic HTML
- Schema.org structured data
- Mobile-responsive design
- Fast loading times
- Local SEO optimization for Chicago

## Support

For issues or questions, please create an issue in this repository.