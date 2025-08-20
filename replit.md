# Dollar Gift Cards Store

## Overview

A modern e-commerce web application for selling digital dollar gift cards with instant delivery. The platform allows customers to purchase gift cards ranging from $5 to $100 using local Bangladeshi mobile payment methods (Bkash and Nagad). Built with React frontend and Express.js backend, featuring a responsive design with dark mode support and smooth animations.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 19.1.1 with functional components and hooks
- **Routing**: React Router DOM for client-side navigation with animated page transitions
- **State Management**: Context API for cart management and local storage persistence
- **Styling**: Tailwind CSS 4.1.12 with custom design system and dark mode support
- **Animations**: Framer Motion for smooth transitions and micro-interactions
- **Build Tool**: React Scripts for development and production builds

### Backend Architecture
- **Framework**: Express.js 5.1.0 with RESTful API design
- **Middleware**: CORS for cross-origin requests, body-parser for request parsing
- **Static Serving**: Express static middleware for serving React build files
- **Data Layer**: Mock data structure for gift cards (no database currently implemented)
- **API Structure**: RESTful endpoints for products, orders, and newsletter subscriptions

### Design System
- **Color Scheme**: Brand colors with indigo/purple gradient theme, specialized payment method colors (pink for Bkash, orange for Nagad)
- **Typography**: Inter font family with consistent sizing scale
- **Components**: Reusable UI components (Button, ProductCard, TrustBadge) with consistent styling patterns
- **Responsive Design**: Mobile-first approach with breakpoint-based grid layouts
- **Dark Mode**: System preference detection with manual toggle and localStorage persistence

### Payment Integration Architecture
- **Payment Methods**: Bkash and Nagad mobile payment integration (manual process)
- **Order Flow**: Three-step process (select card → pay via mobile → receive via email)
- **Verification**: Transaction ID-based payment verification system
- **Delivery**: Email-based gift card code delivery after payment confirmation

### Performance Optimizations
- **Code Splitting**: React.lazy for route-based code splitting
- **Image Optimization**: Placeholder images with consistent sizing
- **CSS Optimization**: Tailwind CSS purging for smaller bundle sizes
- **Caching**: Browser caching for static assets and localStorage for user preferences

## External Dependencies

### Core Frontend Libraries
- **React 19.1.1**: Core frontend framework
- **React Router DOM 7.8.1**: Client-side routing
- **Framer Motion**: Animation library for smooth transitions
- **React Hook Form**: Form handling and validation

### Backend Dependencies
- **Express.js 5.1.0**: Web application framework
- **CORS 2.8.5**: Cross-origin resource sharing middleware
- **Body-parser 2.2.0**: Request body parsing middleware

### Styling and UI
- **Tailwind CSS 4.1.12**: Utility-first CSS framework
- **@tailwindcss/forms 0.5.10**: Form styling plugin
- **@tailwindcss/typography 0.5.16**: Typography plugin
- **PostCSS 8.5.6**: CSS post-processing
- **Autoprefixer 10.4.21**: CSS vendor prefixing

### Icon Library
- **Lucide React**: Modern icon library for UI elements

### Development Tools
- **React Scripts 5.0.1**: Build tools and development server

### Planned Integrations
- **Payment APIs**: Future integration with Bkash/Nagad official APIs for automated payment processing
- **Email Service**: Email delivery service for automated gift card code distribution
- **Database**: Potential database integration for order management and user accounts
- **Analytics**: Web analytics for tracking user behavior and conversion rates