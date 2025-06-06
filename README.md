# Vibe - Social Commerce Platform

A cutting-edge social commerce platform that combines e-commerce with interactive social media experiences, powered by advanced AI technologies for dynamic product discovery and engagement.

## 🚀 Features

### Core Functionality
- **Dual-Experience Home Page** - Content reels and shopping reels
- **TikTok/Instagram Reels-style** product videos with social interactions
- **Multi-vendor Marketplace** with seller and creator accounts
- **Real-time Social Features** - likes, comments, shares, follows
- **AI-Powered Content Creation** using OpenAI integration
- **Virtual Try-On** feature for fashion products
- **Advanced Search** with AI assistance and niche tagging

### User Accounts
- **Regular Users** - Browse, shop, and engage with content
- **Content Creators** - Upload videos/images with monetization
- **Sellers** - Manage products, reels, analytics, and payouts
- **Admin Dashboard** - Complete platform management

### Commerce Features
- **Product Catalog Management** with multiple images and videos
- **Shopping Cart & Checkout** with multiple payment options
- **Order Tracking** with real-time updates
- **Wishlist & Favorites** functionality
- **Wallet System** with UPI payment support
- **Seller Payouts** using RazorpayX integration

### Technical Features
- **Mobile-First Design** with responsive UI
- **Real-time Notifications** using Socket.io
- **Database Integration** with PostgreSQL and Drizzle ORM
- **Payment Gateways** - Razorpay, Stripe, PayPal support
- **Shipping Integration** - Shiprocket and Rapido
- **Email Services** with automated notifications
- **Push Notifications** for mobile applications

## 🛠 Tech Stack

### Frontend
- **React 18** with TypeScript
- **Vite** for fast development and building
- **Tailwind CSS** for styling
- **Shadcn/UI** components
- **Wouter** for routing
- **TanStack Query** for data fetching
- **Framer Motion** for animations
- **React Hook Form** with Zod validation

### Backend
- **Express.js** with TypeScript
- **PostgreSQL** database
- **Drizzle ORM** for database operations
- **Passport.js** for authentication
- **Socket.io** for real-time features
- **Multer** for file uploads
- **Node.js** runtime

### Integrations
- **OpenAI API** for AI-powered features
- **Firebase** for push notifications
- **Razorpay** for Indian payments
- **Stripe** for international payments
- **PayPal** for global transactions
- **Shiprocket** for shipping
- **SendGrid** for email services

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ and npm
- PostgreSQL database
- Required API keys (see Environment Variables)

### Installation

1. **Clone and Install**
```bash
git clone <your-repo>
cd vibe-app
npm install
```

2. **Database Setup**
```bash
# Create PostgreSQL database
npm run db:push
```

3. **Environment Variables**
Create a `.env` file in the root directory:

```env
# Database
DATABASE_URL="postgresql://username:password@localhost:5432/vibe"

# Authentication
SESSION_SECRET="your-session-secret"

# OpenAI (for AI features)
OPENAI_API_KEY="sk-your-openai-key"

# Payment Gateways
RAZORPAY_KEY_ID="rzp_test_your-key"
RAZORPAY_KEY_SECRET="your-razorpay-secret"
STRIPE_SECRET_KEY="sk_test_your-stripe-key"
VITE_STRIPE_PUBLIC_KEY="pk_test_your-stripe-public-key"

# Firebase (for push notifications)
FIREBASE_PROJECT_ID="your-project-id"
FIREBASE_API_KEY="your-api-key"
FIREBASE_APP_ID="your-app-id"
FIREBASE_MESSAGING_SENDER_ID="your-sender-id"
FIREBASE_VAPID_KEY="your-vapid-key"

# Email Service
SENDGRID_API_KEY="SG.your-sendgrid-key"

# Shipping
SHIPROCKET_API_KEY="your-shiprocket-key"
RAPIDO_API_KEY="your-rapido-key"

# Domain Configuration
DOMAIN_NAME="vibe-app.co.in"
```

4. **Run Development Server**
```bash
npm run dev
```

The app will be available at `http://localhost:5000`

## 📱 Mobile App Development

The codebase is ready for mobile app development using:
- **React Native** (recommended)
- **Expo** for rapid development
- **Progressive Web App** (PWA) capabilities

### PWA Setup
The app includes service worker configuration for offline functionality and app-like experience on mobile devices.

## 🏗 Architecture

### Frontend Structure
```
client/
├── src/
│   ├── components/     # Reusable UI components
│   ├── pages/         # Page components
│   ├── hooks/         # Custom React hooks
│   ├── lib/           # Utility functions
│   ├── context/       # React context providers
│   └── assets/        # Static assets
```

### Backend Structure
```
server/
├── routes.ts          # API route definitions
├── db.ts             # Database configuration
├── storage.ts        # Data access layer
├── auth.ts           # Authentication logic
├── services/         # External service integrations
└── utils/            # Utility functions
```

### Shared
```
shared/
└── schema.ts         # Database schema and types
```

## 🔐 Authentication

The app supports multiple authentication methods:
- **Email/Password** with secure password hashing
- **Social Login** ready for Google, Facebook integration
- **Role-based Access** (User, Creator, Seller, Admin)
- **Session Management** with secure cookies

## 💾 Database Schema

Key database tables:
- **users** - User accounts and profiles
- **products** - Product catalog
- **orders** - Purchase orders and tracking
- **reels** - Video content and metadata
- **notifications** - Real-time notification system
- **wallet_transactions** - Payment and wallet operations

## 🎨 UI/UX Features

- **Mobile-First Design** optimized for touch interfaces
- **Dark/Light Mode** support
- **Responsive Grid Layouts** for all screen sizes
- **Smooth Animations** using Framer Motion
- **Accessibility** features with proper ARIA labels
- **Professional Color Scheme** with consistent branding

## 🔧 Development

### Available Scripts
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run db:push` - Update database schema
- `npm run db:studio` - Open database studio
- `npm run type-check` - Run TypeScript checks

### Code Quality
- **TypeScript** for type safety
- **ESLint** for code linting
- **Prettier** for code formatting
- **Zod** for runtime validation

## 🚀 Deployment

### Production Deployment
1. **Build the application**
```bash
npm run build
```

2. **Environment Setup**
- Set all production environment variables
- Configure PostgreSQL database
- Set up CDN for static assets

3. **Deploy Options**
- **Vercel** (recommended for frontend)
- **Railway/Render** (for full-stack)
- **AWS/GCP/Azure** (for enterprise)

### Docker Support
The app includes Docker configuration for containerized deployment.

## 📊 Analytics & Monitoring

- **User Analytics** tracking
- **Seller Performance** metrics
- **Real-time Dashboards** for all user types
- **Revenue Tracking** and reporting
- **Error Monitoring** and logging

## 🔒 Security Features

- **Input Validation** with Zod schemas
- **SQL Injection Protection** via Drizzle ORM
- **XSS Prevention** with proper sanitization
- **CSRF Protection** with secure tokens
- **Rate Limiting** on API endpoints
- **Secure File Uploads** with validation

## 🌟 Advanced Features

### AI Integration
- **Content Generation** using OpenAI
- **Smart Product Recommendations**
- **Automated Content Moderation**
- **Intelligent Search** with semantic matching

### Social Commerce
- **Influencer Marketplace** connecting creators with brands
- **Live Shopping** events and streams
- **User-Generated Content** campaigns
- **Social Proof** with reviews and ratings

## 📞 Support

For development support and questions:
- Check the documentation in `/docs`
- Review component examples in `/examples`
- API documentation available at `/api/docs`

## 📄 License

This project is proprietary software. All rights reserved.

---

**Built with ❤️ for the future of social commerce**