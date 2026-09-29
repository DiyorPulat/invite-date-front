# Birga — Invite Date frontend

Invite Date Spring Boot API uchun React/Vite frontend.

```bash
npm install
cp .env.example .env.local
npm run dev
```

Backend odatiy holatda `http://localhost:8080` manzilida ishlaydi. Boshqa manzil uchun `.env.local` ichida `VITE_API_BASE_URL` qiymatini o'zgartiring.

Developmentda `/api` so‘rovlari Vite proxy orqali backendga uzatiladi, shuning uchun brauzer CORS xatosi bermaydi. Backend boshqa hostda bo‘lsa `.env.local` ichida `VITE_API_PROXY_TARGET` ni o‘zgartiring.

Productionda frontend va backend turli domenlarda bo‘lsa, backenddagi `PUBLIC_BASE_URL` ni frontend domeniga, `CORS_ALLOWED_ORIGINS=*` ni esa barcha originlarga ruxsat beradigan qilib sozlang. Agar Spring Boot `CorsConfiguration` ishlatilsa, `allowedOrigins("*")`, `allowedMethods("*")`, `allowedHeaders("*")` va kerak bo‘lsa `allowCredentials(false)` ni qo‘llang. `*` bilan credentials/cookie ishlatib bo‘lmaydi.
