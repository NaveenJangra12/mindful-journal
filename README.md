# Mindful Journal

A web-based journaling application with automated sentiment analysis.
Built with React.js, local storage persistence, and a VADER-style NLP sentiment engine.

## Features

- User registration and login (stored locally)
- Create, read, edit, delete journal entries
- Real-time sentiment analysis (positive / neutral / negative)
- Mood trend charts and analytics (Recharts)
- Responsive design for desktop and mobile
- Demo data seeded on first register

## Tech Stack

- React 18 + React Router 6
- Recharts for data visualization
- date-fns for date formatting
- Custom VADER-style sentiment engine (no external API needed)
- localStorage for data persistence

## Getting Started

### Prerequisites
- Node.js 16+ installed
- npm or yarn

### Installation

```bash
# 1. Install dependencies
npm install

# 2. Start the development server
npm start

# 3. Open in browser
http://localhost:3000
```

### Demo Account

On the Register page, create any account. Demo journal entries will be seeded automatically.

Or on the Login page click **"Use demo account"** — but first register with:
- Email: demo@mindfuljournal.com
- Password: demo123

## Project Structure

```
src/
  components/       # Navbar, EntryCard, SentimentBadge
  context/          # AuthContext, JournalContext
  pages/            # Login, Register, Dashboard, Entries,
                    # NewEntry, EditEntry, EntryDetail, Analytics
  utils/            # sentiment.js (NLP engine + seed data)
  index.css         # Global CSS variables and animations
  App.js            # Routes
  index.js          # Entry point
```

## Deployment

### Docker

```bash
# Build and run with Docker
docker build -t mindful-journal .
docker run -p 3000:3000 mindful-journal
```

### Docker Compose (with backend)

```bash
docker-compose up --build
```

## Author

Naveen Kumar — IU International University of Applied Sciences
DLMCSPSE01 — Project Software Engineering
