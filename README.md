# Cleveland Junk Removal Landing Page - Maintenance Guide

This guide will help you maintain and customize the Cleveland Junk Removal landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions for common updates.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the company name and navigation menu. To update:

1. **Company Name:**
```html
<div class="text-2xl font-bold text-blue-600">CLE Junk Removers</div>
```
Simply replace "CLE Junk Removers" with your desired text.

2. **Navigation Menu Items:**
```html
<div class="hidden md:flex space-x-8">
    <a href="#services" class="text-gray-600 hover:text-blue-600 transition duration-300">Services</a>
    <!-- Additional menu items -->
</div>
```
Change the text between `<a>` tags to update menu items.

### Hero Section
Located at the top of the page:

1. **Main Heading:**
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 mb-6 leading-tight">
    Cleveland's Fastest Junk Removal – Local, Licensed, and Affordable
</h1>
```
Replace the heading text while maintaining the classes.

2. **Subheading:**
```html
<p class="text-xl md:text-2xl text-gray-600 mb-8">
    We Haul It All – Fast, Friendly Junk Removal in Cleveland
</p>
```

### Understanding Tailwind Classes
Key classes explained:
- `text-4xl`: Large text size
- `md:text-5xl`: Larger text on medium screens
- `font-bold`: Bold text
- `mb-6`: Margin bottom spacing
- `text-gray-900`: Dark gray text color

## Managing Links

### Internal Navigation Links
Current internal links use hashtags to scroll to sections:
```html
<a href="#services">Services</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
<a href="#contact">Contact</a>
```

To update:
1. Identify the section ID you want to link to
2. Update the `href` attribute with `#section-id`
3. Ensure the target section has a matching `id` attribute

### External Links
The site contains several external links that need updating:

1. **Quote Button Link:**
```html
<a href="https://clejunkremovers.com" class="bg-blue-600 text-white px-6 py-2 rounded-full">
    Get Quote
</a>
```
Replace `https://clejunkremovers.com` with your desired URL.

2. **Social Media Links:**
```html
<div class="flex space-x-4">
    <a href="#" class="text-gray-400 hover:text-white transition duration-300">
        <i class="fab fa-facebook"></i>
    </a>
    <!-- Additional social links -->
</div>
```
Replace `#` with your social media profile URLs.

## Adding Privacy and Terms Pages

### Footer Modification
Add privacy and terms links to the Quick Links section:

```html
<div>
    <h4 class="text-lg font-semibold mb-4">Quick Links</h4>
    <ul class="space-y-2">
        <li><a href="#services" class="text-gray-400 hover:text-white transition duration-300">Services</a></li>
        <!-- Add these new lines -->
        <li><a href="privacy.html" class="text-gray-400 hover:text-white transition duration-300">Privacy Policy</a></li>
        <li><a href="terms.html" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a></li>
    </ul>
</div>
```

### Creating Policy Pages
1. Create new files named `privacy.html` and `terms.html`
2. Use the same header and footer as `index.html`
3. Maintain consistent styling using Tailwind classes

## Troubleshooting

Common issues and solutions:

1. **Broken Internal Links**
- Verify that section IDs match exactly with href attributes
- Check for typos in IDs
- Ensure sections have unique IDs

2. **Responsive Design Issues**
- Check that you're maintaining responsive classes (e.g., `md:text-5xl`)
- Test on different screen sizes using browser dev tools
- Don't remove `md:` or `lg:` prefixes from classes

3. **Style Inconsistencies**
- Keep color classes consistent (e.g., `text-blue-600`)
- Maintain spacing patterns using margin/padding classes
- Use the same rounded corners (`rounded-full`, `rounded-lg`)

Remember to:
- Always test changes in multiple browsers
- Maintain backup copies before making significant changes
- Check mobile responsiveness after updates
- Keep consistent spacing and styling throughout the page

Need additional help? Contact your web developer or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).