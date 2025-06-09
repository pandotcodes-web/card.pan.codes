# Pan's Cards

A visual, no-code tool for creating beautiful landing pages and digital business cards. Build professional-looking pages with a simple drag-and-drop interface, then export them as standalone HTML files that can be hosted anywhere.

## 🌟 Features

### Visual Editor
- **Two-column interface**: Edit on the left, preview on the right
- **Real-time preview**: See changes instantly as you type
- **Drag-and-drop reordering**: Easily rearrange elements by dragging the grip handles
- **Template system**: Choose from multiple content types with pre-built styling

### Content Types
- **📝 Text Blocks**: Rich text with full Markdown support
- **🔗 Action Rows**: Social media links with branded icons and colors
- **🖼️ Images**: Add images from any URL
- **📏 Spacing**: Control layout with customizable spacing elements
- **📦 Content Boxes**: Call-to-action sections with custom backgrounds and buttons

### Rich Text Support
- **Markdown rendering**: Headers, bold, italic, links, lists, and more
- **Emoji support**: Type `:smile:` or `:thumbs_up:` for emoji rendering
- **Icon integration**: Use `@icon-name` for Bootstrap Icons, `+brand-name` for brand icons or `!icon-name` for FontAwesome Icons.
- **Custom styling**: Adjust colors, alignment, and sizing for any element

### Export & Sharing
- **Standalone HTML export**: Self-contained files with all dependencies included
- **JSON export/import**: Share configurations or create templates
- **QR code generation**: Automatic QR codes for easy mobile sharing
- **Social sharing**: Built-in browser sharing integration
- **Import from URLs**: Load existing pages to use as starting points

## 🚀 Getting Started

### Basic Usage

1. **Open the editor** in your web browser
2. **Configure global settings** in the top section:
   - Site title (appears in browser tab)
   - Background color
   - Toggle footer, share button, and QR code features
3. **Add content** by clicking the `+` button
4. **Choose content type** from the dropdown (Text, Action Row, Image, etc.)
5. **Edit content** using the controls in the left column
6. **Preview** your changes in the right column
7. **Export** your finished page using the download buttons

### Adding Different Content Types

#### Text Blocks
- Select "Text" from the type dropdown
- Write content in the textarea using Markdown syntax
- Examples:
  ```markdown
  # Main Heading
  ## Subheading
  
  **Bold text** and *italic text*
  
  - List item 1
  - List item 2
  
  And emojis! :fire: :rocket:
  ```
  - A full markdown reference can be found at [MARKDOWN.md](https://github.com/pandotcodes-web/card.pan.codes/MARKDOWN.md)

#### Action Rows (Social Links)
- Select "Action Row" from the type dropdown
- Click the `+` button to add social links
- Choose from pre-configured services (GitHub, Discord, YouTube, etc.) or create custom ones
- For each link:
  - Pick the service from dropdown (or "Custom" for your own icon)
    - For custom icons, see [Custom Icons](#custom-icons).
  - Enter the URL
  - Add display text

#### Images
- Select "Image" from the type dropdown
- Enter the image URL in the input field
- The image will appear instantly in the preview

#### Content Boxes
- Select "Content" from the type dropdown
- Customize:
  - Background color of the content box
  - Button color
  - Text content (supports Markdown and emojis)
  - Button link and text

### Advanced Features

#### Custom Icons
- **Twemoji**: Use no prefix (e.g., `heart`)
- **Bootstrap Icons**: Use `@icon-name` (e.g., `@heart-fill`)
- **Brand Icons (simpleicons.org)**: Use `+brand-name` (e.g., `+github`, `+discord`)
- **Font Awesome Free**: Use `!category/icon-name` (e.g., `!solid/star`)

#### Styling Options
- Click "▶ More Options" on any element for advanced styling
- Adjust text alignment, colors, and height
- Each element can be individually customized

#### Import/Export
- **Download HTML**: Get a complete, self-contained webpage
- **Download JSON**: Save your configuration to share or backup
- **Import**: Load a JSON configuration or import from a URL
- **View exported files**: Use the arrow buttons to open exports in new tabs rather than downloading them

## 🛠️ Technical Details

### Dependencies
- **[marked](https://github.com/markedjs/marked)**: Markdown parsing and rendering
    - **Marked extensions**:
- **[node-emoji](https://github.com/omnidan/node-emoji)**: Emoji text-to-image conversion
- **[twemoji](https://github.com/twitter/twemoji)**: High-quality emoji graphics
- **Various icon packs**: [bootstrap-icons](https://github.com/twbs/icons), [Font Awesome Free](https://github.com/FortAwesome/Font-Awesome), [Simple Icons](https://github.com/simple-icons/simple-icons)

### Browser Compatibility
- Modern browsers with ES6 module support
- Chrome, Firefox, Safari, Edge (recent versions)

### Hosting
The exported HTML files are completely self-contained and can be hosted on:
- GitHub Pages
- Any static hosting service
- Your own web server

## 📖 Examples

### Creating a Personal Landing Page
1. Set site title to your name
2. Add a text block with your bio using Markdown
3. Add an action row with your social media links
4. Add a content box with a call-to-action (like "Contact Me")
5. Export as HTML and upload to your hosting service

### Building a Project Showcase
1. Start with a text block describing your project
2. Add images showing screenshots or demos
3. Create action rows linking to GitHub, live demo, documentation
4. Use content boxes for download buttons or getting started guides

### Making a Digital Business Card
1. Add text blocks for your name, title, and brief description
2. Include an image with your photo or logo
3. Add action rows for email, LinkedIn, website, and other contact methods
4. Generate QR code for easy sharing at networking events

## 🔧 Development

The editor is also just an HTML file, thought not entirely self-contained. Nonetheless, you should be able to run it by simply opening it in a browser, and edit it with whatever file you'd like.

**Live Demo**: [card.pan.codes](https://card.pan.codes/)
**Example Page**: [pan.codes](https://pan.codes/)