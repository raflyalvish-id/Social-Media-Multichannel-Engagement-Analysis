# 📱 Social Media Cross-Platform Engagement & Conversion Analysis (Power BI)

## 📌 Project Overview
Project ini berfokus pada analisis performa konten media sosial lintas platform (X/Twitter, Instagram, TikTok, dan YouTube) dengan mengevaluasi **726.933 interaksi** dan total **5.0M Reach**. Menggunakan pemodelan data berbasis rumus DAX tingkat lanjut di Power BI, analisis ini membedah efektivitas distribusi organik vs promosi berbayar (Paid Ads) untuk menentukan format dan saluran mana yang memberikan nilai konversi nyata (CTR) bagi bisnis, bukan sekadar popularitas.

### 🎯 Objectives
- Mengukur efisiensi jangkauan unik audiens menggunakan formulasi metrik *Engagement Rate by Reach* (ER Reach).
- Membandingkan karakteristik performa dan kekuatan distribusi makro antar platform.
- Menganalisis korelasi antara format konten terhadap *Audience Retention* dan rasio konversi klik (CTR).
- Menyusun *Strategic Roadmap* berbasis data untuk optimasi *Content Scheduling* dan alokasi *budget* iklan.

---

## 📂 Project Resources (Quick Links)
- 📊 **[Download Power BI Dashboard File (Social Media Analytics.pbix)](./Social Media Analytics.pbix)**
- 📄 **[View Full Presentation Deck (Social Media Engagement Analysis.pdf)](./Social Media Engagement Analysis.pdf)** 

---

## 🗄️ Methodology & DAX Formulations
Untuk menjamin standardisasi metrik yang objektif di seluruh ekosistem digital, pemodelan data ini menggunakan logika visualisasi DAX sebagai berikut:

* **Total Interactions:** Mengukur bobot respons aktif audiens secara keseluruhan.
  ```dax
  Total Interactions = SUM(Data[Likes]) + SUM(Data[Comments]) + SUM(Data[Shares]) + SUM(Data[Saves])
* **Engagement Rate by Reach (ER Reach):** Mengukur efisiensi konten dalam memicu interaksi dari setiap jangkauan unik pengguna.
    ```dax
    er_reach = DIVIDE([Total Interactions], SUM(Data[Reach]), 0)
* **Click-Through Rate (CTR):** Evaluasi murni terhadap konversi tindakan klik audiens.
  ```dax
  ctr_dax = DIVIDE(SUM(Data[Clicks]), SUM(Data[Impressions]), 0)
* **Average Completion Rate:** Mengukur tingkat ketahanan durasi tontonan audiens pada format video.
  ```dax
  avg_completion_rate = AVERAGE(Data[Completion_Rate])

## 📈 Executive Insights & Key Findings
### 📊 Platform Performance Breakdown
- X / Twitter: Mendominasi volume trafik secara masif dengan menyumbang 331K+ interaksi (45,6% dari total ekosistem) serta mencetak ER Reach tertinggi di angka 23%.
- TikTok: Tampil sebagai platform paling efisien dari segi kualitas interaksi dengan memimpin angka konversi klik (CTR 8%) dan tingkat retensi audiens tertinggi (55%).
- YouTube: Mencatatkan performa terendah dengan kontribusi hanya 65K interaksi dan 6,60% ER Reach, menandakan perlunya evaluasi teknis pada strategi distribusi video.
  

### 🎨 Content Format & Distribution Matrix
- The Reach Drivers: Format Thread dan Reels mencatatkan ER Reach tertinggi (25-28%), menjadikannya senjata terbaik untuk mengakuisisi audiens baru.
- The Retention Leaders: Format Carousel serta Text + Image memimpin pada tingkat retensi penonton hingga 68%, membuktikan bahwa audiens sangat meminati isi konten yang mendalam meskipun algoritmanya terbatas.
- Paid Advertising ROI: Pengeluaran anggaran iklan (Ad Spend) terbukti efektif dan sehat. Dorongan promosi berhasil menaikkan nilai ER Reach dari 14,44% (baseline organik) menjadi 16,31%, serta mengerek ER Impressions menjadi 11,11%.


### ⏰ Audience Behavior & Scheduling
Volume interaksi tertinggi terkonsentrasi secara konsisten pada hari Senin (0.23M) dan Kamis (0.17M), sementara hari Rabu (0.02M) menjadi titik jenuh terendah.

### 💡 Strategic Roadmap & Action Plan
- **Amplify Success:** Meningkatkan volume produksi Twitter Threads dan Instagram Reels secara konsisten untuk mempertahankan dominasi jangkauan unik baru.
- **Duplicate Formula:** Mengadopsi struktur storytelling dan pola penahanan retensi video TikTok ke platform lain guna mendongkrak efisiensi konversi (CTR) secara makro.
- **Optimize Hooks:** Melakukan perbaikan teknis pada 5 detik pertama konten YouTube untuk mengatasi tingginya drop-off rate (durasi tonton rendah 44%).
- **Content Scheduling:** Memfokuskan peluncuran konten campaign utama pada hari Senin dan Kamis untuk memanfaatkan waktu emas interaksi audiens.

