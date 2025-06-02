# 🏠 UofT Housing

[![Built with: React](https://img.shields.io/badge/Built%20with-React-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://reactjs.org/)
[![Backend: Flask](https://img.shields.io/badge/Backend-Flask-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![Database: PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Deployed on Vercel & Render](https://img.shields.io/badge/Hosted%20on-Vercel%20&%20Render-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://uoft-housing.vercel.app)

A marketplace platform exclusively for University of Toronto students to sublet housing, find roommates, and buy/sell furniture. Built with **React**, **Flask**, and **PostgreSQL**, it features user authentication, real-time messaging between buyers and sellers, dynamic listing creation with images and filters, interactive maps, and secure email verification and password reset flows.

---

## 🚀 Features

### 🔐 UofT-Verified Authentication
- Register with a valid `@mail.utoronto.ca` email address
- Confirm email through a **SendGrid-powered verification link**
- Secure login using **JWT token-based authentication**
- Update your name, program, and graduation year — changes reflect instantly across listings and messages
- Forgot your password? Reset securely through an email flow

### 🏘️ Listings Marketplace
- Post listings for:
  - 🛏️ Sublets
  - 🧍 Roommate Requests
  - 🪑 Furniture Market
  - 🏡 Long-Term Housing
- Each listing supports:
  - Title, location, description, negotiable pricing, images, amenities
  - Conditional fields: bedrooms, bathrooms, roommate preference, sublet duration, and furnishing status
- Interactive Leaflet Map Integration:
  - When a listing is created, its address is geocoded via OpenStreetMap Nominatim to generate latitude/longitude
  - A pin is dropped on the map with location preview on hover
  - Clicking a pin filters visible listings by that location for targeted browsing

### ❤️ Favorites System
- Click the ⭐ star icon on any listing to favorite or unfavorite it
- Favorites are stored persistently in PostgreSQL
- Toggle the "Show Saved Only" button to filter the listings view to only your favorites

### 💬 Messaging System
- Initiate chats with listing owners directly from the detail page
- Built with a WhatsApp-style UI:
  - Green message bubbles for sender, white for receiver
  - Auto-scroll to newest messages
  - Delete individual messages
- Sellers can view grouped buyer conversations in the Edit Listing view
- Messages persist via PostgreSQL for consistent experience across sessions

### 🧠 Smart UI/UX
- Fully responsive UI using Tailwind CSS
- Smooth transitions and interactions using Framer Motion
- Listing cards feature:
  - Modal previews
  - Carousel image sliders
  - Filter buttons with icons
  - Skeleton loaders during data fetching
  - Edit pages conditionally render fields based on listing type

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
- 🎥 **Video Demo**: [Watch on Google Drive](https://drive.google.com/file/d/1NHOmTrlppiNmcszzT_7A_Bl2ZQGPeZD9/view?usp=sharing) 
- 💻 **Frontend Code**: [GitHub Repository](https://github.com/nathwung/uoft-housing-frontend)  
- 🔧 **Backend Code**: [GitHub Repository](https://github.com/nathwung/uoft-housing-backend)  
