# RepairAI - AI-Powered Hardware Repair Platform

A comprehensive repair service platform that connects device owners with AI diagnosis and certified technicians.

## Features

### For Device Owners
- **AI Diagnosis**: Upload images and descriptions to get instant AI-powered diagnosis
- **DIY Repair Guides**: Step-by-step instructions for common issues
- **Technician Booking**: Connect with certified repair technicians when needed
- **Repair Tracking**: Real-time status updates for all repair requests
- **Cost Savings**: Try DIY fixes before escalating to paid services

### For Technicians
- **Service Management**: Accept and manage repair jobs
- **Job Requests**: View detailed repair information and customer needs
- **Status Updates**: Update job progress from pending to completed
- **Profile Setup**: Configure specializations, rates, and availability

## Technology Stack

- **Frontend**: React with TypeScript, Tailwind CSS
- **Backend**: Supabase (PostgreSQL, Authentication, Storage)
- **Icons**: Lucide React
- **Build Tool**: Vite

## Database Schema

### Tables
- `user_profiles` - User account information with role separation
- `technician_profiles` - Technician specializations, rates, and ratings
- `repairs` - Device repair requests with AI diagnosis
- `bookings` - Connections between users and technicians
- `repair_updates` - Timeline tracking for repairs

## User Journeys

### Device Owner Journey
1. Land on homepage → See value proposition
2. Sign up as device owner
3. Access dashboard with control hub
4. Create new repair request (upload image + description)
5. Receive AI diagnosis with DIY instructions
6. Either mark as fixed OR escalate to technician
7. Book technician with scheduling
8. Track repair status in real-time

### Technician Journey
1. Sign up as technician
2. Complete profile setup (specializations, rates, location)
3. View incoming job requests
4. Accept jobs and view repair details
5. Update job status (accepted → in progress → completed)
6. Build reputation through completed jobs

## Key Design Decisions

### Role Separation
Users and technicians have completely separate workflows and dashboards for security and usability.

### AI Diagnosis as Primary Feature
The platform prioritizes AI diagnosis to reduce costs and promote eco-friendly repairs through device longevity.

### Escalation System
DIY fixes are attempted first, with professional help available as a fallback, creating a hybrid model.

### Status Tracking
All repairs have detailed tracking to build trust and transparency.

## Getting Started

1. Install dependencies:
   ```bash
   npm install
   ```

2. Environment variables are pre-configured in `.env`

3. Run development server:
   ```bash
   npm run dev
   ```

4. Build for production:
   ```bash
   npm run build
   ```

## Security Features

- Row Level Security (RLS) on all database tables
- Role-based access control
- Secure image upload with storage policies
- Authentication state management
- Input validation and sanitization

## Future Enhancements

- Real-time notifications for status updates
- In-app messaging between users and technicians
- Payment processing integration
- Rating and review system
- Advanced AI models for better diagnosis accuracy
- Multi-language support
