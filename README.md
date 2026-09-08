# ShopEase E-Commerce Platform

A complete, production-ready e-commerce platform built with Next.js (frontend) and Express.js with MongoDB (backend).

## Features

- Product catalog with search and filtering
- Product detail pages with images and descriptions
- Shopping cart with add/remove/quantity adjustment
- Checkout flow with shipping and billing address forms
- User authentication (login/register)
- Contact page with business information
- Order confirmation page
- Responsive design for all devices

## Project Structure

```
ecommerce-frontend/   # Next.js frontend
ecommerce-backend/    # Express.js backend with MongoDB
```

## Setup Instructions

### Prerequisites
- Node.js (v18+)
- MongoDB (local or Atlas)

### Frontend Setup

```bash
cd ecommerce-frontend
npm install
npm run dev
```

Frontend runs on http://localhost:3000

### Backend Setup

```bash
cd ecommerce-backend
npm install
# Copy .env.example to .env and configure MongoDB URI
npm run dev
```

Backend runs on http://localhost:5000

### Seed Database

```bash
cd ecommerce-backend
node seed.js
```

## Environment Variables

### Backend (.env)
```
MONGODB_URI=mongodb://localhost:27017/ecommerce
JWT_SECRET=your_jwt_secret_key_here
PORT=5000
```

## Pages

- `/` - Homepage with featured products
- `/products` - Product listing with search/filter
- `/products/[id]` - Product detail page
- `/cart` - Shopping cart
- `/checkout` - Checkout form
- `/contact` - Contact page
- `/order-confirmation` - Order confirmation

## Tech Stack

- Frontend: Next.js 14, React 18, CSS
- Backend: Express.js, MongoDB, Mongoose
- Authentication: JWT, bcryptjs
- Validation: express-validator