# Oakland Accident Care Landing Page - Maintenance & Customization Guide

Welcome! This comprehensive guide will help you maintain and customize your Oakland Accident Care landing page. Whether you're updating text, fixing links, or adding new pages, we'll walk you through each step with clear, beginner-friendly instructions.

---

## Table of Contents

1. [Understanding Your Landing Page Structure](#understanding-your-landing-page-structure)
2. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
3. [Fixing and Managing Links](#fixing-and-managing-links)
4. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
5. [Troubleshooting Common Issues](#troubleshooting-common-issues)
6. [Best Practices for Maintenance](#best-practices-for-maintenance)

---

## Understanding Your Landing Page Structure

Before making changes, let's understand how your landing page is organized:

### File Organization

Your website consists of:
- **index.html** - The main landing page (what you have)
- **privacy.html** - Privacy policy page (needs to be created)
- **terms.html** - Terms of service page (needs to be created)
- **blog.html** - Blog page (needs to be created)

### Page Sections (In Order)

1. **Header & Navigation** - Top menu with logo and links
2. **Hero Section** - Large welcome area with main headline
3. **Features Section** - Three feature cards (Trauma-Sensitive Care, All Liens Accepted, Start Today)
4. **Benefits Section** - Three benefit boxes (Doctor Coordination, Attorney Collaboration, Insurance Management)
5. **About Us Section** - Company information with values
6. **Testimonials Section** - Customer reviews
7. **Call-to-Action Section** - Large promotion area
8. **FAQ Section** - Questions and answers
9. **Footer** - Bottom information and links

### Key Technologies Used

- **HTML** - The structure and content of the page
- **Tailwind CSS** - A utility-first CSS framework for styling (via CDN link)
- **Font Awesome** - Icon library for visual elements
- **Vanilla JavaScript** - For interactive features (mobile menu, FAQ accordion)

---

## Updating Text and Tailwind CSS Classes

### Part 1: Updating Text Content

Text updates are the most common maintenance task. Here's how to do it safely:

#### Step 1: Open Your HTML File

1. Open `index.html` in your code editor (VS Code, Notepad++, Sublime Text, etc.)
2. Use **Ctrl+F** (Windows) or **Cmd+F** (Mac) to search for the text you want to change

#### Step 2: Finding Specific Text Sections

**To update the main headline:**

Find this section (around line 95):
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold tracking-tight mb-6 leading-tight">
    Same-Day Auto Injury Care
    <span class="gradient-accent bg-clip-text text-transparent"> Oakland Doctors Who Speak Your Language</span>
</h1>
```

**Change it to:**
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold tracking-tight mb-6 leading-tight">
    Your New Headline Here
    <span class="gradient-accent bg-clip-text text-transparent"> Your Subheadline Here</span>
</h1>
```

**To update the hero subtitle:**

Find this section (around line 103):
```html
<p class="text-xl md:text-2xl text-gray-300 mb-4 font-light leading-relaxed">
    Your healing comes first — before insurance approval
</p>
```

**Change it to:**
```html
<p class="text-xl md:text-2xl text-gray-300 mb-4 font-light leading-relaxed">
    Your new subtitle text here
</p>
```

#### Step 3: Updating Feature Cards

Each feature card has three parts: icon, title, and description.

**To update the first feature card (Trauma-Sensitive Care):**

Find this section (around line 155):
```html
<h3 class="text-2xl font-bold mb-3">Trauma-Sensitive Care</h3>
<p class="text-gray-300 leading-relaxed mb-4">
    Our physicians understand that auto accidents can cause both physical and emotional trauma. We provide compassionate, patient-centered care that addresses your complete wellness journey.
</p>
```

**Change the title and description:**
```html
<h3 class="text-2xl font-bold mb-3">Your New Feature Title</h3>
<p class="text-gray-300 leading-relaxed mb-4">
    Your new feature description goes here. Keep it clear and benefit-focused.
</p>
```

**To update the bullet points under each feature:**

Find these lines (around line 161):
```html
<ul class="space-y-2 text-gray-400 text-sm">
    <li class="flex items-start gap-2">
        <i class="fas fa-check text-green-400 mt-1"></i>
        <span>Gentle, evidence-based treatment protocols</span>
    </li>
    <li class="flex items-start gap-2">
        <i class="fas fa-check text-green-400 mt-1"></i>
        <span>Trained in PTSD and accident-related anxiety</span>
    </li>
    <li class="flex items-start gap-2">
        <i class="fas fa-check text-green-400 mt-1"></i>
        <span>Holistic recovery approach</span>
    </li>
</ul>
```

**Update each `<span>` text:**
```html
<ul class="space-y-2 text-gray-400 text-sm">
    <li class="flex items-start gap-2">
        <i class="fas fa-check text-green-400 mt-1"></i>
        <span>Your first benefit point</span>
    </li>
    <li class="flex items-start gap-2">
        <i class="fas fa-check text-green-400 mt-1"></i>
        <span>Your second benefit point</span>
    </li>
    <li class="flex items-start gap-2">
        <i class="fas fa-check text-green-400 mt-1"></i>
        <span>Your third benefit point</span>
    </li>
</ul>
```

#### Step 4: Updating Testimonials

Each testimonial has a name, title, star rating, and quote.

**To update the first testimonial:**

Find this section (around line 340):
```html
<div class="testimonial-card bg-gray-800 border border-gray-700 rounded-xl p-8">
    <div class="flex items-center mb-4">
        <div class="flex-1">
            <h3 class="text-xl font-bold">Maria Rodriguez</h3>
            <p class="text-gray-400 text-sm">Marketing Manager, Tech Company</p>
        </div>
    </div>
    <div class="flex gap-1 mb-4">
        <i class="fas fa-star star-rating"></i>
        <i class="fas fa-star star-rating"></i>
        <i class="fas fa-star star-rating"></i>
        <i class="fas fa-star star-rating"></i>
        <i class="fas fa-star star-rating"></i>
    </div>
    <p class="text-gray-300 leading-relaxed">
        "I was terrified after my accident, but Oakland Accident Care made everything easy..."
    </p>
</div>
```

**Change the name, title, and quote:**
```html
<h3 class="text-xl font-bold">Customer Name Here</h3>
<p class="text-gray-400 text-sm">Their Job Title or Description</p>
```

**And update the quote:**
```html
<p class="text-gray-300 leading-relaxed">
    "Your customer's testimonial text goes here. Make it authentic and specific."
</p>
```

#### Step 5: Updating FAQ Questions and Answers

Each FAQ item has a question and answer.

**To update the first FAQ item:**

Find this section (around line 415):
```html
<div class="faq-item bg-gray-800 border border-gray-700 rounded-xl overflow-hidden">
    <button class="faq-question w-full px-8 py-6 flex items-center justify-between hover:bg-gray-700 transition-colors duration-300 cursor-pointer">
        <h3 class="text-lg font-bold text-left">How quickly can I get an appointment?</h3>
        <i class="faq-icon fas fa-chevron-down text-gray-400"></i>
    </button>
    <div class="faq-answer hidden px-8 pb-6">
        <p class="text-gray-300 leading-relaxed">
            We understand that time is critical after an auto accident...
        </p>
    </div>
</div>
```

**Update the question:**
```html
<h3 class="text-lg font-bold text-left">Your new question here?</h3>
```

**Update the answer:**
```html
<p class="text-gray-300 leading-relaxed">
    Your answer text goes here. Be clear and comprehensive.
</p>
```

#### Step 6: Updating Footer Information

**To update the footer company description:**

Find this section (around line 520):
```html
<p class="text-gray-400 leading-relaxed mb-6">
    Providing compassionate, same-day auto injury care with trauma-sensitive physicians who understand your complete recovery journey.
</p>
```

**Change it to:**
```html
<p class="text-gray-400 leading-relaxed mb-6">
    Your company description here. Keep it concise and professional.
</p>
```

**To update contact information in the footer:**

Find this section (around line 560):
```html
<a href="mailto:frontdesk@oaklandaccidentcare.com" class="text-white hover:text-purple-400 transition-colors duration-300">frontdesk@oaklandaccidentcare.com</a>
```

**Change the email:**
```html
<a href="mailto:your-email@yourdomain.com" class="text-white hover:text-purple-400 transition-colors duration-300">your-email@yourdomain.com</a>
```

**To update the phone number:**

Find this section (around line 568):
```html
<p class="text-white">(510) 555-0147</p>
```

**Change it to:**
```html
<p class="text-white">(YOUR) PHONE-NUMBER</p>
```

**To update the copyright year:**

Find this section (around line 582):
```html
&copy; 2025 Oakland Accident Care. All rights reserved. Compassionate care for your recovery.
```

**Change it to:**
```html
&copy; 2025 Your Company Name. All rights reserved. Your tagline here.
```

---

### Part 2: Understanding and Modifying Tailwind CSS Classes

Tailwind CSS uses utility classes to style elements. Here's how to understand and modify them:

#### What Are Tailwind Classes?

Tailwind classes are short names that apply specific styles. For example:
- `text-white` = white text color
- `bg-gray-900` = dark gray background
- `px-4` = padding on left and right
- `py-6` = padding on top and bottom
- `rounded-xl` = rounded corners

#### Common Tailwind Classes Used in Your Page

| Class | What It Does | Example |
|-------|-------------|---------|
| `text-white` | Makes text white | `<p class="text-white">` |
| `text-gray-300` | Makes text light gray | `<p class="text-gray-300">` |
| `bg-gray-900` | Dark gray background | `<div class="bg-gray-900">` |
| `bg-gray-800` | Medium-dark gray background | `<div class="bg-gray-800">` |
| `px-4` | Horizontal padding (left & right) | `<div class="px-4">` |
| `py-6` | Vertical padding (top & bottom) | `<div class="py-6">` |
| `mb-6` | Margin bottom (space below) | `<div class="mb-6">` |
| `mt-4` | Margin top (space above) | `<div class="mt-4">` |
| `rounded-xl` | Rounded corners | `<div class="rounded-xl">` |
| `font-bold` | Bold text | `<h1 class="font-bold">` |
| `text-2xl` | Large text | `<p class="text-2xl">` |
| `flex` | Flexbox layout | `<div class="flex">` |
| `gap-4` | Space between flex items | `<div class="flex gap-4">` |

#### Responsive Design Classes

Your page uses responsive classes that change appearance on different screen sizes:
- `md:` = applies on medium screens and larger (tablets)
- `lg:` = applies on large screens and larger (desktops)

**Example:**
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl">
```

This means:
- On mobile: text size 4xl
- On tablets (md): text size 5xl
- On desktops (lg): text size 6xl

#### Modifying Colors

**To change text color:**

Find a text element and change the color class:
```html
<!-- Original -->
<p class="text-gray-300">Your text here</p>

<!-- Change to purple -->
<p class="text-purple-400">Your text here</p>

<!-- Change to green -->
<p class="text-green-400">Your text here</p>
```

**Available color options:**
- `text-white` (brightest)
- `text-gray-100` through `text-gray-900` (lighter to darker)
- `text-purple-400`, `text-purple-500`, `text-purple-600` (various purples)
- `text-green-400` (green)
- `text-blue-400` (blue)
- `text-red-400` (red)

**To change background color:**

```html
<!-- Original -->
<div class="bg-gray-800">Content</div>

<!-- Change to darker -->
<div class="bg-gray-900">Content</div>

<!-- Change to lighter -->
<div class="bg-gray-700">Content</div>
```

#### Modifying Spacing

**To add more space below an element:**

```html
<!-- Original - small margin -->
<h2 class="text-4xl mb-4">Title</h2>

<!-- Add more space below -->
<h2 class="text-4xl mb-8">Title</h2>

<!-- Even more space -->
<h2 class="text-4xl mb-12">Title</h2>
```

Spacing numbers: `mb-2`, `mb-4`, `mb-6`, `mb-8`, `mb-10`, `mb-12`, `mb-16`

**To add padding inside a card:**

```html
<!-- Original -->
<div class="bg-gray-800 p-8">Content</div>

<!-- Add more padding -->
<div class="bg-gray-800 p-12">Content</div>

<!-- Add less padding -->
<div class="bg-gray-800 p-6">Content</div>
```

#### Modifying Text Size

**To change heading size:**

```html
<!-- Original -->
<h2 class="text-3xl md:text-4xl lg:text-5xl">Title</h2>

<!-- Make it smaller -->
<h2 class="text-2xl md:text-3xl lg:text-4xl">Title</h2>

<!-- Make it larger -->
<h2 class="text-4xl md:text-5xl lg:text-6xl">Title</h2>
```

Size options: `text-xl`, `text-2xl`, `text-3xl`, `text-4xl`, `text-5xl`, `text-6xl`

#### Modifying Border Styles

**To change border color:**

```html
<!-- Original - gray border -->
<div class="border border-gray-700">Content</div>

<!-- Change to purple -->
<div class="border border-purple-500">Content</div>

<!-- Change to green -->
<div class="border border-green-400">Content</div>
```

**To change border thickness:**

```html
<!-- Thin border -->
<div class="border border-gray-700">Content</div>

<!-- Thicker border -->
<div class="border-2 border-gray-700">Content</div>

<!-- Very thick border -->
<div class="border-4 border-gray-700">Content</div>
```

#### Modifying Rounded Corners

```html
<!-- Slightly rounded -->
<div class="rounded">Content</div>

<!-- More rounded -->
<div class="rounded-lg">Content</div>

<!-- Very rounded -->
<div class="rounded-xl">Content</div>

<!-- Completely round (for circles) -->
<div class="rounded-full">Content</div>
```

#### Practical Example: Modifying a Feature Card

**Original feature card:**
```html
<div class="card-hover bg-gray-800 border border-gray-700 rounded-xl p-8 hover:border-purple-500">
    <div class="w-16 h-16 gradient-accent rounded-lg flex items-center justify-center mb-6">
        <i class="fas fa-hands-praying feature-icon text-white text-2xl"></i>
    </div>
    <h3 class="text-2xl font-bold mb-3">Trauma-Sensitive Care</h3>
    <p class="text-gray-300 leading-relaxed mb-4">Our physicians understand...</p>
</div>
```

**Let's say you want to:**
1. Make the background slightly lighter
2. Add more padding
3. Make the text larger
4. Change the border color to green

**Modified version:**
```html
<div class="card-hover bg-gray-700 border border-green-400 rounded-xl p-12 hover:border-green-300">
    <div class="w-16 h-16 gradient-accent rounded-lg flex items-center justify-center mb-6">
        <i class="fas fa-hands-praying feature-icon text-white text-2xl"></i>
    </div>
    <h3 class="text-3xl font-bold mb-3">Trauma-Sensitive Care</h3>
    <p class="text-gray-200 leading-relaxed mb-4">Our physicians understand...</p>
</div>
```

**What changed:**
- `bg-gray-800` → `bg-gray-700` (lighter background)
- `p-8` → `p-12` (more padding)
- `text-2xl` → `text-3xl` (larger title)
- `text-gray-300` → `text-gray-200` (lighter text)
- `border-gray-700` → `border-green-400` (green border)
- `hover:border-purple-500` → `hover:border-green-300` (green hover effect)

#### Custom Gradient Classes

Your page uses custom gradient classes defined in the `<style>` section. These are already created for you:

- `.gradient-accent` - Purple to pink gradient (main brand color)
- `.gradient-accent-subtle` - Lighter version of the gradient
- `.hero-gradient` - Dark gradient for hero section

**To use the gradient on a button:**
```html
<button class="gradient-accent text-white px-6 py-3 rounded-lg">
    Click Me
</button>
```

---

## Fixing and Managing Links

Links are crucial for navigation. Let's learn how to identify and fix them.

### Part 1: Understanding Link Types

Your page has three types of links:

1. **Internal Links** - Links to sections on the same page
2. **External Links** - Links to other websites
3. **Email Links** - Links that open email client
4. **File Links** - Links to other pages on your website

### Part 2: Finding All Links in Your Page

**In the Header Navigation:**

Find this section (around line 40):
```html
<div class="hidden md:flex items-center space-x-1">
    <a href="#features" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">Features</a>
    <a href="#benefits" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">Benefits</a>
    <a href="#about" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">About</a>
    <a href="#testimonials" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">Testimonials</a>
    <a href="#faq" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">FAQ</a>
</div>
```

These are **internal links** that point to sections on the same page.

**In the Mobile Menu:**

Find this section (around line 58):
```html
<div class="mobile-menu hidden md:hidden pb-4 space-y-2 border-t border-gray-800 mt-4">
    <a href="#features" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">Features</a>
    <a href="#benefits" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">Benefits</a>
    <!-- More links... -->
</div>
```

These mirror the desktop navigation.

**Book Now Buttons:**

Find these sections (around line 51 and 66):
```html
<a href="https://app.acuityscheduling.com/schedule/99abdf40" target="_blank" rel="noopener noreferrer" class="hidden md:inline-block btn-primary text-white px-6 py-2 rounded-lg font-semibold">
    Book Now
</a>
```

This is an **external link** to a scheduling system.

**In the Footer:**

Find this section (around line 540):
```html
<li><a href="#features" class="text-gray-400 hover:text-white transition-colors duration-300">Features</a></li>
<li><a href="#benefits" class="text-gray-400 hover:text-white transition-colors duration-300">Benefits</a></li>
<li><a href="#about" class="text-gray-400 hover:text-white transition-colors duration-300">About Us</a></li>
<li><a href="#testimonials" class="text-gray-400 hover:text-white transition-colors duration-300">Testimonials</a></li>
<li><a href="#faq" class="text-gray-400 hover:text-white transition-colors duration-300">FAQ</a></li>
```

These are also **internal links**.

**Email Link in Footer:**

Find this section (around line 565):
```html
<a href="mailto:frontdesk@oaklandaccidentcare.com" class="text-white hover:text-purple-400 transition-colors duration-300">frontdesk@oaklandaccidentcare.com</a>
```

This is an **email link**.

**Policy Links in Footer:**

Find this section (around line 548):
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
<li><a href="blog.html" class="text-gray-400 hover:text-white transition-colors duration-300">Blog</a></li>
```

These are **file links** to other pages.

### Part 3: Fixing Broken Links - Step by Step

#### Fixing the Scheduling Link

The scheduling link currently points to Acuity Scheduling. If you use a different service:

**Step 1:** Find all instances of the Acuity link. Search for:
```
https://app.acuityscheduling.com/schedule/99abdf40
```

**Step 2:** Replace with your scheduling service URL:

```html
<!-- Original -->
<a href="https://app.acuityscheduling.com/schedule/99abdf40" target="_blank" rel="noopener noreferrer">

<!-- If using Calendly -->
<a href="https://calendly.com/yourusername" target="_blank" rel="noopener noreferrer">

<!-- If using another service -->
<a href="https://your-scheduling-service.com/your-link" target="_blank" rel="noopener noreferrer">
```

**Important:** You'll find this link in 4 places:
1. Line ~51 (Desktop header button)
2. Line ~66 (Mobile menu button)
3. Line ~107 (Hero section main CTA)
4. Line ~112 (Hero section secondary button)
5. Line ~378 (CTA section button)

**Replace all 5 instances** to ensure consistency.

#### Fixing the Email Link

**To change the contact email:**

**Step 1:** Search for:
```
frontdesk@oaklandaccidentcare.com
```

**Step 2:** Replace with your email address:

```html
<!-- Original -->
<a href="mailto:frontdesk@oaklandaccidentcare.com">frontdesk@oaklandaccidentcare.com</a>

<!-- New -->
<a href="mailto:your-email@yourdomain.com">your-email@yourdomain.com</a>
```

**You'll find this in 3 places:**
1. Line ~565 (Footer contact section)
2. Line ~473 (FAQ contact section)
3. Line ~490 (FAQ contact section - text content)

**Replace all 3 instances.**

#### Fixing Social Media Links

**Step 1:** Find the social media links in the footer (around line 580):

```html
<a href="#" aria-label="Facebook" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-purple-600 transition-colors duration-300">
    <i class="fab fa-facebook-f text-white"></i>
</a>
<a href="#" aria-label="Twitter" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-purple-600 transition-colors duration-300">
    <i class="fab fa-twitter text-white"></i>
</a>
<a href="#" aria-label="Instagram" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-purple-600 transition-colors duration-300">
    <i class="fab fa-instagram text-white"></i>
</a>
<a href="#" aria-label="LinkedIn" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-purple-600 transition-colors duration-300">
    <i class="fab fa-linkedin-in text-white"></i>
</a>
```

**Step 2:** Replace each `href="#"` with your actual social media URL:

```html
<!-- Facebook -->
<a href="https://facebook.com/yourpage" aria-label="Facebook" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-purple-600 transition-colors duration-300">
    <i class="fab fa-facebook-f text-white"></i>
</a>

<!-- Twitter -->
<a href="https://twitter.com/yourhandle" aria-label="Twitter" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-purple-600 transition-colors duration-300">
    <i class="fab fa-twitter text-white"></i>
</a>

<!-- Instagram -->
<a href="https://instagram.com/yourprofile" aria-label="Instagram" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-purple-600 transition-colors duration-300">
    <i class="fab fa-instagram text-white"></i>
</a>

<!-- LinkedIn -->
<a href="https://linkedin.com/company/yourcompany" aria-label="LinkedIn" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-purple-600 transition-colors duration-300">
    <i class="fab fa-linkedin-in text-white"></i>
</a>
```

**Tip:** If you don't have a social media account, you can either:
- Remove the link entirely
- Keep `href="#"` (it won't go anywhere)
- Change it to your website homepage

#### Fixing Service Links in Footer

**Step 1:** Find the service links (around line 554):

```html
<li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Medical Evaluation</a></li>
<li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Pain Management</a></li>
<li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Physical Therapy</a></li>
<li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Trauma Counseling</a></li>
<li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Legal Support</a></li>
```

**Step 2:** If you have service detail pages, update the links:

```html
<li><a href="services/medical-evaluation.html" class="text-gray-400 hover:text-white transition-colors duration-300">Medical Evaluation</a></li>
<li><a href="services/pain-management.html" class="text-gray-400 hover:text-white transition-colors duration-300">Pain Management</a></li>
<li><a href="services/physical-therapy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Physical Therapy</a></li>
<li><a href="services/trauma-counseling.html" class="text-gray-400 hover:text-white transition-colors duration-300">Trauma Counseling</a></li>
<li><a href="services/legal-support.html" class="text-gray-400 hover:text-white transition-colors duration-300">Legal Support</a></li>
```

**Or if you don't have these pages yet**, leave them as `href="#"` for now.

### Part 4: Link Best Practices

#### Understanding Link Attributes

Each link has important attributes:

```html
<a href="https://example.com" target="_blank" rel="noopener noreferrer" class="text-white">
    Link Text
</a>
```

- `href` - The destination URL
- `target="_blank"` - Opens link in new tab (use for external links)
- `rel="noopener noreferrer"` - Security attribute for external links (always include with `target="_blank"`)
- `class` - Styling classes

#### When to Use `target="_blank"`

**Use `target="_blank"` for:**
- External websites (like scheduling services)
- Social media links
- Third-party services

**Don't use for:**
- Internal navigation links (links to sections on same page)
- Links to your own pages

**Example:**
```html
<!-- External link - use target="_blank" -->
<a href="https://app.acuityscheduling.com/schedule/99abdf40" target="_blank" rel="noopener noreferrer">
    Book Now
</a>

<!-- Internal link - don't use target="_blank" -->
<a href="#features">
    Features
</a>

<!-- Link to another page on your site - don't use target="_blank" -->
<a href="privacy.html">
    Privacy Policy
</a>
```

---

## Linking Privacy and Terms Pages

Now let's create and link your privacy and terms pages.

### Part 1: Understanding What You Need

You need to create three new HTML files:
1. **privacy.html** - Privacy Policy page
2. **terms.html** - Terms of Service page
3. **blog.html** - Blog page (optional)

### Part 2: Creating the Privacy Policy Page

**Step 1:** Create a new file called `privacy.html` in the same folder as your `index.html`

**Step 2:** Copy this template and save it as `privacy.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Privacy Policy for Oakland Accident Care">
    <title>Privacy Policy - Oakland Accident Care</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        html {
            scroll-behavior: smooth;
        }
        .gradient-accent {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
    </style>
</head>
<body class="bg-gray-900 text-white">
    <!-- Header & Navigation -->
    <header class="sticky top-0 z-50 bg-gray-900 bg-opacity-95 backdrop-blur-md border-b border-gray-800">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center py-4">
                <!-- Logo -->
                <div class="flex items-center space-x-2">
                    <div class="w-10 h-10 gradient-accent rounded-lg flex items-center justify-center">
                        <i class="fas fa-heart text-white text-lg"></i>
                    </div>
                    <a href="index.html" class="text-xl font-bold text-white">Oakland Care</a>
                </div>

                <!-- Desktop Menu -->
                <div class="hidden md:flex items-center space-x-1">
                    <a href="index.html#features" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">Features</a>
                    <a href="index.html#benefits" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">Benefits</a>
                    <a href="index.html#about" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">About</a>
                    <a href="index.html#testimonials" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">Testimonials</a>
                    <a href="index.html#faq" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">FAQ</a>
                </div>

                <!-- CTA & Mobile Menu Button -->
                <div class="flex items-center space-x-4">
                    <a href="https://app.acuityscheduling.com/schedule/99abdf40" target="_blank" rel="noopener noreferrer" class="hidden md:inline-block gradient-accent text-white px-6 py-2 rounded-lg font-semibold">
                        Book Now
                    </a>
                    <button class="mobile-menu-button md:hidden text-white p-2 hover:bg-gray-800 rounded-lg transition-colors duration-300">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                </div>
            </div>

            <!-- Mobile Menu -->
            <div class="mobile-menu hidden md:hidden pb-4 space-y-2 border-t border-gray-800 mt-4">
                <a href="index.html#features" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">Features</a>
                <a href="index.html#benefits" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">Benefits</a>
                <a href="index.html#about" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">About</a>
                <a href="index.html#testimonials" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">Testimonials</a>
                <a href="index.html#faq" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">FAQ</a>
                <a href="https://app.acuityscheduling.com/schedule/99abdf40" target="_blank" rel="noopener noreferrer" class="block gradient-accent text-white px-4 py-2 rounded-lg font-semibold text-center">
                    Book Now
                </a>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <main class="py-16 md:py-24 bg-gray-900">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-4xl md:text-5xl font-bold mb-8">Privacy Policy</h1>
            
            <div class="prose prose-invert max-w-none space-y-6 text-gray-300">
                <section>
                    <h2 class="text-2xl font-bold text-white mb-4">1. Introduction</h2>
                    <p>
                        Oakland Accident Care ("we," "our," or "us") is committed to protecting your privacy. This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you visit our website.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mb-4">2. Information We Collect</h2>
                    <p>
                        We may collect information about you in a variety of ways. The information we may collect on the site includes:
                    </p>
                    <ul class="list-disc pl-6 space-y-2">
                        <li>Personal Information: Name, email address, phone number, and other contact details you voluntarily provide.</li>
                        <li>Medical Information: Information related to your auto injury and medical history, collected during appointments.</li>
                        <li>Usage Data: Information about how you interact with our website, including IP address, browser type, and pages visited.</li>
                    </ul>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mb-4">3. Use of Your Information</h2>
                    <p>
                        Having accurate information about you permits us to provide you with a smooth, efficient, and customized experience. Specifically, we may use information collected about you via the site to:
                    </p>
                    <ul class="list-disc pl-6 space-y-2">
                        <li>Generate a personal profile about you so that future visits to our site are personalized.</li>
                        <li>Increase the efficiency and operation of our site.</li>
                        <li>Monitor and analyze usage and trends to improve your experience with the site.</li>
                        <li>Notify you of updates to our site.</li>
                        <li>Offer new products, services, and/or recommendations to you.</li>
                    </ul>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mb-4">4. Disclosure of Your Information</h2>
                    <p>
                        We may share your information in the following situations:
                    </p>
                    <ul class="list-disc pl-6 space-y-2">
                        <li>With healthcare providers as necessary for your treatment.</li>
                        <li>With insurance companies and legal representatives as authorized by you.</li>
                        <li>With service providers who assist us in operating our website and conducting our business.</li>
                        <li>When required by law or to protect our legal rights.</li>
                    </ul>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mb-4">5. Security of Your Information</h2>
                    <p>
                        We use administrative, technical, and physical security measures to protect your personal information. However, no method of transmission over the Internet is 100% secure.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mb-4">6. Contact Us</h2>
                    <p>
                        If you have questions or comments about this Privacy Policy, please contact us at:
                    </p>
                    <p>
                        Email: <a href="mailto:frontdesk@oaklandaccidentcare.com" class="text-purple-400 hover:text-purple-300">frontdesk@oaklandaccidentcare.com</a><br>
                        Phone: (510) 555-0147
                    </p>
                </section>

                <section>
                    <p class="text-gray-400 text-sm">
                        Last Updated: January 2025
                    </p>
                </section>
            </div>

            <!-- Back to Home Link -->
            <div class="mt-12">
                <a href="index.html" class="gradient-accent text-white px-6 py-3 rounded-lg font-semibold inline-block">
                    <i class="fas fa-arrow-left mr-2"></i>
                    Back to Home
                </a>
            </div>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-950 border-t border-gray-800 py-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="border-t border-gray-800 pt-8">
                <div class="flex flex-col md:flex-row justify-between items-center gap-4">
                    <p class="text-gray-400 text-sm">
                        &copy; 2025 Oakland Accident Care. All rights reserved.
                    </p>
                    <div class="flex gap-6 text-sm">
                        <a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy</a>
                        <a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms</a>
                    </div>
                </div>
            </div>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const mobileMenuButton = document.querySelector('header nav .mobile-menu-button');
            const mobileMenu = document.querySelector('header nav .mobile-menu');
            
            if (mobileMenuButton && mobileMenu) {
                mobileMenuButton.addEventListener('click', () => {
                    mobileMenu.classList.toggle('hidden');
                    const icon = mobileMenuButton.querySelector('i');
                    if (icon) {
                        icon.classList.toggle('fa-bars');
                        icon.classList.toggle('fa-times');
                    }
                });

                const mobileMenuLinks = mobileMenu.querySelectorAll('a');
                mobileMenuLinks.forEach(link => {
                    link.addEventListener('click', () => {
                        mobileMenu.classList.add('hidden');
                        const icon = mobileMenuButton.querySelector('i');
                        if (icon) {
                            icon.classList.remove('fa-times');
                            icon.classList.add('fa-bars');
                        }
                    });
                });
            }
        });
    </script>
</body>
</html>
```

### Part 3: Creating the Terms of Service Page

**Step 1:** Create a new file called `terms.html` in the same folder

**Step 2:** Copy this template and save it as `terms.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Terms of Service for Oakland Accident Care">
    <title>Terms of Service - Oakland Accident Care</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        html {
            scroll-behavior: smooth;
        }
        .gradient-accent {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
    </style>
</head>
<body class="bg-gray-900 text-white">
    <!-- Header & Navigation -->
    <header class="sticky top-0 z-50 bg-gray-900 bg-opacity-95 backdrop-blur-md border-b border-gray-800">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center py-4">
                <!-- Logo -->
                <div class="flex items-center space-x-2">
                    <div class="w-10 h-10 gradient-accent rounded-lg flex items-center justify-center">
                        <i class="fas fa-heart text-white text-lg"></i>
                    </div>
                    <a href="index.html" class="text-xl font-bold text-white">Oakland Care</a>
                </div>

                <!-- Desktop Menu -->
                <div class="hidden md:flex items-center space-x-1">
                    <a href="index.html#features" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">Features</a>
                    <a href="index.html#benefits" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">Benefits</a>
                    <a href="index.html#about" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">About</a>
                    <a href="index.html#testimonials" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">Testimonials</a>
                    <a href="index.html#faq" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">FAQ</a>
                </div>

                <!-- CTA & Mobile Menu Button -->
                <div class="flex items-center space-x-4">
                    <a href="https://app.acuityscheduling.com/schedule/99abdf40" target="_blank" rel="noopener noreferrer" class="hidden md:inline-block gradient-accent text-white px-6 py-2 rounded-lg font-semibold">
                        Book Now
                    </a>
                    <button class="mobile-menu-button md:hidden text-white p-2 hover:bg-gray-800 rounded-lg transition-colors duration-300">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                </div>
            </div>

            <!-- Mobile Menu -->
            <div class="mobile-menu hidden md:hidden pb-4 space-y-2 border-t border-gray-800 mt-4">
                <a href="index.html#features" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">Features</a>
                <a href="index.html#benefits" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">Benefits</a>
                <a href="index.html#about" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">About</a>
                <a href="index.html#testimonials" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">Testimonials</a>
                <a href="index.html#faq" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">FAQ</a>
                <a href="https://app.acuityscheduling.com/schedule/99abdf40" target="_blank" rel="noopener noreferrer" class="block gradient-accent text-white px-4 py-2 rounded-lg font-semibold text-center">
                    Book Now
                </a>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <main class="py-16 md:py-24 bg-gray-900">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-4xl md:text-5xl font-bold mb-8">Terms of Service</h1>
            
            <div class="prose prose-invert max-w-none space-y-6 text-gray-300">
                <section>
                    <h2 class="text-2xl font-bold text-white mb-4">1. Agreement to Terms</h2>
                    <p>
                        By accessing and using this website, you accept and agree to be bound by the terms and provision of this agreement. If you do not agree to abide by the above, please do not use this service.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mb-4">2. Use License</h2>
                    <p>
                        Permission is granted to temporarily download one copy of the materials (information or software) on Oakland Accident Care's website for personal, non-commercial transitory viewing only. This is the grant of a license, not a transfer of title, and under this license you may not:
                    </p>
                    <ul class="list-disc pl-6 space-y-2">
                        <li>Modifying or copying the materials</li>
                        <li>Using the materials for any commercial purpose or for any public display</li>
                        <li>Attempting to decompile or reverse engineer any software contained on the website</li>
                        <li>Removing any copyright or other proprietary notations from the materials</li>
                        <li>Transferring the materials to another person or "mirroring" the materials on any other server</li>
                    </ul>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mb-4">3. Disclaimer</h2>
                    <p>
                        The materials on Oakland Accident Care's website are provided on an 'as is' basis. Oakland Accident Care makes no warranties, expressed or implied, and hereby disclaims and negates all other warranties including, without limitation, implied warranties or conditions of merchantability, fitness for a particular purpose, or non-infringement of intellectual property or other violation of rights.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mb-4">4. Limitations</h2>
                    <p>
                        In no event shall Oakland Accident Care or its suppliers be liable for any damages (including, without limitation, damages for loss of data or profit, or due to business interruption) arising out of the use or inability to use the materials on the website.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mb-4">5. Accuracy of Materials</h2>
                    <p>
                        The materials appearing on Oakland Accident Care's website could include technical, typographical, or photographic errors. Oakland Accident Care does not warrant that any of the materials on our website are accurate, complete, or current. We may make changes to the materials contained on our website at any time without notice.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mb-4">6. Links</h2>
                    <p>
                        Oakland Accident Care has not reviewed all of the sites linked to our website and is not responsible for the contents of any such linked site. The inclusion of any link does not imply endorsement by Oakland Accident Care of the site. Use of any such linked website is at the user's own risk.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mb-4">7. Modifications</h2>
                    <p>
                        Oakland Accident Care may revise these terms of service for our website at any time without notice. By using this website, you are agreeing to be bound by the then current version of these terms of service.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mb-4">8. Governing Law</h2>
                    <p>
                        These terms and conditions are governed by and construed in accordance with the laws of the State of California, and you irrevocably submit to the exclusive jurisdiction of the courts in that location.
                    </p>
                </section>

                <section>
                    <h2 class="text-2xl font-bold text-white mb-4">9. Contact Information</h2>
                    <p>
                        If you have any questions about these Terms of Service, please contact us at:
                    </p>
                    <p>
                        Email: <a href="mailto:frontdesk@oaklandaccidentcare.com" class="text-purple-400 hover:text-purple-300">frontdesk@oaklandaccidentcare.com</a><br>
                        Phone: (510) 555-0147
                    </p>
                </section>

                <section>
                    <p class="text-gray-400 text-sm">
                        Last Updated: January 2025
                    </p>
                </section>
            </div>

            <!-- Back to Home Link -->
            <div class="mt-12">
                <a href="index.html" class="gradient-accent text-white px-6 py-3 rounded-lg font-semibold inline-block">
                    <i class="fas fa-arrow-left mr-2"></i>
                    Back to Home
                </a>
            </div>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-950 border-t border-gray-800 py-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="border-t border-gray-800 pt-8">
                <div class="flex flex-col md:flex-row justify-between items-center gap-4">
                    <p class="text-gray-400 text-sm">
                        &copy; 2025 Oakland Accident Care. All rights reserved.
                    </p>
                    <div class="flex gap-6 text-sm">
                        <a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy</a>
                        <a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms</a>
                    </div>
                </div>
            </div>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const mobileMenuButton = document.querySelector('header nav .mobile-menu-button');
            const mobileMenu = document.querySelector('header nav .mobile-menu');
            
            if (mobileMenuButton && mobileMenu) {
                mobileMenuButton.addEventListener('click', () => {
                    mobileMenu.classList.toggle('hidden');
                    const icon = mobileMenuButton.querySelector('i');
                    if (icon) {
                        icon.classList.toggle('fa-bars');
                        icon.classList.toggle('fa-times');
                    }
                });

                const mobileMenuLinks = mobileMenu.querySelectorAll('a');
                mobileMenuLinks.forEach(link => {
                    link.addEventListener('click', () => {
                        mobileMenu.classList.add('hidden');
                        const icon = mobileMenuButton.querySelector('i');
                        if (icon) {
                            icon.classList.remove('fa-times');
                            icon.classList.add('fa-bars');
                        }
                    });
                });
            }
        });
    </script>
</body>
</html>
```

### Part 4: Verifying Links in Your Main Page

Now that you've created the privacy and terms pages, verify that your `index.html` links to them correctly.

**Step 1:** In your `index.html`, find the footer section (around line 548) and confirm it looks like this:

```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
<li><a href="blog.html" class="text-gray-400 hover:text-white transition-colors duration-300">Blog</a></li>
```

**Good news:** These links are already in your code! No changes needed here.

**Step 2:** Also check the footer bottom section (around line 587):

```html
<a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy</a>
<a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms</a>
<a href="blog.html" class="text-gray-400 hover:text-white transition-colors duration-300">Blog</a>
```

**These links are also already in place!**

### Part 5: Testing Your Links

**To test your links:**

1. Save all three files (`index.html`, `privacy.html`, `terms.html`) in the same folder
2. Open `index.html` in your web browser
3. Scroll to the footer
4. Click on "Privacy Policy" - it should take you to the privacy page
5. Click on "Privacy" (or "Terms") link to go back
6. Click on "Terms of Service" - it should take you to the terms page
7. Use the "Back to Home" button to return to the main page

### Part 6: Creating a Blog Page (Optional)

If you want to create a blog page, follow the same pattern:

**Step 1:** Create a new file called `blog.html`

**Step 2:** Use this template:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Blog - Oakland Accident Care">
    <title>Blog - Oakland Accident Care</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        html {
            scroll-behavior: smooth;
        }
        .gradient-accent {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
    </style>
</head>
<body class="bg-gray-900 text-white">
    <!-- Header & Navigation (same as privacy.html) -->
    <header class="sticky top-0 z-50 bg-gray-900 bg-opacity-95 backdrop-blur-md border-b border-gray-800">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center py-4">
                <div class="flex items-center space-x-2">
                    <div class="w-10 h-10 gradient-accent rounded-lg flex items-center justify-center">
                        <i class="fas fa-heart text-white text-lg"></i>
                    </div>
                    <a href="index.html" class="text-xl font-bold text-white">Oakland Care</a>
                </div>

                <div class="hidden md:flex items-center space-x-1">
                    <a href="index.html#features" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">Features</a>
                    <a href="index.html#benefits" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">Benefits</a>
                    <a href="index.html#about" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">About</a>
                    <a href="index.html#testimonials" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">Testimonials</a>
                    <a href="index.html#faq" class="px-4 py-2 text-gray-300 hover:text-white transition-colors duration-300 font-medium">FAQ</a>
                </div>

                <div class="flex items-center space-x-4">
                    <a href="https://app.acuityscheduling.com/schedule/99abdf40" target="_blank" rel="noopener noreferrer" class="hidden md:inline-block gradient-accent text-white px-6 py-2 rounded-lg font-semibold">
                        Book Now
                    </a>
                    <button class="mobile-menu-button md:hidden text-white p-2 hover:bg-gray-800 rounded-lg transition-colors duration-300">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                </div>
            </div>

            <div class="mobile-menu hidden md:hidden pb-4 space-y-2 border-t border-gray-800 mt-4">
                <a href="index.html#features" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">Features</a>
                <a href="index.html#benefits" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">Benefits</a>
                <a href="index.html#about" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">About</a>
                <a href="index.html#testimonials" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">Testimonials</a>
                <a href="index.html#faq" class="block px-4 py-2 text-gray-300 hover:text-white hover:bg-gray-800 rounded-lg transition-all duration-300">FAQ</a>
                <a href="https://app.acuityscheduling.com/schedule/99abdf40" target="_blank" rel="noopener noreferrer" class="block gradient-accent text-white px-4 py-2 rounded-lg font-semibold text-center">
                    Book Now
                </a>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <main class="py-16 md:py-24 bg-gray-900">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-4xl md:text-5xl font-bold mb-8">Blog</h1>
            
            <div class="space-y-12">
                <!-- Blog Post 1 -->
                <article class="bg-gray-800 border border-gray-700 rounded-xl p-8">
                    <h2 class="text-3xl font-bold mb-3">Your First Blog Post Title</h2>
                    <div class="flex items-center gap-4 text-gray-400 text-sm mb-6">
                        <span><i class="fas fa-calendar mr-2"></i>January 15, 2025</span>
                        <span><i class="fas fa-user mr-2"></i>By Admin</span>
                    </div>
                    <p class="text-gray-300 leading-relaxed mb-4">
                        Your blog post content goes here. This is where you can share valuable information with your patients about auto injury recovery, treatment options, and wellness tips.
                    </p>
                    <a href="#" class="gradient-accent text-white px-4 py-2 rounded-lg font-semibold inline-block">
                        Read More <i class="fas fa-arrow-right ml-2"></i>
                    </a>
                </article>

                <!-- Blog Post 2 -->
                <article class="bg-gray-800 border border-gray-700 rounded-xl p-8">
                    <h2 class="text-3xl font-bold mb-3">Your Second Blog Post Title</h2>
                    <div class="flex items-center gap-4 text-gray-400 text-sm mb-6">
                        <span><i class="fas fa-calendar mr-2"></i>January 10, 2025</span>
                        <span><i class="fas fa-user mr-2"></i>By Admin</span>
                    </div>
                    <p class="text-gray-300 leading-relaxed mb-4">
                        Add more blog posts here to share your expertise with patients and improve your search engine visibility.
                    </p>
                    <a href="#" class="gradient-accent text-white px-4 py-2 rounded-lg font-semibold inline-block">
                        Read More <i class="fas fa-arrow-right ml-2"></i>
                    </a>
                </article>
            </div>

            <!-- Back to Home Link -->
            <div class="mt-12">
                <a href="index.html" class="gradient-accent text-white px-6 py-3 rounded-lg font-semibold inline-block">
                    <i class="fas fa-arrow-left mr-2"></i>
                    Back to Home
                </a>
            </div>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-950 border-t border-gray-800 py-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="border-t border-gray-800 pt-8">
                <div class="flex flex-col md:flex-row justify-between items-center gap-4">
                    <p class="text-gray-400 text-sm">
                        &copy; 2025 Oakland Accident Care. All rights reserved.
                    </p>
                    <div class="flex gap-6 text-sm">
                        <a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy</a>
                        <a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms</a>
                        <a href="blog.html" class="text-gray-400 hover:text-white transition-colors duration-300">Blog</a>
                    </div>
                </div>
            </div>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const mobileMenuButton = document.querySelector('header nav .mobile-menu-button');
            const mobileMenu = document.querySelector('header nav .mobile-menu');
            
            if (mobileMenuButton && mobileMenu) {
                mobileMenuButton.addEventListener('click', () => {
                    mobileMenu.classList.toggle('hidden');
                    const icon = mobileMenuButton.querySelector('i');
                    if (icon) {
                        icon.classList.toggle('fa-bars');
                        icon.classList.toggle('fa-times');
                    }
                });

                const mobileMenuLinks = mobileMenu.querySelectorAll('a');
                mobileMenuLinks.forEach(link => {
                    link.addEventListener('click', () => {
                        mobileMenu.classList.add('hidden');
                        const icon = mobileMenuButton.querySelector('i');
                        if (icon) {
                            icon.classList.remove('fa-times');
                            icon.classList.add('fa-bars');
                        }
                    });
                });
            }
        });
    </script>
</body>
</html>
```

---

## Troubleshooting Common Issues

### Issue 1: Links Not Working

**Problem:** Clicking a link doesn't take you anywhere

**Solution:**
1. Check the `href` attribute spelling - it must match the filename exactly
2. Make sure the file exists in the same folder
3. For internal links, use `#` before the section ID (e.g., `href="#features"`)
4. Clear your browser cache (Ctrl+Shift+Delete on Windows, Cmd+Shift+Delete on Mac)

**Example of correct links:**
```html
<!-- Internal link to section on same page -->
<a href="#features">Features</a>

<!-- Link to another file in same folder -->
<a href="privacy.html">Privacy</a>

<!-- External link to another website -->
<a href="https://example.com">Example</a>
```

### Issue 2: Mobile Menu Not Working

**Problem:** The hamburger menu doesn't open on mobile

**Solution:**
1. Verify the JavaScript code is intact at the bottom of your HTML file
2. Check that Font Awesome is loading (icons should appear)
3. Test in a different browser
4. Clear browser cache

### Issue 3: Styling Looks Wrong

**Problem:** Colors, spacing, or fonts don't look right

**Solution:**
1. Verify Tailwind CSS is loading from CDN (check network tab in browser developer tools)
2. Check that you haven't accidentally deleted any Tailwind classes
3. Make sure you're using valid Tailwind class names
4. Clear browser cache and hard refresh (Ctrl+Shift+R on Windows, Cmd+Shift+R on Mac)

### Issue 4: FAQ Accordion Not Opening

**Problem:** Clicking FAQ questions doesn't expand answers

**Solution:**
1. Verify the JavaScript code is present and intact
2. Check that each FAQ item has the correct structure with `faq-item`, `faq-question`, and `faq-answer` classes
3. Ensure the `hidden` class is on the `faq-answer` div

### Issue 5: Responsive Design Broken

**Problem:** Page doesn't look good on mobile or tablet

**Solution:**
1. Check that you have the viewport meta tag: `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
2. Don't remove responsive classes like `md:` and `lg:`
3. Test in actual mobile devices or use browser developer tools (F12)

### Issue 6: Images Not Showing

**Problem:** Background images or icons don't appear

**Solution:**
1. For background images, verify the URL is correct and accessible
2. For Font Awesome icons, ensure the CDN link is loading
3. Check browser console for errors (F12 → Console tab)
4. Try clearing browser cache

---

## Best Practices for Maintenance

### 1. Backup Your Files

Before making changes, always keep a backup:
- Save copies of your HTML files with dates (e.g., `index_backup_2025-01.html`)
- Use version control like Git if you're comfortable with it
- Store backups in a safe location

### 2. Make One Change at a Time

- Change one thing and test it
- Don't make multiple changes at once
- This makes it easier to find problems

### 3. Test After Every Change

- Test on desktop, tablet, and mobile
- Test all links
- Test interactive features (FAQ, mobile menu)
- Test in multiple browsers (Chrome, Firefox, Safari, Edge)

### 4. Keep Your Content Updated

- Update testimonials regularly with real customer feedback
- Keep FAQ questions current
- Update contact information
- Review and update the About Us section annually

### 5. Use Comments in Your Code

Add comments to help you remember what things do:

```html
<!-- This is a feature card - update the title, description, and icon here -->
<div class="card-hover bg-gray-800 border border-gray-700 rounded-xl p-8">
    <h3 class="text-2xl font-bold mb-3">Feature Title</h3>
    <p class="text-gray-300">Feature description</p>
</div>
```

### 6. Organize Your Files

Create a folder structure like this:
```
your-website/
├── index.html
├── privacy.html
├── terms.html
├── blog.html
├── images/
│   ├── logo.png
│   └── background.jpg
├── css/
│   └── custom-styles.css (optional)
└── js/
    └── custom-scripts.js (optional)
```

### 7. Monitor Performance

- Test page load speed (use Google PageSpeed Insights)
- Monitor broken links regularly
- Check that all external services (scheduling, email) are working

### 8. Security Considerations

- Keep your email address and phone number current
- Don't hardcode sensitive information in the HTML
- Regularly update any external services you use
- Use HTTPS when hosting your website

### 9. SEO Optimization

Update these meta tags in the `<head>` section:

```html
<meta name="description" content="Update this with a compelling description">
<meta name="keywords" content="update, these, keywords">
<meta name="author" content="Your Company Name">
```

### 10. Regular Maintenance Checklist

**Monthly:**
- [ ] Check all links work
- [ ] Verify contact information is correct
- [ ] Test mobile responsiveness
- [ ] Check spelling and grammar

**Quarterly:**
- [ ] Update testimonials if you have new ones
- [ ] Review and update FAQ section
- [ ] Check external services (scheduling, email)
- [ ] Update copyright year if needed

**Annually:**
- [ ] Review entire website content
- [ ] Update About Us section
- [ ] Review and update Privacy Policy and Terms
- [ ] Check for any broken external links

---

## Quick Reference: Common Tasks

### Updating the Main Headline
Find line ~95, update both the main text and the colored span text.

### Changing Colors
Replace color class names like `text-gray-300` with new colors like `text-purple-400`.

### Adding More Space
Change padding with `p-8` → `p-12` or margins with `mb-4` → `mb-8`.

### Updating Contact Info
Search for email and phone number, replace with your information.

### Fixing Scheduling Link
Search for `https://app.acuityscheduling.com/schedule/99abdf40` and replace with your scheduling URL.

### Adding New Testimonial
Copy a testimonial card block and paste below it, then update the name, title, and quote.

### Adding New FAQ
Copy an FAQ item block and paste below it, then update the question and answer.

---

## Getting Help

If you encounter issues:

1. **Check the browser console** - Press F12, go to Console tab, look for red error messages
2. **Validate your HTML** - Use W3C Validator (validator.w3.org)
3. **Test in incognito mode** - This clears cache and helps identify real issues
4. **Compare with the original** - Look at the original code to see what might be different
5. **Search online** - Search for the specific error message you're seeing

---

## Conclusion

Your Oakland Accident Care landing page is now fully customizable. Remember:

- **Text changes** are simple - just find and replace
- **Link fixes** require updating `href` attributes
- **Styling changes** use Tailwind CSS classes
- **Always test** after making changes
- **Keep backups** of working versions

For more information about Tailwind CSS, visit: https://tailwindcss.com/docs

Good luck with maintaining and improving your landing page! Your patients will appreciate the professional, compassionate online presence you've created.