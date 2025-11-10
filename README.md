# KC Nails Landing Page - Maintenance & Customization Guide

Welcome! This comprehensive guide will help you maintain and customize your KC Nails landing page, even if you're new to web development. We'll walk through everything step-by-step with clear examples.

---

## Table of Contents

1. [Getting Started](#getting-started)
2. [Understanding the Page Structure](#understanding-the-page-structure)
3. [Updating Text Content](#updating-text-content)
4. [Customizing with Tailwind CSS](#customizing-with-tailwind-css)
5. [Fixing and Managing Links](#fixing-and-managing-links)
6. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
7. [Troubleshooting Common Issues](#troubleshooting-common-issues)
8. [Best Practices](#best-practices)

---

## Getting Started

### What You Need

- A text editor (we recommend [Visual Studio Code](https://code.visualstudio.com/) - it's free!)
- Your `index.html` file
- A web browser to preview changes
- Basic understanding of HTML tags (don't worry, we'll explain everything!)

### How to Edit the File

1. **Open the file**: Right-click on `index.html` → Select "Open with" → Choose your text editor
2. **Make changes**: Follow the instructions in this guide
3. **Save**: Press `Ctrl+S` (Windows) or `Cmd+S` (Mac)
4. **Preview**: Open the file in your browser to see changes

---

## Understanding the Page Structure

Your landing page is organized into clear sections. Here's what each section contains:

```
📄 index.html
├── Header (Navigation Menu)
├── Hero Section (Main Banner)
├── Features Section (3 Feature Cards)
├── Benefits Section (3 Benefit Cards)
├── Testimonials Section (4 Customer Reviews)
├── About Us Section
├── FAQ Section (5 Questions)
├── CTA Section (Call to Action)
└── Footer (Links & Contact Info)
```

### Finding Sections in Your Code

Each major section starts with a comment. For example:

```html
<!-- Header Navigation -->
<header class="sticky top-0 z-50 bg-white border-b border-gray-100 soft-shadow">
```

**Tip**: Use `Ctrl+F` (or `Cmd+F` on Mac) to search for these comments. It's much faster than scrolling!

---

## Updating Text Content

This section shows you exactly where to find and change text on your page.

### Header & Navigation

**Location**: Lines 25-45 (approximately)

**What to change**:

```html
<!-- BEFORE -->
<a href="#" class="text-2xl font-bold bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent">
    KC Nails
</a>

<!-- AFTER - Change "KC Nails" to your brand name -->
<a href="#" class="text-2xl font-bold bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent">
    Your Brand Name
</a>
```

**Navigation Menu Items** (Lines 30-42):

The navigation has links that say "Features", "Benefits", etc. To change these:

```html
<!-- BEFORE -->
<a href="#features" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">Features</a>

<!-- AFTER -->
<a href="#features" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">Your Custom Text</a>
```

**Important**: Keep the `href="#features"` part the same - it links to sections on the page.

### Hero Section (Main Banner)

**Location**: Lines 70-120 (approximately)

This is the large banner at the top with the main headline.

**Main Headline**:

```html
<!-- BEFORE -->
<h1 class="text-4xl sm:text-5xl md:text-6xl lg:text-7xl font-bold tracking-tight text-gray-900 leading-tight">
    Nail Perfection,
    <span class="bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent">Ukrainian Heartbeat</span>
</h1>

<!-- AFTER -->
<h1 class="text-4xl sm:text-5xl md:text-6xl lg:text-7xl font-bold tracking-tight text-gray-900 leading-tight">
    Your Main Headline,
    <span class="bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent">Colored Part</span>
</h1>
```

**Subheading**:

```html
<!-- BEFORE -->
<p class="text-lg sm:text-xl md:text-2xl text-gray-600 max-w-3xl mx-auto leading-relaxed font-light">
    Experience exquisite nail artistry while contributing to a vibrant Ukrainian community. Every purchase supports local artists and cultural celebration.
</p>

<!-- AFTER -->
<p class="text-lg sm:text-xl md:text-2xl text-gray-600 max-w-3xl mx-auto leading-relaxed font-light">
    Your custom description here. Make it compelling and clear about what you offer.
</p>
```

**Statistics Section** (Lines 103-125):

These are the "500+", "10K+", "100%" numbers:

```html
<!-- BEFORE -->
<div>
    <p class="text-3xl font-bold text-purple-600">500+</p>
    <p class="text-gray-600 font-medium">Exclusive Designs</p>
</div>

<!-- AFTER -->
<div>
    <p class="text-3xl font-bold text-purple-600">YOUR NUMBER</p>
    <p class="text-gray-600 font-medium">Your Stat Label</p>
</div>
```

### Features Section

**Location**: Lines 130-230 (approximately)

There are 3 feature cards. Here's how to update the first one:

**Feature Title**:

```html
<!-- BEFORE -->
<h3 class="text-2xl font-bold text-gray-900 mb-3">Exclusive Collections</h3>

<!-- AFTER -->
<h3 class="text-2xl font-bold text-gray-900 mb-3">Your Feature Title</h3>
```

**Feature Description**:

```html
<!-- BEFORE -->
<p class="text-gray-600 leading-relaxed mb-4 font-light">
    Access limited-edition nail designs curated by master artists from across Ukraine...
</p>

<!-- AFTER -->
<p class="text-gray-600 leading-relaxed mb-4 font-light">
    Your feature description here. Keep it clear and benefit-focused.
</p>
```

**Bullet Points** (Feature highlights):

```html
<!-- BEFORE -->
<li class="flex items-center gap-2 text-gray-700">
    <svg class="w-5 h-5 text-purple-600" fill="currentColor" viewBox="0 0 20 20">
        <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
    </svg>
    <span>Limited Edition Releases</span>
</li>

<!-- AFTER -->
<li class="flex items-center gap-2 text-gray-700">
    <svg class="w-5 h-5 text-purple-600" fill="currentColor" viewBox="0 0 20 20">
        <path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path>
    </svg>
    <span>Your Benefit Text</span>
</li>
```

**To update all 3 features**: Repeat this process for the second and third feature cards (they're right below the first one).

### Benefits Section

**Location**: Lines 235-350 (approximately)

Similar to features, there are 3 benefit cards. Update them the same way:

```html
<!-- BEFORE -->
<h3 class="text-2xl font-bold text-gray-900 mb-3">Master New Techniques</h3>
<p class="text-gray-600 leading-relaxed font-light mb-4">
    Develop advanced nail art skills through structured learning paths...
</p>

<!-- AFTER -->
<h3 class="text-2xl font-bold text-gray-900 mb-3">Your Benefit Title</h3>
<p class="text-gray-600 leading-relaxed font-light mb-4">
    Your benefit description here.
</p>
```

### Testimonials Section

**Location**: Lines 355-480 (approximately)

There are 4 customer testimonials. Here's how to update one:

```html
<!-- BEFORE -->
<p class="text-gray-700 leading-relaxed mb-4 font-light">
    "The tutorials have completely transformed my nail art skills. I went from basic designs to creating intricate 3D art in just three months!"
</p>
<div class="border-t border-gray-200 pt-4">
    <p class="font-semibold text-gray-900">Maria Kosenko</p>
    <p class="text-sm text-gray-600">Professional Nail Artist</p>
</div>

<!-- AFTER -->
<p class="text-gray-700 leading-relaxed mb-4 font-light">
    "Your customer testimonial here. Make it specific and genuine."
</p>
<div class="border-t border-gray-200 pt-4">
    <p class="font-semibold text-gray-900">Customer Name</p>
    <p class="text-sm text-gray-600">Customer Title/Role</p>
</div>
```

**Note**: Each testimonial also has 5 star ratings. The stars are created with SVG code - you don't need to change this unless you want to show fewer stars.

### About Us Section

**Location**: Lines 485-520 (approximately)

**Section Title**:

```html
<!-- BEFORE -->
<h2 class="text-3xl sm:text-4xl md:text-5xl font-bold text-gray-900 mb-4 tracking-tight">
    About KC Nails
</h2>

<!-- AFTER -->
<h2 class="text-3xl sm:text-4xl md:text-5xl font-bold text-gray-900 mb-4 tracking-tight">
    About Your Company
</h2>
```

**About Text** (Two paragraphs):

```html
<!-- BEFORE -->
<p class="text-lg leading-relaxed text-gray-700 font-light">
    KC Nails was founded with a simple yet powerful vision: to celebrate the artistry of nail design...
</p>

<!-- AFTER -->
<p class="text-lg leading-relaxed text-gray-700 font-light">
    Your company story and mission here. Keep it authentic and inspiring.
</p>
```

**About Statistics**:

```html
<!-- BEFORE -->
<div class="text-center p-6">
    <div class="text-4xl font-bold text-purple-600 mb-2">500+</div>
    <p class="text-gray-600 font-medium">Exclusive Designs</p>
</div>

<!-- AFTER -->
<div class="text-center p-6">
    <div class="text-4xl font-bold text-purple-600 mb-2">YOUR NUMBER</div>
    <p class="text-gray-600 font-medium">Your Statistic</p>
</div>
```

### FAQ Section

**Location**: Lines 525-660 (approximately)

**FAQ Title**:

```html
<!-- BEFORE -->
<h2 class="text-3xl sm:text-4xl md:text-5xl font-bold text-gray-900 mb-4 tracking-tight">
    Frequently Asked Questions
</h2>

<!-- AFTER -->
<h2 class="text-3xl sm:text-4xl md:text-5xl font-bold text-gray-900 mb-4 tracking-tight">
    Your Section Title
</h2>
```

**FAQ Question and Answer**:

```html
<!-- BEFORE -->
<button class="faq-question w-full px-6 md:px-8 py-5 md:py-6 flex items-center justify-between hover:bg-gray-50 transition-colors duration-300 cursor-pointer">
    <span class="text-lg font-semibold text-gray-900 text-left">
        Do I need to be an experienced nail artist to join?
    </span>
    <!-- Icon stays the same -->
</button>
<div class="faq-answer hidden px-6 md:px-8 pb-6 border-t border-gray-200">
    <p class="text-gray-700 leading-relaxed font-light">
        Absolutely not! KC Nails welcomes artists of all skill levels...
    </p>
</div>

<!-- AFTER -->
<button class="faq-question w-full px-6 md:px-8 py-5 md:py-6 flex items-center justify-between hover:bg-gray-50 transition-colors duration-300 cursor-pointer">
    <span class="text-lg font-semibold text-gray-900 text-left">
        Your FAQ Question Here?
    </span>
    <!-- Icon stays the same -->
</button>
<div class="faq-answer hidden px-6 md:px-8 pb-6 border-t border-gray-200">
    <p class="text-gray-700 leading-relaxed font-light">
        Your FAQ answer here. Be clear and helpful.
    </p>
</div>
```

### Call-to-Action (CTA) Section

**Location**: Lines 665-685 (approximately)

```html
<!-- BEFORE -->
<h2 class="text-3xl sm:text-4xl md:text-5xl font-bold text-white mb-6 tracking-tight leading-tight">
    Ready to Elevate Your Nail Art?
</h2>
<p class="text-lg md:text-xl text-purple-100 max-w-2xl mx-auto mb-10 font-light">
    Join thousands of artists and enthusiasts who are transforming their skills...
</p>

<!-- AFTER -->
<h2 class="text-3xl sm:text-4xl md:text-5xl font-bold text-white mb-6 tracking-tight leading-tight">
    Your CTA Headline
</h2>
<p class="text-lg md:text-xl text-purple-100 max-w-2xl mx-auto mb-10 font-light">
    Your compelling CTA description.
</p>
```

### Footer

**Location**: Lines 690-760 (approximately)

**Brand Name in Footer**:

```html
<!-- BEFORE -->
<h3 class="text-2xl font-bold bg-gradient-to-r from-purple-400 to-pink-400 bg-clip-text text-transparent mb-4">
    KC Nails
</h3>

<!-- AFTER -->
<h3 class="text-2xl font-bold bg-gradient-to-r from-purple-400 to-pink-400 bg-clip-text text-transparent mb-4">
    Your Brand Name
</h3>
```

**Footer Description**:

```html
<!-- BEFORE -->
<p class="text-gray-400 leading-relaxed font-light">
    Celebrating nail artistry while supporting Ukrainian communities through exclusive collections and expert education.
</p>

<!-- AFTER -->
<p class="text-gray-400 leading-relaxed font-light">
    Your company description for the footer.
</p>
```

**Footer Contact Email**:

```html
<!-- BEFORE -->
<a href="mailto:iainhmunro@gmail.com" class="text-gray-400 hover:text-purple-400 transition-colors duration-300 flex items-center gap-2">
    <i class="fas fa-envelope"></i>
    iainhmunro@gmail.com
</a>

<!-- AFTER -->
<a href="mailto:youremail@example.com" class="text-gray-400 hover:text-purple-400 transition-colors duration-300 flex items-center gap-2">
    <i class="fas fa-envelope"></i>
    youremail@example.com
</a>
```

**Copyright Year**:

```html
<!-- BEFORE -->
<p class="text-gray-400 text-sm font-light">
    &copy; 2025 KC Nails. All rights reserved. Celebrating artistry and supporting communities.
</p>

<!-- AFTER -->
<p class="text-gray-400 text-sm font-light">
    &copy; 2025 Your Company Name. All rights reserved. Your tagline here.
</p>
```

---

## Customizing with Tailwind CSS

Tailwind CSS is a utility-first CSS framework. Instead of writing custom CSS, you add class names to HTML elements. Here's what you need to know:

### Understanding Tailwind Classes

**Example**: `text-3xl font-bold text-purple-600`

- `text-3xl` = Makes text very large
- `font-bold` = Makes text bold/thick
- `text-purple-600` = Makes text purple

### Common Classes You'll See

| Class | What It Does | Example |
|-------|-------------|---------|
| `text-lg`, `text-2xl`, `text-3xl` | Controls text size | Larger numbers = bigger text |
| `font-bold`, `font-semibold`, `font-light` | Controls text weight | How thick the text is |
| `text-gray-600`, `text-purple-600` | Controls text color | Color name + number (darker = higher number) |
| `bg-white`, `bg-purple-600` | Background color | `bg-` prefix for background |
| `px-4`, `py-6`, `p-8` | Padding (space inside) | `x` = left/right, `y` = top/bottom |
| `mb-4`, `mt-6` | Margin (space outside) | `m` = margin, `b` = bottom, `t` = top |
| `rounded-lg`, `rounded-2xl` | Rounded corners | Larger number = more rounded |
| `shadow-lg`, `soft-shadow` | Drop shadows | Creates depth |

### Responsive Classes

Tailwind lets you change styles on different screen sizes:

```html
<h1 class="text-2xl md:text-4xl lg:text-6xl">
    This text is:
    - Small on phones (text-2xl)
    - Medium on tablets (md:text-4xl)
    - Large on desktop (lg:text-6xl)
</h1>
```

**Screen Size Prefixes**:
- `sm:` = Small devices (phones)
- `md:` = Medium devices (tablets)
- `lg:` = Large devices (desktops)

### Color Customization

All colors follow this pattern: `color-number`

```html
<!-- Text colors -->
<p class="text-purple-600">Purple text</p>
<p class="text-pink-500">Pink text</p>
<p class="text-gray-700">Dark gray text</p>

<!-- Background colors -->
<div class="bg-purple-100">Light purple background</div>
<div class="bg-purple-600">Dark purple background</div>
```

**Number Scale** (50-950):
- 50 = Very light
- 100-300 = Light
- 400-600 = Medium
- 700-900 = Dark
- 950 = Very dark

### Changing the Color Scheme

If you want to change from purple/pink to a different color scheme:

**Find all instances** of `purple-600` and `pink-600`:

```html
<!-- BEFORE - Purple and Pink -->
<div class="bg-gradient-to-r from-purple-600 to-pink-600">

<!-- AFTER - Blue and Cyan -->
<div class="bg-gradient-to-r from-blue-600 to-cyan-600">
```

**Available colors**: red, orange, amber, yellow, lime, green, emerald, teal, cyan, blue, indigo, violet, purple, fuchsia, pink, rose

### Spacing Examples

```html
<!-- Padding: space inside the box -->
<div class="p-4">Small padding inside</div>
<div class="p-8">Large padding inside</div>
<div class="px-4 py-8">4 units left/right, 8 units top/bottom</div>

<!-- Margin: space outside the box -->
<div class="mb-4">Space below this box</div>
<div class="mt-8">Space above this box</div>
```

### Common Customizations

**Make text larger**:
```html
<!-- BEFORE -->
<p class="text-lg">Text</p>

<!-- AFTER -->
<p class="text-2xl">Text</p>  <!-- Bigger -->
```

**Add more padding**:
```html
<!-- BEFORE -->
<div class="p-6">Content</div>

<!-- AFTER -->
<div class="p-10">Content</div>  <!-- More space inside -->
```

**Change border radius (roundedness)**:
```html
<!-- BEFORE -->
<div class="rounded-lg">Box</div>

<!-- AFTER -->
<div class="rounded-3xl">Box</div>  <!-- More rounded -->
```

**Add/remove shadow**:
```html
<!-- BEFORE -->
<div class="soft-shadow">Box</div>

<!-- AFTER -->
<div class="shadow-2xl">Box</div>  <!-- Bigger shadow -->
<!-- Or remove shadow entirely -->
<div>Box</div>
```

---

## Fixing and Managing Links

Links are crucial for navigation. Let's go through every link on your page.

### Understanding Links

A basic link looks like this:

```html
<a href="where-to-go" target="_blank">Link Text</a>
```

- `href` = Where the link goes
- `target="_blank"` = Opens in a new tab
- Link Text = What users see and click

### All Links on Your Page

#### 1. Header Navigation Links

**Location**: Lines 30-42 (Desktop navigation)

These links should point to sections on the same page:

```html
<!-- These are CORRECT - they link to sections below -->
<a href="#features">Features</a>          <!-- Links to Features section -->
<a href="#benefits">Benefits</a>          <!-- Links to Benefits section -->
<a href="#testimonials">Testimonials</a>  <!-- Links to Testimonials section -->
<a href="#faq">FAQ</a>                     <!-- Links to FAQ section -->
```

**✓ These don't need changing** - they work perfectly.

#### 2. "Get Started" Button (Header)

**Location**: Lines 43-46

```html
<!-- BEFORE -->
<a href="https://kcnailsukr.com/" target="_blank" class="px-6 py-2 bg-gradient-to-r from-purple-600 to-pink-600 text-white rounded-full font-semibold button-hover">
    Get Started
</a>

<!-- AFTER - Change to your website -->
<a href="https://yourwebsite.com/" target="_blank" class="px-6 py-2 bg-gradient-to-r from-purple-600 to-pink-600 text-white rounded-full font-semibold button-hover">
    Get Started
</a>
```

**Important**: Replace `https://kcnailsukr.com/` with your actual website URL.

#### 3. Mobile Menu "Get Started" Button

**Location**: Lines 52-54

```html
<!-- BEFORE -->
<a href="https://kcnailsukr.com/" target="_blank" class="block px-4 py-3 mx-4 mt-3 text-center bg-gradient-to-r from-purple-600 to-pink-600 text-white rounded-full font-semibold button-hover">
    Get Started
</a>

<!-- AFTER -->
<a href="https://yourwebsite.com/" target="_blank" class="block px-4 py-3 mx-4 mt-3 text-center bg-gradient-to-r from-purple-600 to-pink-600 text-white rounded-full font-semibold button-hover">
    Get Started
</a>
```

#### 4. Hero Section Buttons

**Location**: Lines 90-101

```html
<!-- BEFORE - "Explore Collections" button -->
<a href="https://kcnailsukr.com/" target="_blank" class="px-8 py-4 bg-gradient-to-r from-purple-600 to-pink-600 text-white rounded-full font-bold text-lg button-hover shadow-lg hover:shadow-xl inline-flex items-center justify-center gap-2">
    <i class="fas fa-sparkles"></i>
    Explore Collections
</a>

<!-- AFTER -->
<a href="https://yourwebsite.com/" target="_blank" class="px-8 py-4 bg-gradient-to-r from-purple-600 to-pink-600 text-white rounded-full font-bold text-lg button-hover shadow-lg hover:shadow-xl inline-flex items-center justify-center gap-2">
    <i class="fas fa-sparkles"></i>
    Explore Collections
</a>
```

```html
<!-- BEFORE - "Learn More" button (this one is correct) -->
<a href="#features" class="px-8 py-4 border-2 border-purple-600 text-purple-600 rounded-full font-bold text-lg button-hover hover:bg-purple-50 inline-flex items-center justify-center gap-2">
    <i class="fas fa-arrow-down"></i>
    Learn More
</a>

<!-- ✓ This one is CORRECT - don't change it -->
```

#### 5. CTA Section Buttons

**Location**: Lines 670-683

```html
<!-- BEFORE - "Get Started Today" button -->
<a href="https://kcnailsukr.com/" target="_blank" class="px-8 py-4 bg-white text-purple-600 rounded-full font-bold text-lg button-hover shadow-lg hover:shadow-xl inline-flex items-center justify-center gap-2">
    <i class="fas fa-star"></i>
    Get Started Today
</a>

<!-- AFTER -->
<a href="https://yourwebsite.com/" target="_blank" class="px-8 py-4 bg-white text-purple-600 rounded-full font-bold text-lg button-hover shadow-lg hover:shadow-xl inline-flex items-center justify-center gap-2">
    <i class="fas fa-star"></i>
    Get Started Today
</a>
```

```html
<!-- BEFORE - "Learn More" button (this one is correct) -->
<a href="#faq" class="px-8 py-4 border-2 border-white text-white rounded-full font-bold text-lg button-hover hover:bg-white hover:bg-opacity-10 inline-flex items-center justify-center gap-2">
    <i class="fas fa-question-circle"></i>
    Learn More
</a>

<!-- ✓ This one is CORRECT - don't change it -->
```

#### 6. Footer Links

**Location**: Lines 715-745

**Quick Links Section**:
```html
<!-- These are CORRECT - they link to sections on the page -->
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#testimonials">Testimonials</a>
<a href="#faq">FAQ</a>
```

**Resources Section** (These need to be created - see next section):
```html
<!-- BEFORE -->
<a href="blog.html">Blog</a>
<a href="privacy.html">Privacy Policy</a>
<a href="terms.html">Terms of Service</a>
<a href="https://kcnailsukr.com/" target="_blank">Shop</a>

<!-- AFTER - Update the external link, keep the internal ones for now -->
<a href="blog.html">Blog</a>
<a href="privacy.html">Privacy Policy</a>
<a href="terms.html">Terms of Service</a>
<a href="https://yourwebsite.com/" target="_blank">Shop</a>
```

**Contact Section**:
```html
<!-- BEFORE -->
<a href="mailto:iainhmunro@gmail.com">
    <i class="fas fa-envelope"></i>
    iainhmunro@gmail.com
</a>

<!-- AFTER -->
<a href="mailto:youremail@example.com">
    <i class="fas fa-envelope"></i>
    youremail@example.com
</a>
```

**Social Media Links** (Lines 750-765):
```html
<!-- BEFORE -->
<a href="#" class="text-gray-400 hover:text-purple-400 transition-colors duration-300 text-xl">
    <i class="fab fa-facebook"></i>
</a>

<!-- AFTER - Add your actual social media URLs -->
<a href="https://facebook.com/yourpage" target="_blank" class="text-gray-400 hover:text-purple-400 transition-colors duration-300 text-xl">
    <i class="fab fa-facebook"></i>
</a>
```

**Repeat for**: Instagram, Twitter, Pinterest

**Copyright Section**:
```html
<!-- BEFORE -->
<div class="flex gap-6 mt-4 md:mt-0">
    <a href="privacy.html">Privacy Policy</a>
    <a href="terms.html">Terms of Service</a>
    <a href="blog.html">Blog</a>
</div>

<!-- Keep these the same - we'll create these pages in the next section -->
```

### Quick Reference: All External Links to Update

Find and replace these URLs:

| Current URL | Replace With |
|------------|--------------|
| `https://kcnailsukr.com/` | Your website URL |
| `iainhmunro@gmail.com` | Your email |
| `#` (for social media) | Your actual social media URLs |

---

## Adding Privacy and Terms Pages

Your footer already has links to `privacy.html` and `terms.html`, but these files don't exist yet. Let's create them.

### Step 1: Create the Privacy Policy Page

1. **Open your text editor**
2. **Create a new file**: File → New File
3. **Save it as**: `privacy.html` (in the same folder as `index.html`)
4. **Copy this code** into the file:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Privacy Policy for KC Nails">
    <title>Privacy Policy | KC Nails</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        html {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-white text-gray-900 font-sans">
    <!-- Header Navigation -->
    <header class="sticky top-0 z-50 bg-white border-b border-gray-100 shadow-sm">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <div class="flex-shrink-0">
                    <a href="index.html" class="text-2xl font-bold bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent">
                        KC Nails
                    </a>
                </div>
                <div class="hidden md:flex items-center space-x-8">
                    <a href="index.html" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">Home</a>
                    <a href="privacy.html" class="text-purple-600 font-medium">Privacy Policy</a>
                    <a href="terms.html" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">Terms</a>
                </div>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <main class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 py-20">
        <h1 class="text-4xl font-bold text-gray-900 mb-8">Privacy Policy</h1>
        
        <div class="prose prose-lg max-w-none text-gray-700 space-y-6">
            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Introduction</h2>
                <p class="leading-relaxed">
                    At KC Nails, we are committed to protecting your privacy. This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you visit our website.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Information We Collect</h2>
                <p class="leading-relaxed">
                    We may collect information about you in a variety of ways. The information we may collect on the site includes:
                </p>
                <ul class="list-disc list-inside space-y-2 ml-4">
                    <li>Personal data (name, email address, phone number) that you voluntarily submit</li>
                    <li>Information about your browsing activities and preferences</li>
                    <li>Device information (browser type, IP address, operating system)</li>
                </ul>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">How We Use Your Information</h2>
                <p class="leading-relaxed">
                    Having accurate information about you permits us to provide you with a smooth, efficient, and customized experience. Specifically, we may use information collected about you via the site to:
                </p>
                <ul class="list-disc list-inside space-y-2 ml-4">
                    <li>Generate a personal profile about you so that future visits to the site will be personalized</li>
                    <li>Increase the efficiency and operation of the site</li>
                    <li>Monitor and analyze usage and trends to improve your experience with the site</li>
                    <li>Notify you of updates to the site</li>
                </ul>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Disclosure of Your Information</h2>
                <p class="leading-relaxed">
                    We may share your information in the following situations:
                </p>
                <ul class="list-disc list-inside space-y-2 ml-4">
                    <li>By law or to protect our rights</li>
                    <li>To comply with legal obligations</li>
                    <li>With service providers who assist us in operating our website</li>
                </ul>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Security of Your Information</h2>
                <p class="leading-relaxed">
                    We use administrative, technical, and physical security measures to protect your personal information. However, perfect security cannot be guaranteed on the Internet.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Contact Us</h2>
                <p class="leading-relaxed">
                    If you have questions or comments about this Privacy Policy, please contact us at:
                </p>
                <p class="mt-4">
                    <strong>Email:</strong> <a href="mailto:iainhmunro@gmail.com" class="text-purple-600 hover:text-pink-600">iainhmunro@gmail.com</a>
                </p>
            </section>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-12 mt-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p class="text-gray-400 text-sm">
                &copy; 2025 KC Nails. All rights reserved.
            </p>
        </div>
    </footer>
</body>
</html>
```

**To customize this file**:

1. Change `iainhmunro@gmail.com` to your email
2. Update the content in each section to match your privacy practices
3. Add any additional sections relevant to your business

### Step 2: Create the Terms of Service Page

1. **Create a new file**: File → New File
2. **Save it as**: `terms.html` (in the same folder as `index.html`)
3. **Copy this code** into the file:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Terms of Service for KC Nails">
    <title>Terms of Service | KC Nails</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        html {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-white text-gray-900 font-sans">
    <!-- Header Navigation -->
    <header class="sticky top-0 z-50 bg-white border-b border-gray-100 shadow-sm">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <div class="flex-shrink-0">
                    <a href="index.html" class="text-2xl font-bold bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent">
                        KC Nails
                    </a>
                </div>
                <div class="hidden md:flex items-center space-x-8">
                    <a href="index.html" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">Home</a>
                    <a href="privacy.html" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">Privacy</a>
                    <a href="terms.html" class="text-purple-600 font-medium">Terms of Service</a>
                </div>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <main class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 py-20">
        <h1 class="text-4xl font-bold text-gray-900 mb-8">Terms of Service</h1>
        
        <div class="prose prose-lg max-w-none text-gray-700 space-y-6">
            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Agreement to Terms</h2>
                <p class="leading-relaxed">
                    These Terms of Service constitute a legally binding agreement made between you, whether personally or on behalf of an entity ("you") and KC Nails ("we," "us," "our," or "Company"), concerning your access to and use of the website.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Intellectual Property Rights</h2>
                <p class="leading-relaxed">
                    Unless otherwise indicated, the site is our proprietary property, and all source code, databases, functionality, software, website designs, audio, video, text, photographs, and graphics on the site (collectively, the "Content") and the trademarks, service marks, and logos contained therein (the "Marks") are owned or controlled by us or licensed to us.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">User Representations</h2>
                <p class="leading-relaxed">
                    By using this site, you represent and warrant that:
                </p>
                <ul class="list-disc list-inside space-y-2 ml-4">
                    <li>All registration information you submit is true, accurate, and current</li>
                    <li>You will maintain the confidentiality of your account information</li>
                    <li>You will not use the site for any illegal or unauthorized purpose</li>
                    <li>You will comply with all applicable laws and regulations</li>
                </ul>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">User Contributions</h2>
                <p class="leading-relaxed">
                    The site may invite you to chat, contribute to, or participate in blogs, message boards, online forums, and other functionality, and may provide you with the opportunity to create, submit, post, display, transmit, perform, publish, distribute, or broadcast content and materials to us or on the site.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Disclaimer of Warranties</h2>
                <p class="leading-relaxed">
                    The site is provided on an "as-is" and "as-available" basis. We make no warranties, expressed or implied, regarding the site. To the fullest extent permissible pursuant to applicable law, we disclaim all warranties, express or implied.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Limitation of Liability</h2>
                <p class="leading-relaxed">
                    In no event shall the Company or its suppliers be liable for any damages (including, without limitation, damages for loss of data or profit, or due to business interruption) arising out of or in connection with the use or inability to use the materials on the site.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Indemnification</h2>
                <p class="leading-relaxed">
                    You agree to defend, indemnify, and hold harmless our company and its officers, directors, employees, and agents from and against any claims, damages, losses, liabilities, and expenses arising out of or in any way connected with your access to or use of the site.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Modifications and Interruptions</h2>
                <p class="leading-relaxed">
                    We reserve the right to modify or discontinue, temporarily or permanently, the site (or any part thereof) with or without notice. You agree that we shall not be liable to you or to any third party for any modification, suspension, or discontinuance of the site.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Contact Us</h2>
                <p class="leading-relaxed">
                    If you have any questions about these Terms of Service, please contact us at:
                </p>
                <p class="mt-4">
                    <strong>Email:</strong> <a href="mailto:iainhmunro@gmail.com" class="text-purple-600 hover:text-pink-600">iainhmunro@gmail.com</a>
                </p>
            </section>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-12 mt-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p class="text-gray-400 text-sm">
                &copy; 2025 KC Nails. All rights reserved.
            </p>
        </div>
    </footer>
</body>
</html>
```

**To customize this file**:

1. Change `iainhmunro@gmail.com` to your email
2. Update the content to match your actual terms
3. Add any specific terms relevant to your business

### Step 3: Verify Links Work

1. **Save both new files** in the same folder as `index.html`
2. **Open `index.html`** in your browser
3. **Scroll to the footer**
4. **Click "Privacy Policy"** - it should go to `privacy.html`
5. **Click "Terms of Service"** - it should go to `terms.html`
6. **Click "Home"** on those pages - it should return to `index.html`

### Step 4: Create a Blog Page (Optional)

The footer also links to `blog.html`. If you want this to work, create it similarly:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Blog | KC Nails">
    <title>Blog | KC Nails</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body class="bg-white text-gray-900 font-sans">
    <!-- Header Navigation -->
    <header class="sticky top-0 z-50 bg-white border-b border-gray-100 shadow-sm">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <div class="flex-shrink-0">
                    <a href="index.html" class="text-2xl font-bold bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent">
                        KC Nails
                    </a>
                </div>
                <div class="hidden md:flex items-center space-x-8">
                    <a href="index.html" class="text-gray-700 hover:text-purple-600 transition-colors duration-300 font-medium">Home</a>
                    <a href="blog.html" class="text-purple-600 font-medium">Blog</a>
                </div>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <main class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 py-20">
        <h1 class="text-4xl font-bold text-gray-900 mb-8">Blog</h1>
        <p class="text-lg text-gray-600">Coming soon! Check back for nail art tips, tutorials, and community stories.</p>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-12 mt-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p class="text-gray-400 text-sm">
                &copy; 2025 KC Nails. All rights reserved.
            </p>
        </div>
    </footer>
</body>
</html>
```

Save this as `blog.html` in the same folder.

---

## Troubleshooting Common Issues

### Problem: Links Don't Work

**Symptoms**: Clicking a link does nothing or goes to the wrong page

**Solutions**:

1. **Check the href attribute**:
   ```html
   <!-- WRONG - Missing # for internal links -->
   <a href="features">Features</a>
   
   <!-- CORRECT -->
   <a href="#features">Features</a>
   ```

2. **Check file names match exactly**:
   ```html
   <!-- WRONG - File is named "privacy.html" but link says "privacypolicy.html" -->
   <a href="privacypolicy.html">Privacy</a>
   
   <!-- CORRECT -->
   <a href="privacy.html">Privacy</a>
   ```

3. **Verify files are in the same folder**:
   - `index.html`
   - `privacy.html`
   - `terms.html`
   - `blog.html`
   
   All should be in the same directory.

### Problem: Text Looks Wrong or Doesn't Display

**Symptoms**: Text appears too small, wrong color, or is cut off

**Solutions**:

1. **Check for typos in class names**:
   ```html
   <!-- WRONG - "text-3x1" (with letter L) -->
   <p class="text-3x1">Text</p>
   
   <!-- CORRECT -->
   <p class="text-3xl">Text</p>
   ```

2. **Verify color names**:
   ```html
   <!-- WRONG - "purpl" is not a valid color -->
   <p class="text-purpl-600">Text</p>
   
   <!-- CORRECT -->
   <p class="text-purple-600">Text</p>
   ```

3. **Check closing tags**:
   ```html
   <!-- WRONG - Missing closing </p> tag -->
   <p class="text-lg">Text
   <p class="text-lg">More text</p>
   
   <!-- CORRECT -->
   <p class="text-lg">Text</p>
   <p class="text-lg">More text</p>
   ```

### Problem: Mobile Menu Doesn't Work

**Symptoms**: The hamburger menu button doesn't open/close on mobile

**Solutions**:

1. **Verify JavaScript is not broken**: Check that all `<script>` tags are properly closed
2. **Check browser console**: Press F12 → Console tab → Look for error messages
3. **Test in different browser**: Sometimes browser cache causes issues

### Problem: Page Layout Looks Broken

**Symptoms**: Elements overlap, text is unreadable, or spacing is wrong

**Solutions**:

1. **Check for unclosed HTML tags**:
   ```html
   <!-- WRONG - <div> is never closed -->
   <div class="container">
       <p>Content</p>
   
   <!-- CORRECT -->
   <div class="container">
       <p>Content</p>
   </div>
   ```

2. **Verify Tailwind CSS is loading**:
   - Check that this line exists in the `<head>`:
   ```html
   <script src="https://cdn.tailwindcss.com"></script>
   ```

3. **Clear browser cache**:
   - Press Ctrl+Shift+Delete (or Cmd+Shift+Delete on Mac)
   - Select "Cached images and files"
   - Click "Clear"

### Problem: Colors Don't Look Right

**Symptoms**: Purple/pink colors look different than expected

**Solutions**:

1. **Verify gradient syntax**:
   ```html
   <!-- WRONG - Missing "to-" in gradient -->
   <div class="bg-gradient-to-r from-purple-600 purple-600">
   
   <!-- CORRECT -->
   <div class="bg-gradient-to-r from-purple-600 to-pink-600">
   ```

2. **Check color numbers**:
   - Lower numbers (50-300) = Light colors
   - Higher numbers (700-950) = Dark colors
   - Use 600 for medium colors

### Problem: Images Don't Display

**Symptoms**: You see broken image icons instead of pictures

**Solutions**:

1. **Verify file path**:
   ```html
   <!-- WRONG - File doesn't exist at this path -->
   <img src="images/photo.jpg">
   
   <!-- CORRECT - Make sure the file actually exists -->
   <img src="./images/photo.jpg">
   ```

2. **Check file names are exact** (case-sensitive on some systems):
   - File: `MyPhoto.jpg`
   - Link: `myPhoto.jpg` ❌ (won't work)
   - Link: `MyPhoto.jpg` ✓ (correct)

### Problem: Page Doesn't Scroll Smoothly

**Symptoms**: Clicking anchor links jumps instantly instead of smoothly scrolling

**Solutions**:

1. **Verify smooth scroll CSS exists**:
   ```html
   <style>
       html {
           scroll-behavior: smooth;  <!-- This line is important -->
       }
   </style>
   ```

2. **Check for JavaScript errors**: Press F12 and look at the Console tab

---

## Best Practices

### 1. Always Backup Your Files

Before making changes:
- Copy `index.html` and save it as `index-backup.html`
- If something breaks, you can restore from the backup

### 2. Make One Change at a Time

- Change one thing
- Save and test
- Make sure it works
- Then change something else

This makes it easy to find problems if something breaks.

### 3. Use Consistent Formatting

Keep your code readable:

```html
<!-- GOOD - Easy to read -->
<div class="p-8 rounded-2xl border border-gray-100 soft-shadow">
    <h3 class="text-2xl font-bold text-gray-900 mb-3">Title</h3>
    <p class="text-gray-600">Description</p>
</div>

<!-- HARD TO READ -->
<div class="p-8 rounded-2xl border border-gray-100 soft-shadow"><h3 class="text-2xl font-bold text-gray-900 mb-3">Title</h3><p class="text-gray-600">Description</p></div>
```

### 4. Keep Responsive Design in Mind

Always test on different screen sizes:
- Mobile (phone)
- Tablet
- Desktop

The classes like `md:` and `lg:` handle this automatically, but verify it works.

### 5. Update Related Content

If you change something in one place, update similar content elsewhere:

**Example**: If you change the brand name from "KC Nails" to "Your Brand":
- Update it in the header
- Update it in the footer
- Update it in the About section
- Update it in the title tag

### 6. Test All Links Regularly

Create a checklist and test monthly:
- [ ] Header "Get Started" button
- [ ] Hero "Explore Collections" button
- [ ] All navigation links
- [ ] Footer links
- [ ] Social media links

### 7. Keep Your File Structure Organized

```
📁 Your Project Folder
├── 📄 index.html (main page)
├── 📄 privacy.html (privacy policy)
├── 📄 terms.html (terms of service)
├── 📄 blog.html (blog page)
├── 📁 images/ (folder for images)
│   ├── 📷 logo.png
│   └── 📷 photo.jpg
└── 📁 css/ (optional folder for custom styles)
    └── 📄 custom.css
```

### 8. Use Comments to Mark Your Changes

```html
<!-- CUSTOM: Changed this button color from purple to blue -->
<a href="#" class="bg-blue-600">Button</a>

<!-- CUSTOM: Updated email address -->
<a href="mailto:newemail@example.com">Email</a>
```

This helps you remember what you changed later.

### 9. Test Before Publishing

Before uploading to your web server:

1. Open in multiple browsers (Chrome, Firefox, Safari)
2. Test on mobile device or use browser's mobile view (F12)
3. Click every link
4. Read all text for typos
5. Check colors and spacing

### 10. Keep Tailwind CSS Classes Organized

Group related classes together:

```html
<!-- GOOD - Organized -->
<div class="flex items-center justify-between gap-4 p-6 bg-white rounded-lg border border-gray-200 shadow-md hover:shadow-lg transition-shadow">

<!-- CONFUSING - Random order -->
<div class="shadow-md p-6 gap-4 border border-gray-200 rounded-lg flex bg-white items-center justify-between hover:shadow-lg transition-shadow">
```

---

## Quick Reference Guide

### Commonly Changed Elements

| Element | How to Find | What to Change |
|---------|------------|-----------------|
| Brand Name | Search: "KC Nails" | Replace with your brand name |
| External Links | Search: "https://" | Replace URLs with your website |
| Email | Search: "mailto:" | Replace with your email |
| Colors | Search: "purple-600" or "pink-600" | Change to your brand colors |
| Text Content | Each section | Update to match your content |

### File Locations Reference

| File | Purpose | Location |
|------|---------|----------|
| `index.html` | Main landing page | Root folder |
| `privacy.html` | Privacy Policy | Root folder |
| `terms.html` | Terms of Service | Root folder |
| `blog.html` | Blog page (optional) | Root folder |

### Important Code Sections

| Section | Lines | Purpose |
|---------|-------|---------|
| Header/Nav | 25-55 | Navigation menu |
| Hero | 70-125 | Main banner |
| Features | 130-230 | Feature cards |
| Benefits | 235-350 | Benefit cards |
| Testimonials | 355-480 | Customer reviews |
| About | 485-520 | Company information |
| FAQ | 525-660 | Questions & answers |
| CTA | 665-685 | Call to action |
| Footer | 690-760 | Footer content |

---

## Getting Help

### Resources

- **Tailwind CSS Docs**: https://tailwindcss.com/docs
- **HTML Reference**: https://developer.mozilla.org/en-US/docs/Web/HTML
- **CSS Reference**: https://developer.mozilla.org/en-US/docs/Web/CSS
- **Font Awesome Icons**: https://fontawesome.com/

### Common Questions

**Q: Can I change fonts?**
A: Yes, but you'd need to add custom CSS. For now, the page uses the system default font. Contact a developer if you want a custom font.

**Q: Can I add more feature cards?**
A: Yes! Copy the entire feature card `<div>` (from opening to closing tag) and paste it again. Update the text and icon.

**Q: How do I add images?**
A: Create an `images` folder in your project folder, put your image there, then add:
```html
<img src="images/your-image.jpg" alt="Description">
```

**Q: Can I change the layout?**
A: Yes, but it requires understanding CSS and HTML structure. For major layout changes, consider hiring a developer.

**Q: How do I deploy this to the web?**
A: You need web hosting. Popular options: Netlify, Vercel, or traditional hosting like GoDaddy. Each has different instructions.

---

## Conclusion

You now have a complete guide to maintaining and customizing your KC Nails landing page! Remember:

1. **Start small** - Make one change at a time
2. **Test everything** - Check that changes work before moving on
3. **Keep backups** - Always have a backup of your original files
4. **Use the search function** - Ctrl+F is your friend
5. **Don't be afraid to experiment** - You can always undo changes

Good luck with your landing page! If you have questions, refer back to the relevant section of this guide.