# 🌍 Travel Tracker

**Travel Tracker** is a web application that allows users to track and record the countries they've visited. The app connects to a PostgreSQL database to store visited countries and displays them on an interactive map. Users can also reset the map to clear all visited countries and start fresh.

## 📚 Table of Contents

- [✨ Features](#features)
- [🛠 Tech Stack](#tech-stack)
- [⚙️ Installation](#installation)
- [🚀 Usage](#usage)
- [🔌 API Endpoints](#api-endpoints)

## ✨ Features

- ➕ Add countries that you've visited to your personal map.
- 🌍 View a list of visited countries.
- 🔄 Reset your map to remove all visited countries.
- 🖥 Interactive UI with real-time updates.
- 💾 Backend connected to a PostgreSQL database for persistent storage.

## 🛠 Tech Stack

- **Frontend:** HTML, CSS, EJS (Embedded JavaScript Templates)
- **Backend:** Node.js, Express.js
- **Database:** PostgreSQL
- **Other Libraries:** Body-Parser, pg (Node.js PostgreSQL client)

## ⚙️ Installation

To run the project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/travel-tracker.git
   cd travel-tracker
2. **Install dependencies**:
   ```bash
    npm install
3. **Set up PostgreSQL database**:
   ```bash
   const db = new pg.Client({
   user: "your_postgres_username",
   host: "localhost",
   database: "world",
   password: "your_postgres_password",
   port: 5432,
   });

4. **Run the server**:
   ```bash
   npm start
5. **The server will run on http://localhost:3000**

## 🚀 Features
➕ Add a Visited Country
  * Go to the home page and input the name of a country that you've visited.
  * The app will look up the country and add it to your list of visited countries.

## 🔌 API Endpoints
  * GET /: Renders the main page, showing a list of visited countries.
  * POST/add: Adds a new country to the list of visited countries.
  * POST /reset: Clears the list of visited countries.
