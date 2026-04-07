# 🐝 SkillHive — Skill Sharing Platform

A community platform where users can share their skills and connect with others to learn.  
Built with **React + Vite** for the semester mini project.

---

## ✨ Features

- **Browse & Search Skills** — Filter by skill category, search by name or keyword
- **User Profiles** — Detailed profiles showing skills offered and learning interests  
- **In-app Messaging** — Real-time chat between users to coordinate sessions
- **Skill Swap** — Propose a skill exchange with anyone on the platform
- **Responsive Design** — Works on desktop and mobile

---

## 🚀 Getting Started

### Prerequisites
- Node.js v18+ 
- npm v9+

### Install & Run Locally

```bash
# 1. Navigate to the project folder
cd skillhive

# 2. Install dependencies
npm install

# 3. Start development server
npm run dev
```

Then open **http://localhost:5173** in your browser.

### Demo Login
The app has 3 demo accounts you can log in with:
- **Aryan Mehta** — React, Node.js, Tabla
- **Priya Sharma** — Figma, UI Design, Yoga  
- **Vikram Soni** — Guitar, Cooking, Music Theory

---

## 🏗️ Build for Production

```bash
npm run build
```

This generates a `dist/` folder with the production-ready static files.

---

## 🌐 Deployment

### Option 1: Vercel (Recommended — Free)
1. Push your code to a GitHub repository
2. Go to [vercel.com](https://vercel.com) → **New Project**
3. Import your GitHub repo
4. Leave all settings as default (Vercel auto-detects Vite)
5. Click **Deploy** — done! ✅

### Option 2: Netlify (Free)
1. Run `npm run build` locally
2. Go to [netlify.com](https://netlify.com) → **Add new site → Deploy manually**
3. Drag and drop your `dist/` folder
4. Live instantly! ✅

### Option 3: GitHub Pages
```bash
# Install gh-pages
npm install --save-dev gh-pages

# Add to package.json scripts:
# "deploy": "gh-pages -d dist"

# Add to vite.config.js:
# base: '/your-repo-name/'

npm run build
npm run deploy
```

---

## 📁 Project Structure

```
skillhive/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── Navbar.jsx        # Top navigation bar
│   │   ├── Toast.jsx         # Notification toasts
│   │   └── UserCard.jsx      # User card for explore grid
│   ├── context/
│   │   └── AppContext.jsx    # Global state (users, messages, auth)
│   ├── pages/
│   │   ├── Landing.jsx       # Home / landing page
│   │   ├── Login.jsx         # Login page
│   │   ├── Signup.jsx        # Registration page
│   │   ├── Explore.jsx       # Browse & search skills
│   │   ├── UserProfile.jsx   # Individual user profile
│   │   ├── Messages.jsx      # Chat / messaging page
│   │   └── Profile.jsx       # My profile & edit
│   ├── App.jsx               # Router & app shell
│   ├── index.css             # Global design system
│   ├── mobile.css            # Responsive styles
│   └── main.jsx              # Entry point
├── index.html
├── vite.config.js
└── package.json
```

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| React 18 | UI framework |
| React Router v6 | Client-side routing |
| Vite | Build tool & dev server |
| Lucide React | Icons |
| CSS Variables | Design system / theming |

> **Note:** All data is stored in React state (in-memory). For a production app, you'd connect to a backend (Firebase, Supabase, etc.)

---

Built with 🐝 for semester mini project
