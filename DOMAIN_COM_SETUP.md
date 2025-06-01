# Domain.com DNS Configuration for Las Primas Cleaning

## 🌐 Domain.com DNS Setup Instructions

### Step 1: Log into Domain.com
1. Go to https://www.domain.com
2. Click "Sign In" in the top right
3. Enter your username and password
4. Click on "My Domains" or "Manage"

### Step 2: Access DNS Management
1. Find `lasprimascleaning.com` in your domain list
2. Click on the domain name
3. Look for "DNS & Nameservers" or "Manage DNS"
4. Click on "DNS Records" or "Advanced DNS"

### Step 3: Delete Existing Records
⚠️ **Important**: Delete any existing A records for @ (root) and CNAME for www

### Step 4: Add GitHub Pages DNS Records

Click "Add Record" and create these exact records:

#### A Records (for root domain)
| Type | Name | Value | TTL |
|------|------|-------|-----|
| A | @ | 185.199.108.153 | 3600 |
| A | @ | 185.199.109.153 | 3600 |
| A | @ | 185.199.110.153 | 3600 |
| A | @ | 185.199.111.153 | 3600 |

#### CNAME Record (for www)
| Type | Name | Value | TTL |
|------|------|-------|-----|
| CNAME | www | razonin4k.github.io | 3600 |

### Step 5: Save Changes
1. Click "Save" or "Update" after adding each record
2. Changes may take 5-30 minutes to propagate

### Step 6: Verify in GitHub
1. Go to: https://github.com/RazonIn4K/lasprimascleaning/settings/pages
2. Under "Custom domain", it should show:
   - ✅ DNS check successful
   - 🔒 Enforce HTTPS (check this box)

## 🔍 How to Check if DNS is Working

### Option 1: Command Line
```bash
# Check A records
nslookup lasprimascleaning.com

# Check CNAME
nslookup www.lasprimascleaning.com
```

### Option 2: Online Tool
Visit: https://www.whatsmydns.net
- Enter `lasprimascleaning.com`
- Select "A" record type
- Should show GitHub's IPs globally

## ⏱️ Timeline
- **DNS Propagation**: 5-30 minutes (can take up to 48 hours in rare cases)
- **GitHub Pages Build**: 1-2 minutes after DNS works
- **SSL Certificate**: 15-60 minutes after DNS verification

## 🚨 Troubleshooting

### If "DNS check unsuccessful" in GitHub:
1. Double-check all IP addresses are correct
2. Ensure no typos in CNAME value
3. Wait 30 more minutes
4. Try clearing browser cache

### If site shows 404:
1. Make sure GitHub Pages is enabled
2. Check that `main` branch is selected
3. Verify CNAME file exists in repository

### Domain.com Specific Tips:
- Domain.com sometimes labels records differently
- "Host" = "Name" (use @ for root)
- "Points to" = "Value" 
- "TTL" = Time to Live (3600 is fine)

## 📞 Support
- **Domain.com Support**: 1-800-403-3568
- **GitHub Pages Docs**: https://docs.github.com/pages

## ✅ Success Checklist
- [ ] All 4 A records added for @
- [ ] CNAME record added for www
- [ ] Old records deleted
- [ ] Changes saved in Domain.com
- [ ] GitHub shows "DNS check successful"
- [ ] Site loads at https://lasprimascleaning.com