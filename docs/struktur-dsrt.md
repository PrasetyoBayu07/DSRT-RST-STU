# 📘 Struktur Proyek DSRT Studio – Manual Editor (Next.js)

> Dokumentasi internal struktur folder dan file aktif untuk DSRT Studio (Manual).  
> Semua file dan folder diatur modular & siap deploy ke Vercel.

---

## 📁 Struktur Proyek DSRT Studio Manual

dsrt-studio-app/ ├── public/ │   ├── logo.png │   └── favicon.ico │ ├── src/ │   ├── app/ │   │   ├── layout.tsx             ✅ layout utama │   │   ├── page.tsx               ✅ halaman utama (wajib) │   │   └── studio/ │   │       └── page.tsx           ✅ halaman DSRT Studio manual │   │ │   ├── components/ │   │   ├── ToolRenderer.tsx       ✅ render tool per grup │   │   ├── ToolGroup.tsx          ✅ switch tool ke komponen │   │   └── ToolControls/ │   │       ├── Brightness.tsx     ✅ contoh tool (1 dari 1200+) │   │       ├── Contrast.tsx │   │       ├── Saturation.tsx │   │       └── dst... (boleh sedikit dulu) │   │ │   ├── data/ │   │   └── toolGroups.ts          ✅ daftar grup & id tools │   │ │   ├── utils/ │   │   ├── presets.ts             ✅ simpan preset ke localStorage │   │   └── supabase.ts            ✅ koneksi Supabase (boleh kosong dulu) │   │ │   └── styles/ │       └── globals.css            ✅ styling dasar │ ├── .env.local.example             ✅ (boleh kosong, template ENV) ├── README.md                      ✅ dokumentasi ringkas ├── package.json                   ✅ dependensi & script ├── tsconfig.json ├── tailwind.config.js ├── next.config.js └── postcss.config.js

---

## 🧱 Keterangan

- Semua tools berada dalam `ToolControls/` dan terdiri dari 1.200+ file TSX individual.
- Halaman Studio dinamis & menggunakan state global tool.
- Preset bisa disimpan secara lokal (`localStorage`) dan online (Supabase).
- File `.env.local.example` perlu di-copy jadi `.env.local` saat runtime.

---

## 🔐 Catatan Penting

- Jangan mengganti `toolId`, nama grup, atau nama folder.
- Selalu tes terlebih dahulu sebelum push ke branch utama.
- Jika ingin menambah tool baru, daftar id-nya harus ditambahkan ke `toolGroups.ts`.

---

✅ _Dokumentasi ini bisa digunakan sebagai panduan dev & backup internal. Untuk PDF, cukup konversi file ini._


---
