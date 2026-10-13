# Satner Portfolio

A modern personal portfolio website built as a static multi-page landing site for a technical support engineer and professional services brand. The project includes a responsive homepage, portfolio sections, blog pages, and a working contact form setup.

## Project Overview

This portfolio template is designed to showcase:

- Professional experience and personal branding
- Services and expertise
- Portfolio highlights and case studies
- Blog/news-style content
- Contact form for inquiries

The design is based on a clean, polished Bootstrap layout with custom styling, animation support, and image-based sections.

## Tech Stack

The website uses a classic front-end setup with a lightweight server-side email handler:

- HTML5  
  Provides the page structure, content, and semantic layout for all website sections.

- CSS3  
  Controls the theme styling, spacing, typography, colors, layout responsiveness, and visual polish.

- JavaScript / jQuery  
  Adds interactivity, dropdown effects, slider features, and general page behavior. It is also used for UI enhancements and dynamic components.

- Bootstrap 4  
  Supplies the responsive grid system, navigation components, buttons, forms, and design utilities used throughout the site.

- PHP  
  Handles the contact form submission in `contact_process.php` by collecting form data and sending it via the server mail function.

- Custom theme assets and vendor libraries  
  Includes packaged design assets, icon sets, and third-party front-end libraries that support the visual style and page features.

## Pages Included

Each page serves a distinct purpose in the portfolio website:

- Home (`index.html`)  
  The main landing page featuring the hero section, profile introduction, service summary, experience highlights, and CTAs such as "Hire Me" and "Get CV".

- About (`about.html`)  
  Provides a deeper overview of the personal profile, background, experience, and professional identity.

- Services (`services.html`)  
  Lists the key offerings, technical capabilities, and professional support areas available to clients or employers.

- Portfolio (`portfolio.html`)  
  Displays selected projects, work samples, and case studies in a gallery-style layout.

- Portfolio Details (`portfolio-details.html`)  
  A detailed project showcase page intended to explain a project in more depth with supporting visuals and descriptions.

- Blog (`blog.html`)  
  A news or article listing page that presents blog posts or updates in a magazine-style layout.

- Blog Details (`single-blog.html`)  
  A dedicated article page for a single post with content layout suitable for long-form writing.

- Contact (`contact.html`)  
  Contains the contact form, user information fields, and a communication section for inquiries or job opportunities.

- Elements page (`elements.html`)  
  A generic UI showcase page used to demonstrate reusable design elements, buttons, typography, cards, and page components.

## Project Structure

The project is organized into static site assets, page files, and vendor resources:

```text
.
├── css/                             # Main stylesheet files and theme styling
│   ├── bootstrap.css               # Bootstrap framework styles
│   ├── font-awesome.min.css        # Font Awesome icon library
│   ├── magnific-popup.css          # Lightbox popup styling
│   └── style.css                  # Custom theme styles for the portfolio
├── fonts/                          # Font files used across the website
├── img/                            # Images, banners, logos, and portfolio visuals
├── js/                             # JavaScript files for page behavior and interactions
├── scss/                           # SCSS source files for theme customization
├── vendors/                        # Third-party scripts, plugins, and assets
├── about.html                      # Professional background section
├── blog.html                       # Blog listing page
├── contact.html                    # Contact page and form UI
├── contact_process.php             # PHP handler for sending form submissions by email
├── elements.html                   # UI component demonstration page
├── index.html                      # Main homepage
├── portfolio-details.html          # Detailed project description page
├── portfolio.html                  # Portfolio gallery with project highlights
├── services.html                   # Services and expertise page
├── single-blog.html                 # Individual blog post view
├── prepros-6.config                # Prepros build configuration for SCSS processing
├── README.md                       # Project overview and usage guide
└── .git/                           # Git repository metadata
```

### Folder and Asset Details

- `css/` contains the project styling files, including Bootstrap, custom theme styles, and third-party stylesheets.
- `fonts/` stores custom icon and typography font files used by the theme.
- `img/` holds all images, including profile artwork, brand elements, portfolio visuals, and banners.
- `js/` includes scripts for interactions such as menu behavior, page animations, and plugin integration.
- `scss/` is the source folder for SCSS styling if the design is customized or rebuilt from source.
- `vendors/` contains external libraries and plugins such as carousel, lightbox, and select UI assets.

## Features

- Fully responsive layout for desktop, tablet, and mobile devices
- Portfolio-style sections and hero banner
- Service and experience sections
- Blog and article pages
- Contact form integration using PHP mail
- Bootstrap navigation and clean card-based design
- Custom icons and visual styling from vendor assets

## How to Run Locally

Because the site includes a PHP mail handler, the easiest way to run it locally is with a local PHP server.

1. Open a terminal in the project folder.
2. Run:

```bash
php -S localhost:8000
```

3. Visit:

```text
http://localhost:8000
```

You can also open the HTML files directly in a browser for basic viewing, but the contact form requires PHP support.

## Contact Form Configuration

The contact form is processed by `contact_process.php`.

Before deployment, update the recipient email address in the PHP file:

```php
$to = "your-email@example.com";
```

Also confirm that your hosting environment supports PHP `mail()` functionality. Some hosting providers require SMTP configuration or a mail plugin/service for reliable email sending.

## Notes

- The design is a static portfolio template and does not use a framework such as React or Angular.
- Some assets and vendor libraries are included in the repository for styling and interactivity.
- You may want to replace demo text, sample portfolio items, and placeholder contact information with your own content.

## License

This project is provided as a template for educational and personal portfolio use. If you are using it as a base for a live site, make sure to review licensing for any included third-party assets and replace branding elements as needed.

## Author / Branding

The content in the project appears to be set up for a personal brand named "Satner" and references a professional profile for Stella Matutina Uwamahoro. You may customize the text in the HTML pages to match your own identity and portfolio details.
