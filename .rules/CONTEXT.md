# 📈 Stock Market Prediction App (MERN + AI)

## Overview
This is a full-stack stock market prediction and simulation application built using the MERN stack.

The application allows users to:
- Create an account and login
- View stock market data
- Simulate buying and selling stocks
- View their portfolio performance
- Use AI (Gemini API) to analyze stock trends and predict next movements

---

## Tech Stack

### Frontend
- React (Vite)
- Tailwind CSS
- React Router
- Axios

### Backend
- Node.js
- Express.js
- MongoDB (Mongoose)

### AI Integration
- Gemini API (for stock analysis and prediction)

---

## Features

### 1. Authentication
- User signup and login
- JWT-based authentication
- Protected routes

---

### 2. Dashboard
- Sidebar navigation
- User profile info
- Navigation to stocks and portfolio

---

### 3. Stock Module
- List of stocks with price and change %
- Individual stock detail page
- Historical price chart

---

### 4. Trading Simulation
- Buy stocks
- Sell stocks
- Portfolio tracking
- Profit/Loss calculation

---

### 5. AI Analyzer
- Analyze stock using Gemini API
- Predict next movement (UP/DOWN)
- Confidence score
- Explanation of prediction

---

## Folder Structure

root/
├── client/
├── server/

---

## Environment Variables

### Server (.env)
PORT=5000  
MONGO_URI=your_mongodb_uri  
JWT_SECRET=your_jwt_secret  
GEMINI_API_KEY=your_gemini_api_key  

### Client (.env)
VITE_API_BASE_URL=http://localhost:5000/api  

---

## API Routes

### Auth
- POST /api/auth/signup
- POST /api/auth/login

### Stocks
- GET /api/stocks
- GET /api/stocks/:symbol

### Trading
- POST /api/trade/buy
- POST /api/trade/sell
- GET /api/portfolio

### AI
- POST /api/ai/analyze

---

## AI Prompt Strategy

Gemini should receive:
- Historical stock prices
- Current price
- Trend summary

Expected Output:
- Prediction: UP or DOWN
- Confidence (0–100%)
- Explanation in simple terms

---

## UI Requirements

- Clean modern UI using Tailwind
- Responsive design
- Dashboard layout with sidebar
- Stock charts
- AI analyzer section

---

## Notes

- This is a simulation, not real trading
- AI predictions are indicative, not guaranteed
- Focus on clarity, usability, and structure

---

## Goal

Build a complete, production-ready stock analysis and simulation platform with AI-powered insights.