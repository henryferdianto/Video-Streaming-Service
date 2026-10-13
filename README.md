# Video Streaming Service Management System

> **TL;DR** — Sistem manajemen langganan video streaming (PacFlix) untuk melihat benefit plan, mengelola user, dan menghitung biaya langganan berdasarkan durasi dan tipe plan.

---

## 🔬 Business Question

Bagaimana mengelola dan menampilkan informasi langganan video streaming secara efisien kepada pelanggan?

**Tujuan:**
- Menampilkan benefit setiap plan (Basic/Standard/Premium)
- Mengelola data user dan plan mereka
- Menghitung biaya langganan berdasarkan durasi

---

## 📊 Plan Structure

| Plan | Harga/Bulan | Kualitas | Devices | Konten |
|---|---|---|---|---|
| Basic | Rp 120.000 | SD | 1 | 3rd Party Movie |
| Standard | Rp 160.000 | HD | 2 | + Sports |
| Premium | Rp 200.000 | UHD | 4 | + PacFlix Original |

---

## 🧮 Metodologi

1. **User Management**: Class-based untukelola data user
2. **Plan Lookup**: Query tabel benefit berdasarkan plan user
3. **Price Calculation**: Harga × durasi dengan diskon jangka panjang

---

## 💡 Key Findings

1. **Tiered pricing** memberikan flexibilitas untuk customer
2. **Class-based architecture** memungkinkan scaling
3. **Benefit table** membantu customer memahami perbedaan plan

---

## 🚀 Cara Menjalankan

```bash
git clone https://github.com/henryferdianto/Video-Streaming-Service.git
cd Video-Streaming-Service
pip install tabulate
python "Video streaming services.py"
```

---

## ⚠️ Limitations

- Data masih dummy (4 user)
- CLI-based, belum ada UI
- Belum ada persistence (data di-hardcode)

---

## 🛠️ Tech Stack

- Python
- tabulate

---

## 📜 License

MIT License — lihat [LICENSE](LICENSE).