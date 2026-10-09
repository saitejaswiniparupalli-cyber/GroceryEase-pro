# GroceryEase Pro

A responsive grocery-ordering and resource-management prototype inspired by the convenience of quick-commerce apps and the discovery patterns of large online marketplaces.

## Pages and working prototype features
- Home / offers / category browsing
- Shop with search, category filters and sorting
- Product details modal, favourites and quantity controls
- Cart with quantity updates, removal and subtotal / delivery fee
- Checkout form and demo order placement
- Order history and order status timeline
- Wishlist
- Admin dashboard with product CRUD, stock updates, order status management and low-stock alerts
- Express REST API with JSON-file persistence
- Responsive desktop, tablet and mobile layout

## Run locally
1. Install Node.js 18 or later.
2. Open this folder in VS Code.
3. In the terminal run `npm install`.
4. Run `npm start`.
5. Open `http://localhost:3000`.

The JSON database is in `data/db.json` and is created automatically if missing. This is a local demo database, not production storage.

## Demo notes
- Admin area is a prototype UI and is not protected by authentication. Do not deploy it publicly as-is.
- Orders and stock changes are persisted to `data/db.json` while the server is running locally.
- Product images load from Unsplash URLs and therefore require internet access; emoji fallback icons remain available.
- Before real deployment, add authentication/authorization, validation, rate limiting, secure payment integration, a real database, and environment-based configuration.

## GitHub
Create a new empty repository, then run in this folder:
```
git init
git add .
git commit -m "Build GroceryEase Pro prototype"
git branch -M main
git remote add origin YOUR_REPOSITORY_URL
git push -u origin main
```
Replace `YOUR_REPOSITORY_URL` with your repository URL. Do not upload `node_modules` or secrets.


## Login and sign-up (prototype)
- Open the app at `http://localhost:3000`; users are sent to the sign-in page first.
- Demo access: `demo@groceryease.in` / `Fresh123!`, or click **Continue with demo account**.
- Create-account and sign-in flows are included for local prototype demonstrations. Account records are stored in this browser's local storage and are not production-grade authentication. Do not use real passwords or deploy this login for real customers. For production, replace it with server-side authentication, secure sessions/cookies, rate limiting, password hashing on the server, and authorization checks for admin APIs.
