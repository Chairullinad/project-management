# Modul 08: Setting SMART Goals & OKRs
## Google Project Management Professional Certificate

> **Sumber Materi**: [Cara Menetapkan Tujuan SMART dan Mendapatkan Hasil | Sertifikat Manajemen Proyek Google](https://www.youtube.com/watch?v=1eiTXSkKFtE)  
> **Kategori**: Course 2 — Project Initiation: Starting a Successful Project (Module 3)  
> **Disusun oleh**: Dessy Rahmawati Chairullina, S.Kom  

---

## 📌 Executive Summary
1. **Bahaya Tujuan yang Kabur (*Vague Goals*)**: Tujuan seperti *"memperbaiki sistem"* atau *"meningkatkan efisiensi"* tidak dapat dievaluasi keberhasilannya, membingungkan tim pelaksana, dan memicu sengketa serah terima proyek.
2. **Kerangka Kerja SMART Goals**: Standar baku perumusan sasaran proyek yang *Specific* (Spesifik), *Measurable* (Terukur), *Attainable* (Dapat Dicapai), *Relevant* (Relevan dengan Visi Bisnis), dan *Time-bound* (Memiliki Tenggat Waktu Jelas).
3. **Penyelarasan dengan OKR (Objectives & Key Results)**: Metodologi penetapan sasaran strategis Google yang menghubungkan visi kualitatif ambisius (*Objective*) dengan 2–4 tolok ukur kuantitatif numerik (*Key Results*).
4. **Indikator Leading vs Lagging**: Mengukur aktivitas pendorong proses (*Leading*) untuk memprediksi dan memastikan tercapainya hasil akhir (*Lagging*).

---

## 1. Anatomi Kerangka Kerja SMART Goals

Setiap sasaran proyek harus lolos uji filter 5 kriteria SMART sebelum dimasukkan ke dalam Project Charter atau dokumen perencanaan.

```mermaid
flowchart LR
    S["SPECIFIC<br>Apa yang ingin dicapai,<br>siapa yang terlibat, & di mana?"] --> M["MEASURABLE<br>Berapa angkanya,<br>persentasenya, atau metriknya?"]
    M --> A["ATTAINABLE<br>Apakah realistis dengan<br>sumber daya & waktu yang ada?"]
    A --> R["RELEVANT<br>Apakah mendukung prioritas<br>strategis organisasi saat ini?"]
    R --> T["TIME-BOUND<br>Kapan tanggal pasti<br>tenggat waktu penyelesaiannya?"]
```

### Perbandingan Tujuan Lemah vs SMART:
| Komponen | Rumusan Lemah (Non-SMART) | Rumusan SMART Standar Google |
| :--- | :--- | :--- |
| **Pendaftaran Pasien** | "Mempercepat antrean pendaftaran pasien rawat jalan." | "Memangkas rata-rata waktu tunggu antrean admisi rawat jalan dari 25 menit menjadi $\le$ 7 menit per pasien per 31 Maret 2027 melalui peluncuran kiosk mandiri." |
| **Rekonsiliasi Klaim** | "Memperbaiki proses pencocokan piutang BPJS." | "Mencapai 100% rekonsiliasi otomatis data FPK BPJS dengan catatan billing kasir dengan selisih nominal Rp 0 dalam waktu 1x24 jam pasca-berkas diunggah." |
| **Kepatuhan Berkas** | "Meningkatkan kelengkapan rekam medis perawat." | "Meningkatkan angka kelengkapan pengisian asesmen risiko jatuh bangsal rawat inap dari 62% menjadi $\ge$ 98% sebelum survei akreditasi KARS 15 Mei 2027." |

---

## 2. Metodologi OKR (Objectives and Key Results)

Google mempopulerkan OKR untuk menjembatani visi level eksekutif dengan deliverable proyek teknis di lapangan.

* **Objective (Kualitatif & Menginspirasi)**: Menyatakan *ke mana* proyek ingin membawa organisasi. Bersifat ringkas, berani, dan memotivasi tim.
* **Key Results (Kuantitatif & Terukur)**: Menyatakan *bagaimana kita tahu* bahwa tujuan tersebut telah tercapai. Wajib memuat angka atau persentase baseline dan target.

```text
[ CONTOH OKR TINGKAT DEPARTEMEN IT & SIMRS ]
Objective:
Membangun infrastruktur rekam medis digital yang andal, cepat, dan sepenuhnya patuh 
terhadap standarisasi Kemenkes SATUSEHAT.

Key Results:
• KR 1: 100% data kunjungan rawat jalan dan inap terkirim ke platform SATUSEHAT 
        dengan response time API < 500 ms.
• KR 2: Menurunkan tingkat galat validasi payload JSON dari 14.2% menjadi < 0.5%.
• KR 3: Mempertahankan uptime ketersediaan server database SIMRS pada angka 99.95% 
        selama jam operasional rumah sakit.
```

---

## 3. Leading Indicators vs Lagging Indicators

Manajer Proyek yang hebat tidak hanya menunggu laporan akhir (*Lagging*), tetapi aktif memantau indikator pendorong harian (*Leading*).

| Tipe Indikator | Karakteristik | Contoh Kasus (Modul Rekam Medis) |
| :--- | :--- | :--- |
| **Lagging Indicator** (Hasil Akhir) | Mudah diukur, namun terlambat diintervensi jika gagal karena kejadian sudah lewat. | Angka kelulusan audit rekam medis 100% pada akhir tahun. |
| **Leading Indicator** (Pendorong Aksi) | Dapat dipantau dan diintervensi setiap hari untuk menjamin tercapainya *lagging indicator*. | Jumlah perawat yang menyelesaikan simulasi form EWS harian; jumlah baris kode yang lolos *automated testing* per sprint. |

---

## 4. Studi Kasus Nyata: Mengubah Target Abstrak Direksi Menjadi SMART Deliverable

* **Tantangan**: Direktur Rumah Sakit memberikan instruksi singkat kepada tim PM: *"Saya ingin modul pembagian Jasa Medis dokter kita diperbaiki agar tidak ada lagi dokter yang komplain ke ruangan saya setiap tanggal 5!"*.
* **Tindakan PM**:
  1. *Bedah Masalah & Baseline*: PM menganalisis data historis dan menemukan bahwa setiap bulan terdapat rata-rata 34 komplain dokter terkait ketidakjelasan potongan farmasi dan keterlambatan pencairan jasa hingga 18 hari kerja.
  2. *Perumusan SMART Goal Proyek*:
     * **S**: Membangun modul *Kalkulator Jasa Medis Otomatis* yang terintegrasi langsung dengan verifikasi kasir dan sistem akuntansi.
     * **M**: Menurunkan angka komplain dari 34 kasus menjadi $\le$ 2 kasus/bulan, dan memangkas waktu kalkulasi dari 18 hari menjadi 2 hari kerja.
     * **A**: Menggunakan infrastruktur database MySQL dan Java Swing internal yang sudah ada tanpa membeli server baru.
     * **R**: Menyelaraskan dengan prioritas direksi untuk menjaga retensi dokter spesialis kunci.
     * **T**: Sistem harus *go-live* dan siap digunakan untuk tutup buku periode gaji 25 Januari 2027.
* **Hasil**:
  * Proyek memiliki tolok ukur sukses yang disepakati hitam di atas putih oleh Direksi dan Komite Medis.
  * Pada tutup buku pertama, komplain dokter turun menjadi 0 kasus karena transparansi rincian tindakan dapat dilihat langsung di sistem.

---

## 5. 🛠️ Actionable SMART Goal Setting Checklist

- [ ] **No Jargon/Vagueness**: Apakah rumusan sasaran bebas dari kata-kata abstrak seperti "optimal", "cepat", atau "lebih baik"?
- [ ] **Baseline Identified**: Apakah kita sudah tahu angka awal saat ini (*current baseline*) sebelum menentukan angka target baru?
- [ ] **Hard Deadline**: Apakah tenggat waktu menyebutkan tanggal, bulan, dan tahun spesifik (bukan sekadar "kuartal depan")?
- [ ] **Resource Alignment**: Apakah target angka realistis dicapai dengan alokasi tim, kapasitas komputasi, dan anggaran yang ada?
- [ ] **Executive Sign-Off**: Apakah sasaran SMART ini sudah disetujui secara tertulis oleh Project Sponsor?
