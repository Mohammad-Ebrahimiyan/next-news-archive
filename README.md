# NextNews

A modern news archive project built with Next.js (App Router) and a simple Node.js (Express) backend using SQLite. This project demonstrates a clean, responsive UI for browsing, filtering, and viewing news articles, with a minimal backend for data storage and retrieval.

## Features
- 📰 **News Listing**: Browse all news articles with images and summaries.
- 📅 **Archive Filtering**: Filter news by year and month.
- 🔍 **News Details**: View full details and images for each article.
- 🖼️ **Image Modal**: Click images to view in fullscreen modal.
- 🎨 **Modern, Responsive Design**: Clean CSS, mobile-friendly layout.
- ⚡ **Simple Backend**: Express.js API with SQLite database.

## Project Structure
```.
├── app/ # Next.js app directory (pages, layouts, styles)
│ ├── (content)/ # News, archive, and content pages
│ ├── (marketing)/ # Home/landing page
│ ├── api/ # (Optional) API routes
│ └── globals.css # Global styles
├── backend/ # Express.js backend and SQLite DB
│ ├── app.js
│ └── data.db
├── components/ # React UI components
├── lib/ # Helper functions (API, data fetching)
├── public/ # Static assets (images, favicon, etc.)
├── package.json
└── jsconfig.json
```

## Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm

### Installation
1. Install dependencies (frontend & backend):
    ```bash
    npm install
    cd backend
    npm install
    cd ..
    ```

2. Run the backend:
    ```bash
    cd backend
    node app.js
    ```
    The backend runs on `http://localhost:8080`.

3. Run the Next.js frontend:
    ```bash
    npm run dev
    ```
    The app will be available at `http://localhost:3000`.

## Main Routes
- `/` — Home (landing/marketing)
- `/news` — News list
- `/news/[slug]` — News details
- `/archive` — News archive (filter by year/month)

## Styling
- Uses **Merriweather** and **Inter** fonts.
- Modern, accessible color palette.
- Responsive grid for news listing.
- Custom modal for fullscreen images.

## License
This project is for educational and demonstration purposes only.
