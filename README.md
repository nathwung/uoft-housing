# 🏠 UofT Housing

[![Built with: React](https://img.shields.io/badge/Built%20with-React-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://reactjs.org/)
[![Backend: Flask](https://img.shields.io/badge/Backend-Flask-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![Database: PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Deployed on Vercel & Render](https://img.shields.io/badge/Hosted%20on-Vercel%20&%20Render-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://uoft-housing.vercel.app)

A marketplace platform **exclusively for University of Toronto students** to sublet housing, find roommates, and buy/sell furniture. Built with **React**, **Flask**, and **PostgreSQL**, it features user authentication, real-time messaging between buyers and sellers, dynamic listing creation with images and filters, interactive maps, and secure email verification and password reset flows.

---

## 🚀 Features

### 🔐 UofT-Verified Authentication
- Register with a valid `@mail.utoronto.ca` email
- Email verification via SendGrid
- Secure login with JWT token authentication
- Edit profile (name, program, year) with instant reflection across listings & messages
- Password reset via email

### 🏘️ Listings Marketplace
- Create listings for:
  - 🛏️ Sublets
  - 🧍 Roommate Requests
  - 🪑 Furniture Market
  - 🏡 Long-Term Housing
- Upload multiple images
- Dynamic amenities, duration, and price options
- Integrated Leaflet map & geolocation from OpenStreetMap
- View listings in real-time by location or category

### ⭐ Favorites System
- Save and unsave listings (persistent in PostgreSQL)
- View saved listings under `/saved`
- Filter by favorites or listing type

### 💬 Messaging System
- Buyer–seller chat system per listing
- WhatsApp-style UI with green/white message bubbles
- Send and delete messages (both sides synced)
- Seller can view grouped chats by buyer on listing edit page

### 🧠 Smart UI/UX
- Responsive layout with Tailwind CSS & Framer Motion
- Listing modals, animated carousels, filter buttons with icons
- Skeleton loaders for loading states
- Chat auto-scroll, grouped messages, and rich detail badges

---

## 🛠 Tech Stack

- **Frontend**: React, Tailwind CSS, Framer Motion  
- **Backend**: Python, Flask, Flask-SQLAlchemy, Flask-CORS  
- **Database**: PostgreSQL  
- **Authentication & Email**: JWT, SendGrid  
- **Hosting**: Vercel (frontend), Render (backend)

---

## 🔗 Links

- 🌐 **Website**: [uoft-housing.vercel.app](https://uoft-housing.vercel.app/)  
- 🎥 **Video Demo**: [Watch on Google Drive](https://drive.google.com/file/d/1EzaCifBafGvaQluX7zmfk1MRs3IsTnuR/view) 
- 💻 **Frontend Code**: [GitHub Repo](https://github.com/nathwung/uoft-housing-frontend)  
- 🔧 **Backend Code**: [GitHub Repo](https://github.com/nathwung/uoft-housing-backend)  
