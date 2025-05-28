# Dropshipping Store User Guide

## Overview
This document provides instructions for managing your free dropshipping online store built with Jekyll. The store is designed to be hosted on GitHub Pages or Netlify at zero cost, meeting your budget requirements while providing all essential e-commerce functionality.

## Store Structure
Your dropshipping store includes:
- Responsive design for both mobile and desktop
- Product catalog with category filtering
- Shopping cart functionality
- Checkout system with PayPal integration
- Shipping options configuration
- Dropshipping-ready product structure with supplier IDs and SKUs

## How to Add/Edit Products
1. Navigate to the `_products` folder
2. Create a new Markdown file for each product (use existing files as templates)
3. Each product file should include:
   - Layout: product
   - Title: Product name
   - ID: Unique identifier
   - Price: Product price
   - Description: Detailed product description
   - Category: Product category for filtering
   - Image: Path to product image
   - Supplier_id: Your dropshipping supplier identifier
   - Supplier_sku: The SKU used by your supplier

## How to Update Product Data
The main product data is stored in `_data/products.json`. Update this file to:
- Change product information
- Add new products
- Remove discontinued products
- Update pricing

## Managing Orders
When a customer completes checkout:
1. Order details are processed through PayPal
2. You'll receive notification of the order
3. Forward the order details to your dropshipping supplier using the supplier_id and supplier_sku

## Customizing Your Store
- **Theme**: Edit files in `_layouts` and `_includes` folders
- **Styles**: Modify CSS in `assets/css/main.css`
- **Homepage**: Edit `index.html` to change featured products and content
- **Store Name/Logo**: Update in `_includes/header.html`

## Deployment Instructions
### GitHub Pages (Recommended)
1. Create a GitHub account if you don't have one
2. Create a new repository
3. Push all store files to the repository
4. Enable GitHub Pages in repository settings
5. Your store will be available at `https://yourusername.github.io/repository-name/`

### Netlify (Alternative)
1. Create a Netlify account
2. Connect to your GitHub repository or upload the store files directly
3. Configure build settings (not required for pre-built sites)
4. Your store will be available at a Netlify subdomain with option to add a custom domain

## Technical Support
This store is designed to be self-maintained, but if you need assistance:
- Review the code comments for guidance
- Check Jekyll documentation for static site questions
- For dropshipping workflow questions, consult with your suppliers

## Updating Your Store
To make changes to your store after deployment:
1. Edit the relevant files locally
2. Test changes using `bundle exec jekyll serve`
3. Commit and push changes to GitHub (if using GitHub Pages)
4. For Netlify, changes will automatically deploy when pushed to the connected repository

## Security Considerations
- This is a static site with client-side processing
- Payment processing is handled securely through PayPal
- No customer data is stored on the server
- Regularly update your GitHub/Netlify account passwords

## Limitations
- As a static site, advanced dynamic features require external services
- Order management is manual (forwarding to suppliers)
- Inventory synchronization with suppliers must be done manually

## Future Enhancements
Consider these paid upgrades when your business grows:
- Custom domain name
- Advanced inventory management
- Automated order processing
- Customer accounts and loyalty programs
