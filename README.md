# Collection Carousel – Shopify Technical Assessment

Custom **Collection Carousel** section for Shopify collection pages, built following **Online Store 2.0** standards and Dawn architecture.

---

## Overview

This project implements a reusable carousel section that can be added to collection templates via the Shopify Theme Editor.  
It is designed to be lightweight, configurable, and fully compatible with Shopify’s native workflows.

---

## How to Test (Shopify CLI – Recommended)

### Prerequisites
- Shopify CLI
- Shopify Partner account with access to a development store

### Steps

```bash
git clone https://github.com/YOUR-USERNAME/shopify-carousel-task.git
cd shopify-carousel-task
shopify theme dev --store=your-store.myshopify.com
```

The theme will open automatically in the browser with live reload enabled.

### Adding the Section
1. Open the **Theme Customizer**
2. Navigate to any **collection page**
3. Click **Add section**
4. Select **Collection Carousel**
5. Configure slides using the settings panel

---

## Library Choice: Swiper.js

### Why Swiper?
- ~45 KB gzipped via CDN
- Touch and swipe support
- Responsive breakpoints
- Keyboard navigation
- Accessibility features
- Pagination and navigation controls
- Loop support
- No build step required

**Conclusion:**  
Swiper provides the best balance between bundle size, accessibility, reliability, and development speed for this use case.

---

## Technical Notes

- Built following **Shopify OS 2.0** and **Dawn** architecture
- Written in **Liquid + Vanilla JavaScript**
- No jQuery or external build tooling
- Fully compatible with the Shopify Theme Editor
- Gracefully handles edge cases (0, 1, or multiple slides)
