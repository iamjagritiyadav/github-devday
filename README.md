# 🌆 Lucknow.today

**Lucknow.today** is a modern event discovery platform that aggregates and displays all events happening in Lucknow in one place.
It helps users quickly find concerts, workshops, comedy shows, tech events, and more — without scrolling endlessly across multiple platforms.

---

## 🚀 Features

* 🔎 **Smart Event Discovery**

  * Find events happening *today, this weekend, or upcoming*

* 🧠 **Multi-Source Aggregation**

  * Collects events from platforms like:

    * BookMyShow
    * Paytm Insider
    * Meetup
    * Facebook Events

* 🧹 **Clean & Structured Data**

  * Normalized dates and formats
  * Duplicate event removal
  * Categorized automatically

* 🎨 **Modern UI/UX**

  * Responsive design (mobile-first)
  * Dark & Light mode
  * Smooth animations

* 🎟️ **Detailed Event Pages**

  * Event description
  * Date & time
  * Venue with map
  * Redirect to booking source

* 📅 **Advanced Filters**

  * Category-based filtering
  * Free vs Paid events
  * Date filters (Today, Weekend)

---

## 🛠️ Tech Stack

### Frontend

* Next.js 14 (App Router)
* Tailwind CSS
* ShadCN UI
* Framer Motion

### Backend

* Node.js / Next.js API Routes

### Database

* MongoDB (Mongoose)

### Scraping

* Playwright / Puppeteer

---

## 📂 Project Structure

```
lucknow-today/
│
├── app/                  # Next.js app router
├── components/          # Reusable UI components
├── lib/                 # Utilities & helpers
├── models/              # MongoDB schemas
├── pages/api/           # Backend API routes
├── scraper/             # Scraping scripts
├── public/              # Static assets
└── styles/              # Global styles
```

---

## ⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/your-username/lucknow-today.git
cd lucknow-today
```

### 2. Install dependencies

```bash
npm install
```

### 3. Setup environment variables

Create a `.env.local` file:

```
MONGODB_URI=your_mongodb_connection_string
```

---

### 4. Run the development server

```bash
npm run dev
```

App will be live at:

```
http://localhost:3000
```

---

## 🤖 Running the Scraper

To fetch latest events:

```bash
node scraper/index.js
```

Or trigger via API:

```
POST /api/scrape
```

---

## 🔌 API Endpoints

| Method | Endpoint                   | Description        |
| ------ | -------------------------- | ------------------ |
| GET    | /api/events                | Get all events     |
| GET    | /api/events?category=music | Filter by category |
| GET    | /api/events?date=today     | Events for today   |
| GET    | /api/events/:id            | Event details      |
| POST   | /api/scrape                | Trigger scraper    |

---

## 🔄 Automation

* Scraper runs every 6 hours using cron jobs
* Keeps database updated with latest events

---

## ⚠️ Disclaimer

* This project aggregates publicly available event data
* All event bookings redirect to original platforms
* Proper attribution is maintained

---

## 🌟 Future Enhancements

* AI-based event recommendations
* User accounts & saved events
* Email / WhatsApp alerts
* Organizer dashboard (post your own event)
* Mobile app version

---

## 🤝 Contributing

Contributions are welcome!
Feel free to fork the repo and submit a pull request.

---

## 📌 Author

Built with 💻 by Jagriti

