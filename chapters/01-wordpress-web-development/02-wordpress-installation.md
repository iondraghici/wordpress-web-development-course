# Lesson 2: WordPress Installation

**Type**: OVERVIEW | **Duration**: ~30 minutes

---

## What You'll Learn

✅ Understand system requirements for WordPress
✅ Choose and configure web hosting
✅ Install WordPress in multiple ways
✅ Complete initial WordPress setup
✅ Make your first login
✅ Understand basic security settings

---

## Introduction

Now that you understand what WordPress is, it's time to get it installed and running! This lesson will guide you through the entire installation process, from choosing hosting to making your first WordPress login.

Don't worry - modern hosting companies have made WordPress installation incredibly easy!

---

## System Requirements

Before installing WordPress, ensure your hosting meets these minimum requirements:

### Server Requirements

**Minimum (but outdated)**:
- PHP 5.6.20 or higher
- MySQL 5.0.15 or higher

**Recommended** (current WordPress standard):
- PHP 7.4 or higher (ideally PHP 8.0+)
- MySQL 5.7 or higher
- OR MariaDB 10.3 or higher

### What These Mean:

- **PHP**: The programming language WordPress is written in
- **MySQL/MariaDB**: The database that stores your content

### Check Your Hosting

Most modern hosting providers meet these requirements. When choosing hosting, always check:

1. PHP version (7.4+)
2. Database support (MySQL 5.7+ or MariaDB 10.3+)
3. At least 10GB of disk space
4. HTTPS support (SSL certificate)
5. Email support

---

## Installation Methods

There are three main ways to install WordPress:

### Method 1: One-Click Installation (Easiest) ⭐

Most hosting providers offer automated WordPress installation.

**Pros**:
- Fastest method
- No technical knowledge required
- Usually takes 5 minutes
- Hosting company handles everything

**Cons**:
- Less customization
- Limited control over installation details

**Recommended for**: Beginners

### Method 2: Manual Installation via FTP (Intermediate)

Download WordPress files and upload them via FTP.

**Pros**:
- Full control
- Learn how WordPress works
- Can customize during installation

**Cons**:
- More technical steps
- Need FTP knowledge
- Takes 15-20 minutes

**Recommended for**: Intermediate users

### Method 3: Command Line Installation (Advanced)

Using SSH and the command line.

**Pros**:
- Most control
- Fastest for experienced users
- Can automate

**Cons**:
- Requires SSH access
- Technical command line knowledge needed

**Recommended for**: Developers and experienced users

---

## Step-by-Step: One-Click Installation (Recommended)

### Step 1: Log Into Your Hosting Control Panel

Most hosting providers use cPanel, Plesk, or their own dashboard.

1. Go to your hosting provider's website
2. Log in with your account credentials
3. Look for the control panel or dashboard

### Step 2: Find the Installation Tool

Look for one of these:

- **Softaculous** (Most common)
- **WordPress Toolkit**
- **Installatron**
- **Auto-Installers**

They're usually under "Software" or "Applications" section.

### Step 3: Select WordPress

1. Click on "Softaculous" or similar tool
2. Find "WordPress" in the list
3. Click "Install"

### Step 4: Configure Installation

You'll see a form with these important fields:

**Domain Selection**
```
- Choose your domain (e.g., yourdomain.com)
- Decide between www or non-www
- Use /wp or root directory
```

**Directory**
```
- Leave empty for root install
- Use /blog for subdirectory install
```

**Admin Account**
```
Username: [Create a strong, unique username - NOT "admin"]
Password: [Create a very strong password - 16+ characters]
Email: [Your email address]
```

**Site Settings**
```
Site Title: [Your website name]
Site Description: [Brief description of your site]
```

### Step 5: Complete Installation

1. Review all settings
2. Check "I agree to the terms" (if shown)
3. Click "Install"
4. Wait 2-5 minutes for installation to complete
5. You'll get a confirmation message

### Step 6: Access Your WordPress Site

You'll receive installation details:

**Your Site**:
```
URL: https://yourdomain.com
```

**Admin Login**:
```
URL: https://yourdomain.com/wp-admin
Username: [Your chosen username]
Password: [Your chosen password]
```

---

## Your First WordPress Login

### Accessing the Admin Panel

1. Go to `https://yourdomain.com/wp-admin`
2. Enter your username and password
3. Click "Log In"

### What You'll See

The WordPress Dashboard - your command center!

```
┌─────────────────────────────────┐
│ WordPress Admin Dashboard        │
├─────────────────────────────────┤
│                                 │
│  Left Sidebar:                  │
│  - Dashboard                    │
│  - Posts                        │
│  - Pages                        │
│  - Comments                     │
│  - Media                        │
│  - Appearance (Themes)          │
│  - Plugins                      │
│  - Users                        │
│  - Settings                     │
│                                 │
└─────────────────────────────────┘
```

---

## Initial Setup Checklist

After installation, complete these important tasks:

### Security - CRITICAL! 🔒

**1. Set Admin Password**
- Make it very strong (mix of uppercase, lowercase, numbers, symbols)
- Store it in a password manager
- Never use "admin" as username

**2. Enable HTTPS**
- Go to Settings > General
- Ensure both URLs use `https://`
- Install SSL certificate (usually free with hosting)

**3. Delete Sample Content**
- Delete "Hello World" post
- Delete "Sample Page"
- Delete "Hello World" comment

**4. Create Admin User**
- If needed, create a second admin account
- Use a strong password
- Keep one for emergencies only

### Basic Configuration

**1. Set Site Title and Tagline**
- Settings > General
- Site Title: Your website name
- Tagline: Brief description

**2. Configure Timezone**
- Settings > General
- Select your timezone

**3. Set Permalink Structure**
- Settings > Permalinks
- Choose "Post name" (best for SEO)

**4. Visibility and Reading Settings**
- Settings > Reading
- Set homepage to static page (if you want)
- Adjust posts per page

### Optional but Recommended

**1. Install Essential Plugins**
- Yoast SEO (SEO optimization)
- Wordfence Security (security)
- Jetpack (backup and performance)

**2. Change Your Theme**
- Appearance > Themes
- Choose from thousands of free themes

**3. Create First Pages**
- Home page
- About page
- Contact page

---

## Troubleshooting Common Installation Issues

### Issue 1: "Error Establishing Database Connection"

**Cause**: Database credentials are wrong

**Solution**:
1. Check your database name, username, password
2. Usually stored in `wp-config.php`
3. Contact hosting support for correct credentials

### Issue 2: "WordPress Address and Site Address are different"

**Cause**: Settings mismatch

**Solution**:
1. Go to Settings > General
2. Make sure both URLs match exactly
3. Both should include `https://`

### Issue 3: "Page not found" or "404 errors"

**Cause**: Permalink structure issue

**Solution**:
1. Go to Settings > Permalinks
2. Change to "Post name"
3. Save changes
4. If still broken, contact hosting support about .htaccess

### Issue 4: "Connection Timed Out"

**Cause**: Server is slow or overloaded

**Solution**:
1. Wait a few minutes and try again
2. Contact hosting support if persistent
3. Consider upgrading hosting plan

---

## Manual Installation (Optional - For Advanced Users)

If one-click installation isn't available:

### Step 1: Download WordPress

1. Go to [wordpress.org](https://wordpress.org/download)
2. Download the latest version (ZIP file)
3. Extract the file on your computer

### Step 2: Create a Database

1. Log into your hosting control panel
2. Find "MySQL Databases" or similar
3. Create new database
4. Create new user with password
5. Grant user ALL privileges to database
6. Note down: database name, username, password

### Step 3: Upload WordPress Files

1. Connect via FTP to your server
2. Upload WordPress files to public_html directory
3. If installing in subdirectory, create folder first

### Step 4: Run Installation

1. Go to `yourdomain.com/wp-admin/install.php`
2. Select your language
3. Click "Let's Go!"
4. Enter your database information
5. Complete the setup form
6. Finish installation

---

## Quick Reference: Installation Checklist

```
Pre-Installation:
☐ Choose hosting with PHP 7.4+ and MySQL 5.7+
☐ Create hosting account
☐ Access hosting control panel

 Installation:
☐ Use one-click installation tool
☐ Configure domain and directory
☐ Create admin username and password
☐ Set site title and description
☐ Complete installation

Post-Installation:
☐ Log in to WordPress dashboard
☐ Change admin password
☐ Enable HTTPS
☐ Delete sample content
☐ Configure basic settings
☐ Set permalink structure
☐ Create basic pages
☐ Install security plugin
```

---

## Key Takeaways

1. **WordPress has simple requirements**: PHP 7.4+ and MySQL 5.7+
2. **One-click installation is easiest**: Takes just 5 minutes
3. **Admin security is critical**: Use strong passwords and unique username
4. **Initial setup matters**: Configure settings immediately after installation
5. **HTTPS is essential**: Always use secure connections
6. **Delete sample content**: Clean up default posts and pages

---

## Practical Exercise

### Exercise 1: Install WordPress (If You Haven't)

If you have hosting:
1. Log into your control panel
2. Find the installation tool
3. Complete WordPress installation
4. Login and complete initial setup
5. Delete sample content

### Exercise 2: Explore Your Dashboard

1. Take a screenshot of your WordPress dashboard
2. Click on each menu item in the sidebar
3. Explore what's available
4. Read the help text on each page
5. Note features you want to use

### Exercise 3: Change Your Settings

1. Go to Settings > General
2. Change your site title and description
3. Go to Settings > Permalinks
4. Change to "Post name" permalink structure
5. Visit a post to confirm it works

---

## Quick Quiz

### Questions:

1. **What's the minimum PHP version for WordPress?**
   - A) 5.2
   - B) 5.6.20
   - C) 7.4
   - **Answer**: C (recommended)

2. **What's the easiest installation method?**
   - A) FTP upload
   - B) One-click installation
   - C) Command line
   - **Answer**: B

3. **Why should you delete the "admin" username?**
   - A) It's confusing
   - B) It's a security risk
   - C) WordPress won't work with it
   - **Answer**: B

4. **What should you always use?**
   - A) HTTP
   - B) HTTPS
   - C) FTP
   - **Answer**: B

---

## What's Next?

Now that WordPress is installed, the next lesson covers:

🎨 **Dashboard Overview** - A complete tour of your WordPress control center

**Topics covered**:
- Dashboard layout and widgets
- Navigation and menu system
- Admin bar and quick access
- Screen options and customization
- Theme and plugin management

---

## Resources

- [Official WordPress Installation Guide](https://wordpress.org/support/article/how-to-install-wordpress/)
- [WordPress Server Requirements](https://wordpress.org/support/article/requirements/)
- [Hosting Recommendations](https://wordpress.org/hosting/)
- [WordPress Support Forums](https://wordpress.org/support/forums/)

---

## Summary

**WordPress installation is simple!** Most modern hosting providers make it one-click, taking just 5 minutes. The key steps are:

1. **Choose hosting** that meets WordPress requirements
2. **Use one-click installer** for ease
3. **Secure your site** with strong passwords and HTTPS
4. **Configure basic settings** immediately
5. **Clean up sample content** before starting

Your WordPress site is now ready to use!

---

**Lesson Complete!** ✅

Ready for the next lesson? Proceed to [03-dashboard-overview.md](./03-dashboard-overview.md)

[Back to Chapter Overview](./README.md) | [Back to Course Index](../../README.md)
