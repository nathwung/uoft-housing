# 🏠 UofT Housing

[![Built with: React](https://img.shields.io/badge/Built%20with-React-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://reactjs.org/)
[![Backend: Flask](https://img.shields.io/badge/Backend-Flask-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![Database: PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Deployed on Vercel & Render](https://img.shields.io/badge/Hosted%20on-Vercel%20&%20Render-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://uoft-housing.vercel.app)

A marketplace platform exclusively for University of Toronto students to sublet housing, find roommates, and buy/sell furniture. Built with **React**, **Flask**, and **PostgreSQL**, it features user authentication, real-time messaging between buyers and sellers, dynamic listing creation with images and filters, interactive maps, and email flows for both verification and password reset.

---

## 🚀 Features

### 🛬 Landing Page

- Hero with category cards for Roommates, Sublets, Furniture, and Long-Term Housing
- Step-by-step timeline on how the platform works  
- Real-world student scenarios
- Blurred featured listings
- About section with mission-driven highlights and trust badges  
- A floating assistant bot is embedded to help users with suggestions during their visit
- Dark mode toggle

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

### 🗺 Interactive Map
  - Uses **Leaflet.js** with **OpenStreetMap Nominatim**
  - On listing creation, location is geocoded to lat/lng
  - Pins dropped on map
  - Hover preview shows location name
  - Clicking a pin filters listings by that location for targeted discovery
  - Includes a toggle to show or hide the map for a full-screen listings view

### 💾 Save Listings Feature
- Click the ⭐ star icon on any listing to save or unsave it
- Saved listings are stored persistently in PostgreSQL
- Toggle the "Show Saved Only" button to filter and view just your saved listings

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

- **Frontend**: React, Tailwind CSS, Framer Motion, Leaflet.js
- **Backend**: Python, Flask, Flask-SQLAlchemy, Flask-CORS
- **Database**: PostgreSQL
- **Authentication & Email**: JWT, SendGrid
- **Geolocation**: OpenStreetMap Nominatim API
- **Hosting**: Vercel (frontend), Render (backend)

---

## 🔗 Links

- 🌐 **Website**: [uoft-housing.vercel.app](https://uoft-housing.vercel.app/)  
- 🎥 **Video Demo**: [Watch on Google Drive](https://drive.google.com/file/d/1NHOmTrlppiNmcszzT_7A_Bl2ZQGPeZD9/view?usp=sharing) 
- 💻 **Frontend Code**: [GitHub Repository](https://github.com/nathwung/uoft-housing-frontend)  
- 🔧 **Backend Code**: [GitHub Repository](https://github.com/nathwung/uoft-housing-backend)  
