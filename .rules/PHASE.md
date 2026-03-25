🧩 PHASE 0 — Project Setup (MERN Base)

Create a full MERN stack project with separate client and server folders.

Requirements:
	•	Client: React (Vite), Tailwind CSS, Axios, React Router
	•	Server: Node.js, Express, MongoDB (Mongoose)

Folder Structure:
	•	client/
	•	server/

Setup:
	•	Configure basic Express server
	•	Connect MongoDB using Mongoose
	•	Enable CORS and JSON parsing
	•	Setup React app with routing

Environment:
	•	Create .env in both client and server

Server .env:
PORT=5000
MONGO_URI=
JWT_SECRET=
GEMINI_API_KEY=

Client .env:
VITE_API_BASE_URL=http://localhost:5000/api

Ensure:
	•	Server runs on port 5000
	•	Client runs on port 5173
	•	Basic test route /api/test

⸻

🔐 PHASE 1 — Authentication System

Build authentication system using JWT.

Backend:
	•	User model:
	•	name
	•	email
	•	password (hashed using bcrypt)

Routes:
	•	POST /api/auth/signup
	•	POST /api/auth/login

Features:
	•	Hash passwords
	•	Generate JWT token
	•	Middleware to protect routes

Frontend:
	•	Pages:
	•	Login
	•	Signup

UI:
	•	Clean modern form using Tailwind

Logic:
	•	Store JWT in localStorage
	•	Redirect to dashboard after login

Validation:
	•	Proper error messages

⸻

📊 PHASE 2 — Dashboard UI

Create dashboard layout after login.

Features:
	•	Sidebar (Dashboard, Stocks, Portfolio, Logout)
	•	Navbar (User info)

Pages:
	•	Dashboard Home
	•	Stocks List Page
	•	Portfolio Page

Design:
	•	Use Tailwind
	•	Clean, minimal UI

Functionality:
	•	Protect all routes (only logged-in users)
	•	Fetch user info from backend

⸻

📈 PHASE 3 — Stock Data Integration

Implement stock listing and detail page.

Backend:
	•	Routes:
GET /api/stocks
GET /api/stocks/:symbol

Data:
	•	Use mock data or free stock API (Alpha Vantage / Yahoo Finance)

Frontend:
	•	Stocks Page:
	•	List of stocks with price and change %
	•	Stock Detail Page:
	•	Graph using Chart.js or Recharts
	•	Price history

Ensure:
	•	Clicking a stock opens detail page

⸻

💰 PHASE 4 — Buy/Sell Simulation

Implement buy/sell stock simulation.

Backend:
	•	Portfolio model:
	•	userId
	•	stockSymbol
	•	quantity
	•	avgPrice

Routes:
	•	POST /api/trade/buy
	•	POST /api/trade/sell
	•	GET /api/portfolio

Logic:
	•	Update portfolio on buy/sell
	•	Prevent selling more than owned

Frontend:
	•	Stock Page:
	•	Buy/Sell form
	•	Portfolio Page:
	•	Show holdings
	•	Profit/Loss calculation

⸻

🤖 PHASE 5 — Gemini AI Analyzer

Integrate Gemini API for stock prediction.

Backend:
	•	Route:
POST /api/ai/analyze

Input:
	•	Stock historical data
	•	Current price

Logic:
	•	Send prompt to Gemini API including:
	•	Trend analysis
	•	Price movement prediction

Expected Output:
	•	Prediction (UP/DOWN)
	•	Confidence %
	•	Explanation

Frontend:
	•	Add “AI Analyzer” section in stock detail page
	•	Button: “Analyze Stock”

Display:
	•	Prediction
	•	Confidence
	•	Explanation

⸻

🎨 PHASE 6 — UI Polish & UX

Improve UI/UX across the app.

Enhancements:
	•	Loading states (spinners/skeletons)
	•	Toast notifications
	•	Proper error handling
	•	Fully responsive design

Optional:
	•	Animations (Framer Motion)
	•	Improved charts
	•	Clean spacing & typography

⸻

🚀 PHASE 7 — Deployment Ready

Prepare the app for deployment.

Tasks:
	•	Move all secrets to .env
	•	Optimize API calls
	•	Build React app

Deployment Options:
	•	Serve frontend from backend OR deploy separately

Add:
	•	Basic security:
	•	helmet
	•	rate limiting
	•	Environment-based configs

⸻

⚠️ FINAL NOTES
	•	This is a simulation, not real trading
	•	AI predictions are not guaranteed accurate
	•	Backend must control all core logic
	•	Keep UI and logic separate