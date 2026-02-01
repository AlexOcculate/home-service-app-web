# Technology Stack

This document provides an overview of the technology stack and programming languages used in the Home Service App Web project.

## Programming Languages

- **JavaScript** - Primary programming language for both frontend and backend
- **CSS** - Styling and layout
- **HTML** - Markup (via JSX/React)

## Core Framework

- **[Next.js](https://nextjs.org/) 14.1.0** - React framework with server-side rendering, routing, and API routes
  - Server Components (RSC enabled)
  - App Router architecture
  - Built-in API routes

## Frontend Technologies

### UI Framework & Libraries

- **[React](https://react.dev/) 18** - JavaScript library for building user interfaces
- **[React DOM](https://react.dev/) 18** - React rendering for web applications

### UI Components & Design System

- **[Radix UI](https://www.radix-ui.com/)** - Headless UI component library
  - `@radix-ui/react-alert-dialog` - Alert dialog components
  - `@radix-ui/react-dialog` - Modal dialog components
  - `@radix-ui/react-dropdown-menu` - Dropdown menu components
  - `@radix-ui/react-slot` - Slot components for composition
  - `@radix-ui/react-tabs` - Tab components
- **[shadcn/ui](https://ui.shadcn.com/)** - Re-usable components built with Radix UI and Tailwind CSS

### Styling

- **[Tailwind CSS](https://tailwindcss.com/) 3.3.0** - Utility-first CSS framework
- **[PostCSS](https://postcss.org/) 8** - CSS processing tool
- **[Autoprefixer](https://github.com/postcss/autoprefixer) 10** - Automatic vendor prefix handling
- **tailwindcss-animate** - Tailwind CSS plugin for animations
- **tailwind-merge** - Utility for merging Tailwind CSS classes
- **class-variance-authority** - CSS variant management

### Icons & Visual Elements

- **[Lucide React](https://lucide.dev/) 0.343.0** - Icon library for React

### State Management & Theming

- **[next-themes](https://github.com/pacocoursey/next-themes) 0.2.1** - Theme management for Next.js (dark mode support)

### Date & Time Handling

- **[date-fns](https://date-fns.org/) 3.3.1** - Modern JavaScript date utility library
- **[Moment.js](https://momentjs.com/) 2.30.1** - JavaScript date library for parsing, validating, and formatting dates
- **[react-day-picker](https://react-day-picker.js.org/) 8.10.0** - Date picker component for React

### Utilities

- **clsx** - Utility for constructing className strings conditionally
- **[Sonner](https://sonner.emilkowal.ski/) 1.4.3** - Toast notification library for React

## Backend & API

### Authentication

- **[NextAuth.js](https://next-auth.js.org/) 4.24.6** - Authentication solution for Next.js applications
- **Descope** - OAuth provider integration for authentication

### Data Fetching & API Communication

- **[GraphQL](https://graphql.org/) 16.8.1** - Query language for APIs
- **[graphql-request](https://github.com/jasonkuhrt/graphql-request) 6.1.0** - GraphQL client for making API requests
- **[Hygraph](https://hygraph.com/)** - Headless CMS with GraphQL API (formerly GraphCMS)

## Build Tools & Configuration

- **[Node.js](https://nodejs.org/)** - JavaScript runtime environment
- **npm** - Package manager
- **jsconfig.json** - JavaScript compiler configuration with path aliases

## Development Tools

- **ESLint** - Code linting (via `next lint`)
- **Git** - Version control

## Hosting & Deployment

The application is designed to be deployed on:
- **[Vercel](https://vercel.com/)** - Recommended hosting platform (optimized for Next.js)

## Architecture Patterns

- **Server-Side Rendering (SSR)** - Next.js server components
- **Client-Side Rendering (CSR)** - React client components
- **API Routes** - Built-in Next.js API handling
- **Component-Based Architecture** - Modular React components
- **Headless CMS** - GraphQL-based content management with Hygraph

## File Structure

- `/app` - Next.js App Router structure
  - `(routes)` - Route groups
  - `_components` - Private/shared components
  - `_services` - API services and utilities
  - `api` - API route handlers
- `/components` - Reusable UI components (shadcn/ui)
- `/lib` - Utility functions and helpers
- `/public` - Static assets

## Configuration Files

- `next.config.mjs` - Next.js configuration
- `tailwind.config.js` - Tailwind CSS configuration
- `postcss.config.js` - PostCSS configuration
- `components.json` - shadcn/ui configuration
- `jsconfig.json` - JavaScript/Path configuration
- `package.json` - Project dependencies and scripts
