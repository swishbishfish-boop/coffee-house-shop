# The Roost — Coffee Shop

A simple coffee shop storefront (inspired by watchhouse.com's layout) with a live Supabase backend.

## Stack
- Frontend: plain HTML/CSS/JS (no build step), Supabase JS client via CDN
- Backend: Supabase Postgres table `products`
- Cart: client-side (localStorage)

## Run it
Just open `index.html` in a browser, or deploy as a static site (GitHub Pages, Netlify, Vercel).

## Backend
The `products` table lives in Supabase project `koctawglvhoqefwnjzhq`. Row Level Security is enabled with a public **read-only** policy — the frontend can list products but cannot write to the table using the public key.

Columns: `id, name, description, price, stock, image_url, origin, created_at`

## Next steps (optional)
- Add an `orders` table + Edge Function to handle real checkout
- Add Supabase Auth for accounts/login
- Deploy frontend to GitHub Pages
