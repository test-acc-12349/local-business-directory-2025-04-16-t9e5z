# Local Business Directory

> Discover the best local businesses in one place

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization Guide](#customization-guide)
- [Deployment](#deployment)
- [Troubleshooting](#troubleshooting)
- [Support](#support)

## Overview
Local Business Directory is a responsive web directory showcasing businesses in a clean, three-column grid layout. The platform helps users discover and connect with local businesses through an intuitive category-based navigation system.

## Features
- Responsive 3-column grid layout
- Category-based filtering
- Search functionality
- Business detail pages
- Contact forms
- Mobile-friendly design
- SEO optimized structure
- Custom category labels
- Image optimization

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Basic knowledge of HTML/CSS

### Installation
1. Clone the repository:
```bash
git clone https://github.com/yourusername/local-business-directory.git
```

2. Install dependencies:
```bash
cd local-business-directory
npm install
```

3. Start development server:
```bash
npm run dev
```

## Directory Structure
```
local-business-directory/
├── src/
│   ├── components/
│   │   ├── Directory/
│   │   ├── Header/
│   │   └── Footer/
│   ├── data/
│   │   └── businesses.json
│   ├── styles/
│   │   └── main.css
│   └── pages/
├── public/
│   └── images/
├── config/
└── package.json
```

## Customization Guide

### Adding Business Listings
1. Open `src/data/businesses.json`
2. Add new business entry:
```json
{
  "id": "unique-id",
  "name": "Business Name",
  "category": "Category",
  "description": "Business description",
  "address": "Business address",
  "phone": "Phone number",
  "website": "Website URL",
  "image": "image-filename.jpg"
}
```

### Modifying Categories
1. Navigate to `src/config/categories.js`
2. Edit category structure:
```javascript
export const categories = [
  {
    id: "category-1",
    label: "Restaurants",
    icon: "restaurant-icon"
  },
  // Add more categories
];
```

### Customizing Styles
1. Locate `src/styles/variables.css`
2. Modify color scheme:
```css
:root {
  --primary-color: #007bff;
  --secondary-color: #6c757d;
  --background-color: #ffffff;
}
```

### Updating Hero Section
1. Open `src/components/Header/Hero.js`
2. Modify content and styling:
```jsx
<div className="hero">
  <h1>Your Custom Heading</h1>
  <p>Your custom description</p>
</div>
```

## Deployment

### Standard Deployment
1. Build the project:
```bash
npm run build
```

2. Deploy to hosting service:
```bash
npm run deploy
```

### Custom Domain Setup
1. Purchase domain name
2. Add DNS records:
   - A Record: Point to your hosting IP
   - CNAME: www to your domain
3. Update site configuration in `config/site.js`

## Troubleshooting

### Common Issues
- **Images not loading**: Verify path in businesses.json
- **Categories not filtering**: Check category IDs match
- **Styling issues**: Clear cache and rebuild
- **Build errors**: Ensure all dependencies are installed

### Performance Optimization
- Compress images before upload
- Minimize CSS/JS files
- Enable caching
- Use CDN for assets

## Support
- Documentation: [docs.localbusinessdirectory.com](https://docs.localbusinessdirectory.com)
- Issues: [GitHub Issues](https://github.com/yourusername/local-business-directory/issues)
- Email: support@localbusinessdirectory.com
- Community: [Discord Server](https://discord.gg/localbusinessdirectory)

### Contributing
1. Fork the repository
2. Create feature branch
3. Commit changes
4. Push to branch
5. Create Pull Request

### License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

---
© 2023 Local Business Directory. All rights reserved.