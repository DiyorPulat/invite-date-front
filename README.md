# Birga — Invite Date frontend

Invite Date Spring Boot API uchun React/Vite frontend.

```bash
npm install
cp .env.example .env.local
npm run dev
```

Backend odatiy holatda `http://localhost:8080` manzilida ishlaydi. Boshqa manzil uchun `.env.local` ichida `VITE_API_BASE_URL` qiymatini o'zgartiring.

Productionda backenddagi `PUBLIC_BASE_URL` frontend domeniga, `CORS_ALLOWED_ORIGINS` esa shu domen(lar)ga sozlanishi kerak.
