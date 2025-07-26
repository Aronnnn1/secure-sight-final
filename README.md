# Secure Sight Final

## 1. Deployment Instructions

This project is deployed on [Render](https://render.com).

### Steps to deploy:

1. Clone the repository:
    ```bash
    git clone https://github.com/Aronnnn1/secure-sight-final.git
    cd secure-sight-final
    ```
2. Install dependencies:
    ```bash
    npm install
    ```
3. Build the project:
    ```bash
    npm run build
    ```
4. Start the app locally (for testing):
    ```bash
    npm start
    ```
5. Deploy on Render:
    - Connect your GitHub repo `secure-sight-final` on Render as a **Web Service**
    - Set **Build Command:** `npm install && npm run build`
    - Set **Start Command:** `npm start`
    - Add environment variables (see below)
    - Render automatically redeploys on new commits

### Environment variables

- `DATABASE_URL` — for Prisma DB connection (example for SQLite):
    ```
    file:./dev.db
    ```
---

## 2. Technical Decisions

- **Framework:** Next.js 15 — for server-side rendering, routing, and React support  
- **Database:** Prisma ORM with SQLite — simple file-based database for easy local development  
- **Hosting:** Render.com — chosen for ease of GitHub integration and auto deployment  
- **State Management:** Zustand — lightweight, flexible React state management  
- **Styling:** Tailwind CSS — utility-first CSS framework for fast styling  
- **Authentication:** NextAuth.js — easy authentication with support for multiple providers  

---

## 3. If I Had More Time…

- Implement better error handling and user feedback UI  
- Add role-based access control and user permissions  
- Optimize video loading and implement CDN for media assets  
- Add offline support and better caching strategies  
- Implement analytics and usage tracking dashboard  
- Improve responsive design and accessibility features  

---

**Live demo:** [https://secure-sight-final.onrender.com](https://secure-sight-final.onrender.com)
