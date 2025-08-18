# Astrio Documentation

This repository contains the documentation for Astrio, built with [Mintlify](https://mintlify.com/).

## 🚀 Quick Start

### Prerequisites

- Node.js 18 or higher
- npm or yarn

### Local Development

1. **Install Mintlify CLI**
   ```bash
   npm install -g mintlify
   ```

2. **Clone and navigate to the repository**
   ```bash
   git clone <your-repo-url>
   cd docs
   ```

3. **Start the development server**
   ```bash
   mintlify dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:3000` to see your documentation.

## 📁 Project Structure

```
docs/
├── .github/workflows/    # GitHub Actions for deployment
├── api-reference/        # API documentation
├── essentials/          # Core documentation pages
├── images/              # Images and assets
├── introduction.mdx     # Welcome page
├── quickstart.mdx       # Getting started guide
├── development.mdx      # Development guide
├── mint.json           # Mintlify configuration
└── README.md           # This file
```

## 📝 Writing Documentation

### Creating New Pages

1. Create a new `.mdx` file in the appropriate directory
2. Add frontmatter with title and description:
   ```mdx
   ---
   title: 'Page Title'
   description: 'Page description'
   ---
   ```
3. Add the page to `mint.json` navigation

### Using Components

Mintlify provides several built-in components:

- `<Card>` and `<CardGroup>` - For feature highlights
- `<Steps>` and `<Step>` - For step-by-step guides
- `<Accordion>` and `<AccordionGroup>` - For collapsible content
- `<Note>`, `<Tip>`, `<Warning>`, `<Info>` - For callouts
- `<CodeGroup>` - For multiple code examples

### Code Examples

Use fenced code blocks with language specification:

````markdown
```javascript
const example = "Hello World";
```
````

## 🎨 Customization

### Branding

Update the following in `mint.json`:
- `name` - Documentation site name
- `logo` - Path to your logo files
- `favicon` - Path to favicon
- `colors` - Brand colors

### Navigation

Modify the `navigation` array in `mint.json` to organize your content:

```json
{
  "navigation": [
    {
      "group": "Get Started",
      "pages": ["introduction", "quickstart"]
    }
  ]
}
```

## 🚀 Deployment

### GitHub Pages (Automatic)

This repository is configured to automatically deploy to GitHub Pages when changes are pushed to the `main` branch.

#### Setup GitHub Pages

1. Go to your repository settings
2. Navigate to "Pages" in the sidebar
3. Set source to "GitHub Actions"
4. Push to the `main` branch to trigger deployment

### Manual Deployment

You can also deploy manually:

```bash
# Build the documentation
mintlify build

# Deploy to your hosting provider
# (upload the contents of the _site directory)
```

### Other Hosting Options

- **Vercel**: Connect your GitHub repository
- **Netlify**: Connect your GitHub repository
- **Mintlify Cloud**: Use `mintlify deploy`

## 🔧 Configuration

### Environment Variables

If you need to customize the build process, you can use these environment variables:

- `MINTLIFY_SITE_URL` - Your site's base URL
- `MINTLIFY_ANALYTICS_ID` - Google Analytics ID

### Advanced Configuration

For advanced configuration options, refer to the [Mintlify documentation](https://mintlify.com/docs).

## 📚 Resources

- [Mintlify Documentation](https://mintlify.com/docs)
- [MDX Documentation](https://mdxjs.com/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This documentation is licensed under the [MIT License](LICENSE).

## 🆘 Support

If you need help with the documentation:

1. Check the [Mintlify documentation](https://mintlify.com/docs)
2. Open an issue in this repository
3. Contact the team at support@astrio.dev 