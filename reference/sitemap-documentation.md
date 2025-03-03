# MacLeod Jordan Website Sitemap Documentation

## Overview

This document provides detailed information about the MacLeod Jordan website sitemap structure. The sitemap serves as a blueprint for the website's architecture, navigation, and content organization. It is designed to help stakeholders understand the website structure and guide developers during implementation.

## Sitemap Structure

The website follows a hierarchical structure with the following main components:

### Main Navigation

1. **Home**
   - Primary landing page
   - Features company overview and highlighted content
   - Links to all main sections
   - Links to legal pages (Privacy Policy, Terms & Conditions)
   - Links to social media profiles

2. **About Us**
   - Company information and overview
   - **Subpages**:
     - History: Timeline and company milestones
     - Mission & Vision: Company values and future goals

3. **Services**
   - Overview of all engineering and consultancy services
   - **Subpages**:
     - Civil Engineering: Details of civil engineering services
     - Structural Engineering: Structural design and analysis services
     - Principal Designer: Design management services
     - Environmental Engineering: Environmental impact and sustainability services
     - Project Management: Project planning and execution services

4. **Projects**
   - Portfolio of completed and ongoing projects
   - Case studies and project highlights

5. **News**
   - Company news and announcements
   - Industry updates
   - Blog posts and articles

6. **Careers**
   - Job openings
   - Information about working at MacLeod Jordan
   - Application process

7. **Contact Us**
   - Contact information
   - Inquiry form
   - Office locations and map

### Secondary Pages

1. **Privacy Policy**
   - Information about data collection
   - Privacy practices and GDPR compliance
   - Cookie policy

2. **Terms & Conditions**
   - Legal terms for website usage
   - Intellectual property information
   - Disclaimer and limitations

### Social Media Integration

- Links to company profiles on:
  - Facebook
  - Twitter
  - LinkedIn
  - Instagram

## Implementation Guidelines

### Navigation Structure

- **Primary Navigation**: Implement as a horizontal menu at the top of all pages
- **Secondary Navigation**: Include in the footer area of all pages
- **Social Media Links**: Display in both header and footer areas

### URL Structure

Follow this URL structure for consistency:

- Home: `/`
- About Us: `/about`
  - History: `/about/history`
  - Mission & Vision: `/about/mission-vision`
- Services: `/services`
  - Civil Engineering: `/services/civil-engineering`
  - Structural Engineering: `/services/structural-engineering`
  - Principal Designer: `/services/principal-designer`
  - Environmental Engineering: `/services/environmental-engineering`
  - Project Management: `/services/project-management`
- Projects: `/projects`
- News: `/news`
- Careers: `/careers`
- Contact Us: `/contact`
- Privacy Policy: `/privacy-policy`
- Terms & Conditions: `/terms-conditions`

### Responsive Design Considerations

- Ensure all pages are fully responsive for mobile, tablet, and desktop
- On mobile devices, convert the main navigation to a hamburger menu
- Maintain hierarchy and relationships between pages in mobile view

### Content Requirements

Each page should include:

- Clear heading structure (H1, H2, H3)
- Relevant images and media
- Call-to-action elements
- Internal links to related content
- Consistent branding elements

## Technical Specifications

### Recommended Technologies

- **Frontend Framework**: Next.js or similar React-based framework
- **Styling**: CSS modules or styled-components
- **CMS Integration**: Consider Contentful or Sanity for content management
- **Analytics**: Google Analytics or similar for tracking user behavior

### SEO Considerations

- Implement proper meta tags on all pages
- Create an XML sitemap for search engines
- Ensure all pages have unique titles and descriptions
- Implement schema markup for rich snippets

## Maintenance Plan

- Regular content updates for News section (minimum monthly)
- Quarterly review of all service pages for accuracy
- Annual comprehensive review of the entire site structure
- Ongoing performance optimization

---

*This documentation was prepared based on the sitemap created by Ashley Milne & Steven Brown - Sitecut Ltd. on 29/06/22.* 