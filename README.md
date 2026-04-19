# Smart Study Tracker

Smart Study Tracker is a web-based application designed to provide an accurate view of study productivity. It goes beyond basic timers by tracking focus time, detecting distractions, and generating behavioral insights.

---

## Overview

Most study trackers measure total time, which often leads to misleading conclusions about productivity. This application addresses that limitation by distinguishing between active focus and distractions, enabling users to evaluate how effectively they study rather than how long.

---

## Key Features

### Focus Session Tracking

* Start, pause, and end study sessions
* Assign subjects (e.g., DSA, ML, OS)
* Optional goal setting for each session
* Real-time session timer

### Distraction Detection

* Tracks tab switching using browser visibility APIs
* Detects inactivity (idle time)
* Records:

  * Total distraction time
  * Number of interruptions

### Dashboard

* Total study time (daily)
* Focused time
* Distraction time
* Efficiency percentage

Visualizations:

* Subject-wise distribution (pie chart)
* Daily study trends (line graph)

### Insights Engine

Rule-based analysis to generate insights such as:

* Peak productivity hours
* High-distraction time periods
* Changes in efficiency over time

### Session History

* Complete log of study sessions
* Filter by subject or date
* Session-level analytics

---

## Core Logic

```
focus_time = total_time - distraction_time
efficiency = (focus_time / total_time) * 100
```

---

## Technology Stack

### Frontend

* React (Vite)
* Tailwind CSS
* Framer Motion
* Recharts

### Backend

* Node.js
* Express.js

### Database

* MongoDB

---

## Project Structure

```
/client
  /components
  /pages
  /assets

/server
  /routes
  /models
  /controllers
```

---

## Installation

### Clone Repository

```
git clone https://github.com/your-username/smart-study-tracker.git
cd smart-study-tracker
```

### Backend Setup

```
cd server
npm install
npm run dev
```

### Frontend Setup

```
cd client
npm install
npm run dev
```

---

## Future Enhancements

* Browser extension for enhanced tracking
* AI-based personalized recommendations
* Streak tracking and performance analytics
* Notification and reminder system
* Ambient study environment features

---

## Purpose

This project is intended to provide an honest assessment of study behavior by focusing on actual productivity rather than inflated study time.

---

## License

This project is intended for educational and development purposes.
