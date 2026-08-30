# Commons — AI-Powered Peer Networking

🏆 **Best Hack in Tech, AthenaHacks 2025**

Commons matches students with peers worth meeting — not by follower counts, but by what they're actually into. Sign up with a verified **.edu** address, and a **Gemini-powered matching engine** recommends people based on interests and goals.

> This repo holds the Node.js backend from the hackathon build.

## What's inside

```
Backend/src/
  ├─ app.js / server.js       Express app + entry point
  ├─ middleware/auth.js       JWT auth, .edu verification
  ├─ models/                  users, friends, authentication (MongoDB)
  ├─ routes/userRoutes.js     signup, login, matching, friends
  └─ utils/matchingEngine.js  Gemini API–driven peer recommendations
```

- **.edu verification** gates signup so every profile is a real student.
- **Matching engine** sends structured interest profiles to the Gemini API and ranks peer recommendations.
- **JWT-based auth** protects all user routes.

## Tech

Node.js · Express · MongoDB (Mongoose) · Gemini API · JWT

## Running it

```bash
cd Backend
npm install
cp .env.example .env   # MONGO_URI, JWT_KEY, GEMINI_API_KEY
npm start
```
