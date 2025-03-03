# website planner prompt

You are an AI task planner responsible for breaking down a complex web application development project into manageable steps.

Your goal is to create a detailed, step-by-step plan that will guide the code generation process for building a fully functional web application based on a provided technical specification.

First, carefully review the following inputs:

<project_request>
# Implementation Plan for Structural/Civil Engineering Consultancy Website

## Project Name
MacLeod Jordan Engineering Consultancy Website

## Project Description
A modern, interactive website for a structural/civil engineering consultancy that showcases the firm's expertise, projects, and capabilities. The website will feature interactive 3D models exported from Revit and Twinmotion to demonstrate structural designs and engineering solutions, built with Next.js and Shadcn UI for a polished, professional appearance.

## Target Audience
- Architecture firms seeking engineering partners
- Property developers and construction companies
- Government agencies and municipalities 
- Industrial and commercial clients requiring structural assessments
- Other engineers and industry professionals

## Core Website Structure
- [x] Step 1: Setup project foundation
  - **Task**: ✅ Next.js project with TypeScript, folder structure, and key dependencies already set up
  - **Files**: ✅ Already configured
    - `package.json`: Project dependencies
    - `tsconfig.json`: TypeScript configuration
    - `next.config.js`: Next.js configuration
    - `README.md`: Project documentation

- [x] Step 2: Set up Shadcn UI
  - **Task**: ✅ Shadcn UI with Tailwind CSS already configured
  - **Files**: ✅ Already configured
    - `components.json`: Shadcn configuration
    - `tailwind.config.js`: Tailwind CSS configuration
    - `app/globals.css`: Global styles
    - `lib/utils.ts`: Utility functions for Shadcn

- [x] Step 3: Create basic layout and navigation with Shadcn components
  - **Task**: ✅ Basic layout components already implemented
  - **Files**: ✅ Already configured
    - `app/layout.tsx`: Root layout
    - `components/header.tsx`: Main navigation
    - `app/(marketing)/layout.tsx`: Marketing layout
    - `app/(marketing)/page.tsx`: Homepage

## 3D Visualization Features (To Be Implemented)
- [ ] Step 4: Install and set up 3D libraries
  - **Task**: Install Three.js and related libraries for 3D visualization
  - **Files**:
    - Update `package.json` to include:
      - three
      - @react-three/fiber
      - @react-three/drei
      - @types/three (dev dependency)

- [ ] Step 5: Implement 3D model viewer infrastructure
  - **Task**: Set up Three.js or similar 3D engine, create viewer component, and implement basic controls
  - **Files**:
    - `components/3d/ModelViewer.tsx`: Core 3D viewer component
    - `lib/3d/controls.ts`: Camera and interaction controls
    - `components/ui/model-viewer-card.tsx`: Shadcn-styled card for 3D viewer

- [ ] Step 6: Develop Revit model integration
  - **Task**: Create pipeline for importing and displaying Revit models (via IFC or converted formats)
  - **Files**:
    - `lib/3d/importers/revit.ts`: Revit model loading logic
    - `components/3d/RevitModelViewer.tsx`: Specialized viewer for Revit models

- [ ] Step 7: Develop Twinmotion visualization integration
  - **Task**: Create components for displaying Twinmotion exports and panoramic renders
  - **Files**:
    - `lib/3d/importers/twinmotion.ts`: Twinmotion content loading
    - `components/3d/PanoramaViewer.tsx`: 360° panorama viewer

## Content Pages (Partially Implemented)
- [ ] Step 8: Enhance homepage with engineering-specific content
  - **Task**: Customize existing hero section and features for engineering focus
  - **Files**:
    - `components/landing/hero.tsx`: Update hero section with engineering messaging
    - `components/landing/features.tsx`: Update features with engineering services
    - `components/landing/projects-preview.tsx`: Add featured projects section

- [ ] Step 9: Implement services pages
  - **Task**: Create pages detailing different engineering services with relevant 3D examples
  - **Files**:
    - `app/(marketing)/services/page.tsx`: Services overview
    - `app/(marketing)/services/[service]/page.tsx`: Individual service detail pages
    - `components/services/ServiceCard.tsx`: Shadcn card component for services

- [ ] Step 10: Develop projects portfolio section
  - **Task**: Create project showcase with filtering, details, and 3D model integration
  - **Files**:
    - `app/(marketing)/projects/page.tsx`: Projects gallery
    - `app/(marketing)/projects/[slug]/page.tsx`: Individual project detail page
    - `components/projects/ProjectGallery.tsx`: Project browsing component with Shadcn tabs and filters
    - `components/projects/ProjectModelViewer.tsx`: Project-specific 3D viewer

- [ ] Step 11: Enhance about and team section
  - **Task**: Expand existing about page with company profile, team member profiles, and company values
  - **Files**:
    - `app/(marketing)/about/page.tsx`: Update about page
    - `components/about/TeamGrid.tsx`: Team member display with Shadcn avatars and cards
    - `components/about/CompanyValues.tsx`: Company values section

- [ ] Step 12: Enhance contact and inquiry forms
  - **Task**: Expand existing contact page with engineering-specific forms
  - **Files**:
    - `app/(marketing)/contact/page.tsx`: Update contact page
    - `components/forms/ContactForm.tsx`: Engineering-specific contact form
    - `app/api/contact/route.ts`: Contact form API endpoint

## Technical Features (Partially Implemented)
- [ ] Step 13: Set up database schema for projects and case studies
  - **Task**: Create database schema for storing project information
  - **Files**:
    - `db/schema/projects-schema.ts`: Project database schema
    - `db/schema/services-schema.ts`: Services database schema
    - `actions/db/projects-actions.ts`: Project database actions
    - `actions/db/services-actions.ts`: Services database actions

- [ ] Step 14: Develop performance optimizations for 3D content
  - **Task**: Implement lazy loading, progressive enhancement, and fallbacks for 3D models
  - **Files**:
    - `components/3d/LazyModelLoader.tsx`: Lazy loading wrapper
    - `lib/3d/optimization.ts`: Model optimization utilities
    - `components/ui/model-skeleton.tsx`: Custom skeleton loaders for 3D content

- [ ] Step 15: Implement animations and transitions
  - **Task**: Add scroll-based animations and page transitions for enhanced UX
  - **Files**:
    - `components/animation/ScrollAnimation.tsx`: Scroll-based animation
    - `lib/animation/transitions.ts`: Page transition utilities
    - `components/ui/animated-card.tsx`: Custom animated Shadcn card component

## Engineering-Specific Features
- [ ] Step 16: Create structural calculation demonstrations
  - **Task**: Implement interactive demonstrations of structural calculations
  - **Files**:
    - `components/engineering/BeamCalculator.tsx`: Interactive beam calculator
    - `components/engineering/StructuralDiagram.tsx`: Interactive structural diagrams
    - `lib/engineering/calculations.ts`: Engineering calculation utilities

- [ ] Step 17: Implement project timeline visualization
  - **Task**: Create interactive timeline for project phases
  - **Files**:
    - `components/projects/ProjectTimeline.tsx`: Project timeline component
    - `lib/projects/timeline.ts`: Timeline utilities

- [ ] Step 18: Create case study template
  - **Task**: Develop detailed case study template with technical specifications
  - **Files**:
    - `app/(marketing)/case-studies/[slug]/page.tsx`: Case study page template
    - `components/case-studies/CaseStudyHeader.tsx`: Case study header
    - `components/case-studies/TechnicalSpecs.tsx`: Technical specifications component

## Deployment and Analytics (Already Configured)
- [x] Step 19: Analytics setup
  - **Task**: ✅ PostHog analytics already configured
  - **Files**: ✅ Already configured

- [x] Step 20: Payment processing
  - **Task**: ✅ Stripe integration already configured
  - **Files**: ✅ Already configured

## Additional Considerations
- Browser compatibility for 3D elements
- Fallback options for devices that can't handle complex 3D rendering
- Loading strategies for heavy 3D models
- Caching and optimization for repeat visitors
- Accessibility considerations, including alternatives to 3D content
- Consistent application of Shadcn UI design language across custom components
</project_request>

After reviewing these inputs, your task is to create a comprehensive, detailed plan for implementing the web application.

Before creating the final plan, analyze the inputs and plan your approach. Wrap your thought process in <brainstorming> tags.

Break down the development process into small, manageable steps that can be executed sequentially by a code generation AI.

Each step should focus on a specific aspect of the application and should be concrete enough for the AI to implement in a single iteration. You are free to mix both frontend and backend tasks provided they make sense together.

When creating your plan, follow these guidelines:

1. Start with the core project structure and essential configurations.
2. Progress through database schema, server actions, and API routes.
3. Move on to shared components and layouts.
4. Break down the implementation of individual pages and features into smaller, focused steps.
5. Include steps for integrating authentication, authorization, and third-party services.
6. Incorporate steps for implementing client-side interactivity and state management.
7. Include steps for writing tests and implementing the specified testing strategy.
8. Ensure that each step builds upon the previous ones in a logical manner.

Present your plan using the following markdown-based format. This format is specifically designed to integrate with the subsequent code generation phase, where an AI will systematically implement each step and mark it as complete. Each step must be atomic and self-contained enough to be implemented in a single code generation iteration, and should modify no more than 20 files at once (ideally less) to ensure manageable changes. Make sure to include any instructions the user should follow for things you can't do like installing libraries, updating configurations on services, etc (Ex: Running a SQL script for storage bucket RLS policies in the Supabase editor).

```md
# Implementation Plan

## [Section Name]
- [ ] Step 1: [Brief title]
  - **Task**: [Detailed explanation of what needs to be implemented]
  - **Files**: [Maximum of 20 files, ideally less]
    - `path/to/file1.ts`: [Description of changes]
  - **Step Dependencies**: [Step Dependencies]
  - **User Instructions**: [Instructions for User]

[Additional steps...]
```

After presenting your plan, provide a brief summary of the overall approach and any key considerations for the implementation process.

Remember to:
- Ensure that your plan covers all aspects of the technical specification.
- Break down complex features into smaller, manageable tasks.
- Consider the logical order of implementation, ensuring that dependencies are addressed in the correct sequence.
- Include steps for error handling, data validation, and edge case management.

Begin your response with your brainstorming, then proceed to the creation your detailed implementation plan for the web application based on the provided specification.

Once you are done, we will pass this specification to the AI code generation system. 