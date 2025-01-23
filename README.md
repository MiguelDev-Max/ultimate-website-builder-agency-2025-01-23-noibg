# WebBuilder Landing Page - Maintenance Guide

This guide will help you maintain and customize the WebBuilder landing page. Whether you're new to HTML and CSS or just getting started, follow these instructions to make updates while maintaining the page's professional appearance.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the logo and navigation menu. To update:

1. **Logo Text:**
```html
<!-- Find this section in the header -->
<div class="text-2xl font-bold bg-gradient-to-r from-purple-600 to-blue-500 bg-clip-text text-transparent">
    WebBuilder  <!-- Change this text to your brand name -->
</div>
```

2. **Navigation Menu Items:**
```html
<div class="hidden md:flex space-x-8">
    <!-- Update these link texts as needed -->
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```

### Hero Section
Located at the top of the page:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold mb-6">
    Ultimate Website Builder Agency  <!-- Main headline -->
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12">
    An advanced website builder for modern businesses  <!-- Subheadline -->
</p>
```

### Tailwind CSS Classes Explained
- `text-4xl`: Large text size
- `md:text-5xl`: Larger text on medium screens
- `font-bold`: Bold text weight
- `mb-6`: Margin bottom spacing
- `text-gray-600`: Gray text color

## Managing Links

### Navigation Menu Links
```html
<!-- Internal page links (scroll to sections) -->
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
<a href="#contact">Contact</a>

<!-- To change these to external pages, replace # with full URL -->
<a href="https://yoursite.com/features">Features</a>
```

### Call-to-Action Buttons
Current external link that needs updating:
```html
<a href="https://www.bocastraders.com" class="inline-block bg-gradient-to-r...">
    Start Building Now  <!-- Update text and URL -->
</a>
```

### Footer Links
```html
<div class="grid grid-cols-1 md:grid-cols-4 gap-12">
    <!-- Quick Links Section -->
    <ul class="space-y-2">
        <li><a href="#features">Features</a></li>
        <li><a href="#benefits">Benefits</a></li>
        <li><a href="#faq">FAQ</a></li>
    </ul>
</div>
```

## Adding Privacy and Terms Pages

### Step 1: Create New HTML Files
Create two new files in your project folder:
- `privacy.html`
- `terms.html`

### Step 2: Update Footer Links
Replace the placeholder links with:
```html
<!-- Find this section in the footer -->
<div>
    <h4 class="text-white text-lg font-semibold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

### Step 3: Style Consistency
Ensure new pages maintain the same styling by copying these elements from index.html:
- Header section
- Footer section
- Font imports
- Tailwind CSS import

## Troubleshooting

### Common Issues and Solutions

1. **Broken Links**
   - Check for typos in href attributes
   - Ensure file names match exactly
   - Verify file locations in your project folder

2. **Styling Issues**
   - Make sure Tailwind CSS is properly imported
   - Check for missing classes
   - Verify responsive classes (md:, lg:) are correct

3. **Layout Problems**
   - Check container classes are present
   - Verify grid column settings
   - Ensure proper spacing classes

### Need Help?
- Double-check the original HTML structure
- Use browser developer tools (F12) to inspect elements
- Maintain consistent indentation for readability
- Test all links after making changes

Remember to:
- Back up files before making changes
- Test on multiple devices and browsers
- Keep the responsive design in mind
- Maintain consistent spacing and styling

This guide covers the basics of maintaining your WebBuilder landing page. For additional support or questions, refer to the Tailwind CSS documentation or contact your development team.