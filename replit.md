# Overview

This is a minimal, professional timesheet calculator designed for ECATS (Electronic Contractor Time Accounting System) and similar time tracking systems. The application provides accurate decimal time conversion, handles complex time scenarios like overnight shifts, and includes features for break time deduction and late arrival tracking. Built as a Progressive Web App (PWA), it works entirely offline after the initial load and can be installed as a desktop application.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Framework**: React 18 with TypeScript for type safety and modern development
- **Build Tool**: Vite for fast development and optimized production builds
- **UI Components**: shadcn/ui component library built on Radix UI primitives
- **Styling**: Tailwind CSS with custom design system following Material Design principles
- **State Management**: React hooks (useState, useEffect) with localStorage for persistence
- **PWA Support**: Service Worker implementation for offline functionality and app installation

## Design System
- **Component Library**: Custom implementation using shadcn/ui with consistent styling
- **Theme System**: Dual light/dark mode support with automatic detection and manual override
- **Typography**: Inter font family via Google Fonts CDN
- **Color Palette**: Professional neutral colors with HSL-based CSS custom properties
- **Layout**: Single-column centered design with responsive breakpoints

## Data Management
- **Local Storage**: Persistent user preferences and timesheet data
- **No Backend Required**: Fully client-side application with no server dependencies
- **Form Handling**: React Hook Form with Zod validation schemas
- **State Persistence**: Automatic saving and loading of user inputs and settings

## Backend Architecture (Optional)
- **Express.js Server**: Minimal server setup for potential future features
- **Database Integration**: Drizzle ORM configured for PostgreSQL with schema definitions
- **Session Management**: connect-pg-simple for PostgreSQL session storage
- **API Structure**: RESTful endpoints with proper error handling and logging

## PWA Features
- **Service Worker**: Caches static assets and enables offline functionality
- **Web App Manifest**: Enables installation as native-like desktop application
- **Responsive Design**: Mobile-first approach with touch-friendly interfaces
- **Performance**: Optimized loading and minimal JavaScript bundle

## Development Workflow
- **TypeScript Configuration**: Strict type checking with path aliases for clean imports
- **Code Organization**: Feature-based file structure with shared utilities
- **Build Process**: Vite-based bundling with separate client and server builds
- **Component Architecture**: Reusable UI components with consistent prop interfaces

# External Dependencies

## Frontend Dependencies
- **React Ecosystem**: @tanstack/react-query for potential future data fetching
- **UI Components**: Comprehensive Radix UI component collection (@radix-ui/react-*)
- **Styling**: Tailwind CSS with PostCSS for processing
- **Icons**: Lucide React for consistent iconography
- **Utilities**: clsx and tailwind-merge for conditional styling, date-fns for date operations

## Development Tools
- **Build System**: Vite with React plugin and TypeScript support
- **Replit Integration**: Custom plugins for development environment integration
- **Error Handling**: Runtime error overlay for development debugging

## Potential Database Integration
- **ORM**: Drizzle ORM for type-safe database operations
- **Database**: PostgreSQL via Neon serverless (configured but not actively used)
- **Migrations**: Drizzle Kit for schema management and migrations

## PWA Infrastructure
- **Service Worker**: Custom implementation for caching strategies
- **Manifest**: Web app manifest for installation capabilities
- **Google Fonts**: External CDN for typography (Inter font family)

## Session Management (Server)
- **Express Session**: PostgreSQL-backed session storage
- **Authentication**: Basic user schema prepared for future authentication features