# E-commerce Setup Guide

## Environment Variables Required

Create a `.env.local` file in the root directory with the following variables:

```env
# Clerk Authentication
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key_here
CLERK_SECRET_KEY=your_clerk_secret_key_here

# MongoDB Database
MONGODB_URI=mongodb://localhost:27017/your_database_name
# Or for MongoDB Atlas:
# MONGODB_URI=mongodb+srv://username:password@cluster.mongodb.net/your_database_name

# Currency (optional)
NEXT_PUBLIC_CURRENCY=USD

# Inngest (optional - for background jobs)
INNGEST_EVENT_KEY=your_inngest_event_key_here
INNGEST_SIGNING_KEY=your_inngest_signing_key_here
```

## Installation Steps

1. Install dependencies:
   ```bash
   npm install
   ```

2. Set up your environment variables in `.env.local`

3. Run the development server:
   ```bash
   npm run dev
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser

## Clerk Setup

1. Go to [clerk.com](https://clerk.com) and create an account
2. Create a new application
3. Copy your publishable key and secret key to the environment variables
4. Configure your Clerk application settings as needed

## MongoDB Setup

1. Install MongoDB locally or use MongoDB Atlas
2. Create a database for your application
3. Update the MONGODB_URI in your environment variables

## Issues Fixed

- ✅ Database connection string syntax error
- ✅ User model schema syntax error  
- ✅ ESLint configuration issue
- ✅ Layout.js syntax error
- ✅ Missing environment variables documentation 