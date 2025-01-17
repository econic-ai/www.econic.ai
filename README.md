# Econic.ai

Intelligent insights, collaboration and automation for your digital economy.

## Project Overview

This repository contains the source code for the Econic.ai website. The site is built using Hugo static site generator, with Tailwind CSS, SCSS, and Svelte for enhanced functionality.

## Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:
- Git
- Node.js (v18 or higher)
- Yarn (latest version)
- Hugo Extended (latest version)
- Go (required for Hugo)

### Project Setup

1. Clone the repository:

```bash
git clone https://github.com/econic-ai/www.econic.ai.git
cd www.econic.ai
```

2. Install dependencies:

```bash
yarn install
```

3. Start the development server:
```bash
hugo server -D
```

The site will be available at `http://localhost:1313`

## Project TODO List

### 1. Initial Hugo Setup
- [ ] Create a new Hugo site:
  ```bash
  hugo new site . --force
  ```
- [ ] Set up basic Hugo configuration in `config.toml`
- [ ] Create initial content structure:
  ```
  content/
  ├── _index.md          # Home page
  ├── api-docs/
  │   └── _index.md      # API documentation
  └── blog/
      └── _index.md      # Blog listing page
  ```

### 2. Theme Development
- [ ] Create a basic theme structure:
  ```
  themes/econic/
  ├── layouts/
  │   ├── _default/
  │   │   ├── baseof.html
  │   │   ├── list.html
  │   │   └── single.html
  │   ├── partials/
  │   │   ├── header.html
  │   │   ├── footer.html
  │   │   └── nav.html
  │   └── index.html
  ```

### 3. Asset Pipeline Setup
- [ ] Configure Tailwind CSS:
  - [ ] Initialize Tailwind:
    ```bash
    yarn add -D tailwindcss
    yarn tailwindcss init
    ```
  - [ ] Create `assets/css/main.scss`
  - [ ] Set up Tailwind directives in SCSS

- [ ] Configure Svelte:
  - [ ] Create `assets/js/components/` directory
  - [ ] Set up Svelte build process in `package.json`
  - [ ] Install Svelte dependencies:
    ```bash
    yarn add -D svelte svelte-loader
    ```
  - [ ] Create initial Svelte components

### 4. Template Implementation
- [ ] Create basic templates first:
  - [ ] Implement base layout
  - [ ] Create header partial
  - [ ] Create footer partial
  - [ ] Create navigation partial

### 5. Content Pages
- [ ] Implement home page layout
- [ ] Create API documentation page structure
- [ ] Set up blog listing and single post templates

### 6. Design and Implementation
- [ ] Review Figma design at https://www.figma.com/design/KVtINn6yZtnmhO2NgqEEI6/econic.ai
- [ ] Redesign to a minimal responsive layout:
  - [ ] Clean, flat design system with:
    - Dark background
    - A single primary and secondary color
    - Font: Kreon and Life Saver
  - [ ] Responsive breakpoints.
- [ ] Break down design into components
- [ ] Implement design using Tailwind and SCSS
- [ ] Create placeholder Svelte components for interactive elements

## Development Guidelines

### CSS Structure
- Use SCSS for custom styles
- Follow Tailwind CSS utility-first approach
- Create custom components when needed using @apply directives

### JavaScript/Svelte
- Place Svelte components in `assets/js/components/`
- Use ES6+ features
- Follow component-based architecture

### Hugo Best Practices
- Use partials for reusable components
- Implement proper content organization
- Utilize Hugo's built-in functions for optimization

## Build and Deployment

To build the site for production:

```bash
hugo --minify
```

The built site will be in the `public/` directory.

## Additional Resources

- [Hugo Documentation](https://gohugo.io/documentation/)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [Svelte Documentation](https://svelte.dev/docs)

## Need Help?

If you run into any issues:
1. Check the Hugo documentation
2. Review the Tailwind and Svelte docs
3. Reach out to the team lead

## Contributing

1. Create a new branch for each major milestone above.
2. Make your changes
3. Submit a pull request
4. Wait for review and approval

Remember to follow the team's coding standards and commit message conventions.