# zekeinnovate - Company Website

This repo contains the source code for Zekeinnovate company website. 

## Website Structure

The website is a multi-page static site, with each major section residing in its own HTMl file.
* **`index.html`**: The main landing page(Home).
* **`services.html`**: Details the software solutions and services offered by ZekeInnovate.
* **`about.html`**: Provides information about the company, its mission, vision, and values.
* **`contact.html`**: Includes a contact form (static, requires backend integration for live submission) and other ways to get in touch.

## Features

* **Responsive Design**: Adapts to various screen sizes (desktop, tablet, mobile) using Tailwind CSS's utility classes.
* **Mobile-First Navigation**: Features a hamburger menu for smaller screens that expands to show navigation links, ensuring a good user experience on all devices. The navigation is implemented using CSS-only techniques (the "checkbox hack").
* **Sticky Navigation**: The navigation bar remains at the top of the viewport as the user scrolls.
* **Semantic HTML**: Structured with semantic HTML5 tags for better accessibility and SEO.
* **Tailwind CSS Styling**: Leverages the utility-first Tailwind CSS framework for rapid UI development and consistent styling.
* **Custom CSS**: Minimal custom CSS is used for elements or styles not easily achievable with Tailwind's default utilities (e.g., specific hero background gradients, active navigation link indicators, and the hamburger menu toggle logic).
* **Clear Call-to-Actions**: Designed to guide users towards learning more about services or contacting the company.
* **Informative Content Sections**: Well-defined sections for showcasing services, company information, and contact details.
* **SVG Icons**: Uses inline SVGs for icons to ensure scalability and crisp rendering on all displays.

## Technologies Used

* **HTML5**: For the basic structure and content of the website.
* **Tailwind CSS v3**: For all styling and responsive design. Loaded via CDN.
* **Google Fonts (Inter)**: For a clean and modern typography.
* **Heroicons/Custom SVGs**: For iconography.

## Setup and Usage

1.  **Clone the repository (if applicable) or download the files.**
    ```bash
    $ git clone https://github.com/2502-5-software/zekeinnovate.git
    $ cd zekeinnovate
    ```
2.  **Open HTML Files in a Browser**:
    Simply open any of the `.html` files (e.g., `index.html`) in your web browser to view the website. No build process or local server is strictly required for viewing, as it's a static site.

## File Overview

* `index.html`: Home page.
* `services.html`: Services page.
* `about.html`: About Us page.
* `contact.html`: Contact Us page.
* **(No separate CSS file)**: Styles are primarily from Tailwind CSS via CDN, with minor custom styles embedded in `<style>` tags within each HTML file's `<head>` section.
* **(No JavaScript files)**: The website is designed to function without client-side JavaScript for core navigation and layout.

## Navigation Details

The navigation menu is designed to be responsive:
* **Desktop/Large Screens**: Displays a horizontal list of links.
* **Tablet/Mobile Screens**: Displays a hamburger icon. Clicking this icon reveals a vertical list of navigation links. This is achieved using a hidden checkbox and CSS sibling selectors (`#menu-toggle:checked + label + div#menu-links`). When the mobile menu is opened, it pushes the page content down rather than overlaying it.

## Contact Form

The contact form in `contact.html` is currently a static HTML form. For it to send messages, it would need to be integrated with a backend script (e.g., PHP, Node.js, Python) or a third-party form handling service like Formspree, Netlify Forms, etc.

## Customization

* **Content**: Edit the text content directly within the HTML files in the respective sections.
* **Styling**:
    * Most styling can be adjusted by changing Tailwind CSS classes on the HTML elements.
    * For custom CSS (e.g., `nav-link-active`, `hero-bg`, hamburger menu logic), modify the `<style>` block in the `<head>` of each HTML file.
* **Images**: Placeholder images are used (from `placehold.co`). Replace these with your actual company images.
* **SVG Icons**: Modify the inline SVG code if different icons are desired.

## Future Enhancements (Suggestions)

* Integrate the contact form with a backend service.
* Add a portfolio or case studies section.
* Implement a blog.
* Optimize images for faster loading.
* Add more detailed accessibility (ARIA attributes) enhancements if needed.
* Consider a build step for Tailwind CSS to purge unused styles for production if the project grows significantly.

---

This README provides a comprehensive guide to the ZekeInnovate static website.