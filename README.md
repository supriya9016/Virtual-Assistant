 AI Mock Interviewer App

An AI-powered mock interview platform built with Next.js, TailwindCSS, Firebase, Vercel AI SDK, Google Gemini, and VAPI.
This app allows users to generate custom AI-driven interviews and practice them with a voice-enabled AI assistant.

✨ Features :

📞 Voice-enabled AI Assistant powered by VAPI workflows
🤖 Custom Interview Generation using Google Gemini AI
⚡ Real-time AI Integration via Vercel AI SDK
🗂️ Firestore Database to store interview data and user responses
🎨 Modern UI styled with TailwindCSS
🚀 Serverless API Endpoints with Next.js Route Handlers
☁️ Deployed on Vercel for seamless scalability

Architecture
flowchart TD
  U[👤 User] -->|Initiates Call| VAPI[🎤 VAPI Voice Agent]
  VAPI -->|Collects Responses| API[⚡ Next.js API Endpoint]
  API -->|Feeds User Choices| GEMINI[🤖 Google Gemini AI]
  GEMINI -->|Generates Questions| API
  API -->|Stores Data| DB[(🔥 Firestore Database)]
  DB -->|Dashboard & Analytics| UI[💻 Next.js + Tailwind UI]

📂 Tech Stack

Frontend → Next.js, TailwindCSS
Backend → Next.js Route Handlers
AI Integration → Vercel AI SDK + Google Gemini
Voice AI → VAPI Web SDK (Workflows)
Database → Firebase Firestore
Deployment → Vercel

Setup & Installation

1.Clone the Repository
git clone https://github.com/your-username/ai-mock-interviewer.git
cd ai-mock-interviewer
2️.Install Dependencies
npm install
3️.Configure Environment Variables

Create a .env.local file in the root directory:

# Google Gemini API Key
GOOGLE_API_KEY=your_gemini_api_key

# Firebase Config
NEXT_PUBLIC_FIREBASE_API_KEY=your_firebase_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_project.appspot.com
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id

# VAPI Config
VAPI_API_KEY=your_vapi_api_key

4️. Run the Development Server
npm run dev


How It Works

User initiates a call with AI Assistant (VAPI)
Assistant asks structured questions (frontend/backend/fullstack, tech focus, etc.)
Responses are sent to Next.js API Endpoint
API calls Gemini AI → generates custom interview questions
Results are stored in Firestore
Dashboard displays interview data for analysis & practice




