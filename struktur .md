```
dsrt-studio-app/
├── .github/                  → (Opsional) Workflow
│
├── public/                   → Aset publik
│   ├── logo.png
│   ├── favicon.ico
│   └── splashscreen.mp4
│
├── src/
│   ├── app/
│   │   ├── layout.tsx        → Layout utama
│   │   └── studio/
│   │       └── page.tsx      → Halaman DSRT Studio Manual
│   │
│   ├── components/
│   │   ├── tools/            → Semua tool (1.200+)
│   │   │   ├── Brightness.tsx
│   │   │   ├── Contrast.tsx
│   │   │   └── ...
│   │   ├── ToolRenderer.tsx  → Render berdasarkan grup
│   │   └── ToolGroup.tsx     → Switch toolId ke komponen
│   │
│   ├── data/
│   │   └── toolGroups.ts     → Grup tool
│   │
│   ├── utils/
│   │   ├── supabase.ts       → Koneksi Supabase
│   │   └── presets.ts        → Menyimpan preset
│   │
│   └── styles/
│       └── globals.css       → Styling Tailwind global
│
├── .env.local.example        → Template Supabase ENV
├── README.md                 → Dokumentasi GitHub
├── tailwind.config.js        → Konfigurasi Tailwind
├── tsconfig.json             → Konfigurasi TypeScript
├── next.config.js            → Konfigurasi Next.js
├── package.json              → Dependensi proyek
└── postcss.config.js         → Konfigurasi PostCSS
```