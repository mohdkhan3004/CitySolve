# CitySolve - Community Complaint Management System

## Overview
CitySolve is a comprehensive web application for managing community complaints and issues. Citizens can submit complaints about municipal problems (potholes, garbage, infrastructure, etc.) while administrators can track, manage, and resolve these issues through a dedicated admin dashboard.

## Project Architecture
- **Frontend**: React 18.3 with Wouter for routing, TailwindCSS for styling, React Query for data fetching
- **Backend**: Express.js with TypeScript, providing REST API endpoints
- **Database**: Neon PostgreSQL with Drizzle ORM for type-safe database operations
- **Authentication**: Session-based admin authentication with bcrypt password hashing

## Database Schema
- `complaints`: Main complaint records with location, status, priority, and reporting details
- `admin_users`: Administrative users with role-based access
- `users`: Basic user management (legacy, can be expanded)

## Recent Changes (January 31, 2025)
- ✅ Successfully migrated from Bolt/Supabase to Replit/Neon PostgreSQL
- ✅ Replaced React Router with Wouter for routing
- ✅ Implemented server-side PostgreSQL queries with Drizzle ORM
- ✅ Created comprehensive REST API endpoints for complaints and admin management
- ✅ Migrated client-side data fetching to React Query
- ✅ Removed all Supabase dependencies
- ✅ Created default admin user (citysolve1122@gmail.com / 1122)

## API Endpoints
- `GET /api/complaints` - Fetch complaints with filtering
- `POST /api/complaints` - Create new complaint
- `GET /api/complaints/:id` - Get specific complaint
- `PATCH /api/complaints/:id/status` - Update complaint status
- `POST /api/admin/login` - Admin authentication
- `GET /api/complaints/stats` - Dashboard statistics

## Admin Credentials
- Email: citysolve1122@gmail.com
- Password: 1122

## Key Features
- Citizen complaint submission with location mapping
- Real-time complaint tracking
- Admin dashboard with filtering and status updates
- Responsive design for mobile and desktop
- Secure admin authentication

## User Preferences
- Prefers clean, modern UI with gradient backgrounds
- Uses professional color scheme (blues, yellows for branding)
- Implements real-time updates for admin dashboard
- Maintains separation between citizen and admin interfaces