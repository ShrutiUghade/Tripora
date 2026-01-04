🌍TripOra — Smart Travel Itinerary Planner

TripOra is a smart, all-in-one travel planner that creates personalized itineraries for your trips. Explore destinations, hotels, restaurants, and flights — all in one platform.

🔗 Live Demo → https://Tripora.netlify.app

✨ Features
🎯 Core Functionality


AI-like Itinerary Builder — Generates day-wise plans based on destination and dates


Destination Search — Real-time data from trusted APIs


Attraction Recommendations — Find landmarks, museums, beaches, etc.


Hotel & Restaurant Finder — Curated listings near your destination


Flight Info — View available flights across Indian cities


Drag & Drop Planner — Reorder places intuitively


PDF Export — Download complete itineraries offline


🔐 Authentication


JWT-secured Login/Signup


Google OAuth 2.0


User Profiles & Saved Trips


Protected Routes & Session Cookies


🎨 User Experience


Modern UI/UX — Tailwind CSS + Framer Motion animations


Responsive Design — Works smoothly on all devices


Toast Notifications — Instant feedback for user actions



🛠️ Tech Stack
Frontend: React 19, Tailwind CSS, React Router DOM,Axios + html2pdf.js
Backend: Node.js + Express , MongoDB (Mongoose),Passport.js + JWT, CORS Middleware, bcryptjs + Cookie Parser 
APIs / Services: OpenTripMap (Attractions), Geoapify (Hotels/Restaurants),Google OAuth, MongoDB Atlas


📁 Project Structure
WayOra/
├── backend/
│   ├── controllers/        # Auth, Itinerary, Flights, Search
│   ├── models/             # User, Itinerary, Cache Schemas
│   ├── routes/             # Auth, Itinerary, Search, Flights
│   ├── middleware/         # Auth & Error handlers
│   ├── utils/              # API handlers, cache utilities
│   └── server.js           # Entry point
│
├── frontend/
│   ├── src/
│   │   ├── components/     # UI components (Dashboard, Trips, Flights, etc.)
│   │   ├── pages/          # Home, Dashboard, OAuth success
│   │   ├── utils/          # API helpers
│   │   └── App.jsx         # App entry & routing
└── images/                 # Static assets


🚀 Getting Started
Prerequisites


Node.js v18+


npm or yarn


MongoDB Atlas (or local)


Google Cloud OAuth credentials


Installation
# Clone repo
git clone https://github.com/yourusername/wayora.git
cd wayora

# Install backend & frontend dependencies
cd backend && npm install
cd ../frontend && npm install

Environment Setup
Backend .env
PORT=5000
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_secret_key
GOOGLE_CLIENT_ID=your_client_id
GOOGLE_CLIENT_SECRET=your_client_secret
CLIENT_URL=http://localhost:5173
OPENTRIPMAP_API_KEY=your_key
GEOAPIFY_API_KEY=your_key

Frontend .env
VITE_API_BASE_URL=http://localhost:5000/api


🏃 Running Locally
Development
# Backend
cd backend
npm run dev

# Frontend (in another terminal)
cd frontend
npm run dev


Open http://localhost:5173

Production
cd frontend && npm run build
cd ../backend && npm start


🌐 Deployment
Frontend (Netlify)


Deploy the frontend/dist folder


Add env: VITE_API_BASE_URL=https://your-backend.onrender.com


Backend (Render)


Build: cd backend && npm install


Start: cd backend && npm start


Add env vars (same as .env)


Set CLIENT_URL to your Netlify frontend URL



Update OAuth redirect URIs in Google Cloud Console for production.


📚 API Overview
Endpoint	Method	Description
/api/auth/register	POST	Register user
/api/auth/login	POST	Login user
/api/auth/google	GET	Google OAuth
/api/search	GET	Fetch destination data
/api/itinerary/save	POST	Save itinerary
/api/itinerary/mytrips	GET	Get saved trips
/api/flights	GET	Fetch flight info



Password hashing via bcrypt


JWT token authentication


Protected API routes


Secure cookies & CORS config



🎯 Highlights


Smart day-by-day planning with automated attraction sorting


Caching system for destinations & flights (faster results)


Interactive drag-and-drop itinerary editor


PDF export & trip management for travelers



🤝 Contributing


Fork the repo


Create a branch → git checkout -b feature/NewFeature


Commit changes → git commit -m "Add new feature"


Push → git push origin feature/NewFeature


Open a Pull Request



🔮 Future Enhancements


Real flight booking


Weather integration


Collaborative trip planning


Cost estimation & budgeting


Social sharing


Multi-language support


Mobile app (React Native)



📝 License
Licensed under the ISC License

👨‍💻 Author
Medha Pant — Full Stack Developer

🙏 Acknowledgments
Thanks to:


OpenTripMap


Geoapify


Google OAuth


React, Vite, Tailwind & open-source contributors



Made with ❤️ for travelers everywhere.



