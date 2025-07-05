# Travel Billing System - Replit Setup Guide

## Overview

This is a comprehensive Travel Billing System web application built for managing travel-related expenses, invoices, GPS tracking, and client management. The system provides a modern interface for travel service providers to handle their billing operations, track routes, manage expenses, and generate professional invoices.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **Routing**: Wouter (lightweight React router)
- **State Management**: TanStack Query (React Query) for server state
- **UI Components**: Radix UI primitives with custom shadcn/ui components
- **Styling**: Tailwind CSS with CSS variables for theming
- **Build Tool**: Vite for fast development and optimized production builds

### Backend Architecture
- **Runtime**: Node.js with Express.js
- **Language**: TypeScript with ES modules
- **Database**: PostgreSQL with Drizzle ORM
- **Database Provider**: Neon Database (serverless PostgreSQL)
- **File Uploads**: Multer middleware for receipt/bill uploads
- **Session Management**: Express sessions with PostgreSQL store

### Key Components

#### Database Layer
- **ORM**: Drizzle ORM with type-safe queries
- **Schema Definition**: Centralized in `shared/schema.ts`
- **Migrations**: Managed through Drizzle Kit
- **Database Tables**:
  - `clients`: Company and contact information
  - `invoices`: Invoice details with GST calculations
  - `expenses`: Travel expense tracking with receipt uploads
  - `trips`: GPS route tracking with distance calculation

#### API Structure
- RESTful API endpoints under `/api` namespace
- CRUD operations for all major entities
- File upload endpoints for expense receipts
- Dashboard statistics aggregation
- Real-time data fetching with React Query

#### Authentication & Security
- Session-based authentication (ready for implementation)
- File upload validation and size limits
- CORS and security headers configured
- Input validation using Zod schemas

## Data Flow

1. **Client Management**: Add/edit client information including GST details
2. **Trip Planning**: GPS-based route tracking with distance calculation
3. **Expense Tracking**: Record expenses with receipt uploads and categorization
4. **Invoice Generation**: Create professional invoices with GST calculations
5. **PDF Export**: Generate and download invoices as PDF documents
6. **Dashboard Analytics**: Real-time statistics and recent activity monitoring

## External Dependencies

### Production Dependencies
- **@neondatabase/serverless**: Serverless PostgreSQL connection
- **drizzle-orm**: Type-safe database operations
- **@tanstack/react-query**: Server state management
- **@radix-ui/***: Accessible UI component primitives
- **react-hook-form**: Form state management
- **jspdf**: PDF generation for invoices
- **multer**: File upload handling
- **date-fns**: Date manipulation utilities

### Development Dependencies
- **vite**: Build tool and development server
- **typescript**: Type checking and compilation
- **tailwindcss**: Utility-first CSS framework
- **drizzle-kit**: Database migration tool

### Third-Party Integrations
- **Google Maps API**: GPS tracking and route calculation (configured but needs API key)
- **WhatsApp API**: Invoice sharing capabilities (planned)
- **Email Services**: Automated invoice delivery (planned)

## Deployment Strategy

### Development Environment
- Vite development server with HMR
- In-memory storage fallback for development
- Replit-specific configurations and plugins
- Runtime error overlay for debugging

### Production Build
- **Frontend**: Vite production build with code splitting
- **Backend**: ESBuild compilation to single bundle
- **Database**: Neon Database with connection pooling
- **File Storage**: Local uploads directory (can be extended to cloud storage)

### Environment Configuration
- `DATABASE_URL`: PostgreSQL connection string
- `NODE_ENV`: Environment mode (development/production)
- File upload limits and allowed types configurable

### Build Scripts
- `npm run dev`: Development server with watch mode
- `npm run build`: Production build for both frontend and backend
- `npm run start`: Production server startup
- `npm run db:push`: Database schema synchronization

## Changelog
- July 05, 2025. Initial setup

## User Preferences

Preferred communication style: Simple, everyday language.