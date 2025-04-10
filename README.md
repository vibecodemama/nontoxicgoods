# Mama's Top Picks

A curated collection of family-vetted non-toxic products, focusing on high quality and made in the USA where possible. This interactive web application allows visitors to easily browse, search, and filter products across multiple categories.

## Features

- **Color-coded categories** for easy visual browsing
- **Product filtering** by category
- **Responsive design** works on desktop, tablet, and mobile devices
- **Sortable and searchable** product database

## Live Site

View the site at: https://vibecodemama.com/top-picks/

## Installation

This is a static HTML/CSS/JavaScript website, so installation is straightforward:

1. Clone this repository:

   ```sh
   git clone https://github.com/yourusername/mamas-top-picks.git
   ```

2. Open index.html in your browser to view locally

3. Deploy to GitHub Pages:
- Go to your repository settings
- Navigate to Pages section
- Select main branch as the source
- Click Save

## Customization

### Adding New Products

To add new products, edit the `productsData` array in the JavaScript section:

```javascript
const productsData = [
 {
     "Product": "Your New Product Name",
     "Category": "Existing Category",
     "Link": "https://product-link.com",
     "Notes": "Details about the product",
     "Brand": "Brand Name"
 },
 // More products...
];
```

### Creating New Categories

If adding a new category, you should also add a color for it in the categoryColors object:

```javascript

const categoryColors = {
    'Your New Category': { color: 'var(--new-category-color)', class: 'new-category' },
    // Other categories...
};
```

And add the corresponding CSS variable in the :root section:

```css

:root {
    /* Other variables */
    --new-category-color: #HEX_COLOR;
}
```

## How It Works

- Products Data: All product information is stored in a JavaScript array
- Filtering: Real-time filtering happens client-side with JavaScript
- Styling: CSS variables control the color scheme and layout
- Categories: Each product category has its own color for easy identification

## Technologies Used

- HTML5
- CSS3 (with CSS variables for theming)
- Vanilla JavaScript (no frameworks)
- Font Awesome icons
- Google Fonts
- Responsive design
