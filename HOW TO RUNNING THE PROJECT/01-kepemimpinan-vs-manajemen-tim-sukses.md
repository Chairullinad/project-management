# Modul 01: Kepemimpinan vs Manajemen dalam Tim yang Sukses (Leadership vs Management in Running Projects)

Ketika sebuah proyek memasuki fase eksekusi (*running the project*), dinamika pekerjaan berubah secara drastis. Rencana di atas kertas, bagan Gantt yang rapi, dan piagam proyek yang telah disahkan harus berhadapan langsung dengan realitas operasional: tenggat waktu yang ketat, bug perangkat lunak yang tak terduga, pergeseran prioritas pemangku kepentingan, dan kelelahan mental tim (*team burnout*).

Di fase inilah terlihat perbedaan mencolok antara manajer yang sekadar "mengatur tugas" (*managing tasks*) dengan pemimpin yang "menggerakkan manusia" (*leading people*). 

Seorang Project Manager (PM) yang sukses harus mampu menjalankan kedua peran ini secara seimbang: memiliki ketelitian sistematis seorang manajer dan karisma empatik seorang pemimpin.

---

## 1. Dikotomi Fundamental: Manajemen vs Kepemimpinan

Meskipun sering digunakan secara bergantian, manajemen dan kepemimpinan memiliki fungsi psikologis dan operasional yang sangat berbeda:

```mermaid
flowchart TD
    subgraph Management["FUNGSI MANAJEMEN (Order & Consistency)"]
        M1["• Perencanaan & Penganggaran Detil<br>• Pengorganisasian & Penempatan Staf<br>• Pengendalian Jadwal & Pemecahan Masalah Taktis<br>• Menegakkan Standar Prosedur Operasional (SOP)<br>• Fokus: 'BAGAIMANA' dan 'KAPAN'"]
    end

    subgraph Leadership["FUNGSI KEPEMIMPINAN (Change & Movement)"]
        L1["• Menetapkan Visi & Arah Strategis Masa Depan<br>• Menyelaraskan Manusia di Balik Tujuan Mulia<br>• Menginspirasi, Memotivasi & Membangun Kepercayaan<br>• Menumbuhkan Ketahanan Mental Saat Krisis Datang<br>• Fokus: 'APA' dan 'MENGAPA'"]
    end

    Management ---|Dibutuhkan Bersamaan dalam Fase Eksekusi| Leadership
```

### Tabel Komparasi Praktis di Lapangan:

| Dimensi Proyek | Pendekatan Manajer Murni | Pendekatan Pemimpin Proyek |
| :--- | :--- | :--- |
| **Menghadapi Rintangan (*Blockers*)** | Menelusuri siapa yang terlambat dan menagih komitmen berdasarkan jadwal Jira. | Duduk bersama anggota tim, mendengarkan akar kesulitan, dan menyingkirkan hambatan lintas divisi. |
| **Penyampaian Target** | *"Kalian harus menyelesaikan modul kasir ini sebelum Jumat sesuai sprint backlog."* | *"Modul kasir ini akan memangkas antrean pasien lansia dari 45 menit menjadi 10 menit. Mari kita wujudkan bersama."* |
| **Terjadi Kesalahan / Bug Kritis** | Mencari siapa yang salah melakukan *commit* kode dan meminta pertanggungjawaban. | Menjalankan *blameless post-mortem*: *"Proses validasi apa yang perlu kita perbaiki agar bug serupa tidak lolos lagi?"* |
| **Hubungan dengan Anggota Tim** | Berdasarkan wewenang hierarkis dan instruksi satu arah (*top-down*). | Berdasarkan pengaruh timbal balik (*reciprocity*), empati, dan *servant leadership*. |

---

## 2. Model Kepemimpinan Situasional Hersey-Blanchard

Tidak ada satu gaya kepemimpinan tunggal yang cocok untuk semua situasi dan semua orang. Gaya kepemimpinan Anda harus beradaptasi dengan **Tingkat Kematangan & Kompetensi Tim (*Development Level*)**:

```mermaid
flowchart LR
    D1["D1: Antusias Tinggi, Kompetensi Rendah<br>(Pegawai Baru / Modul Baru)"] --> S1["S1: Directing (Mengarahkan)<br>Beri instruksi spesifik, panduan langkah demi langkah, supervisi ketat."]
    D2["D2: Antusias Menurun, Kompetensi Rendah-Sedang<br>(Mulai Frustrasi Hadapi Bug Berat)"] --> S2["S2: Coaching (Membimbing)<br>Jelaskan alasan keputusan, dengarkan keluhan, bimbing solusi bersama."]
    D3["D3: Kompetensi Tinggi, Percaya Diri Fluktuatif<br>(Insinyur Ahli tapi Cemas Hadapi Direksi)"] --> S3["S3: Supporting (Mendukung)<br>Fasilitasi diskusi, dorong pengambilan keputusan mandiri, beri dorongan moral."]
    D4["D4: Kompetensi Tinggi, Komitmen Tinggi<br>(Tim Otonom Berkinerja Puncak)"] --> S4["S4: Delegating (Mendelegasikan)<br>Beri wewenang penuh atas solusi teknis, cukup pantau hasil akhir & milestone."]
```

### Panduan Aksi PM:
- **Jangan lakukan Micromanagement pada tim D4**: Mengatur detail penamaan variabel programmer senior akan membunuh motivasi dan memicu kebencian kerja.
- **Jangan lakukan Delegating berlebihan pada tim D1**: Membiarkan staf analis pemula merancang skema database kritis tanpa supervisi akan berujung pada malapetaka teknis.

---

## 3. Fondasi Eksekusi: Keamanan Psikologis (*Psychological Safety*)

Berdasarkan studi komprehensif Google (*Project Aristotle*), faktor pembeda utama antara tim yang sukses dan tim yang gagal bukanlah kecerdasan individu atau alat manajemen tercanggih, melainkan **Rasa Aman Psikologis**.

```mermaid
flowchart TD
    subgraph FearCulture["Budaya Ketakutan (Gagal)"]
        F1["Tim Takut Disalahkan"] --> F2["Menyembunyikan Bug & Keterlambatan"]
        F2 --> F3["Masalah Menumpuk Diam-Diam"]
        F3 --> F4["Meledak Menjadi Krisis P1 Saat Go-Live"]
    end

    subgraph SafeCulture["Budaya Keamanan Psikologis (Sukses)"]
        S1["Tim Merasa Aman Mengakui Error"] --> S2["Lapor Cepat di Daily Standup"]
        S2 --> S3["PM & Tim Kolaborasi Cari Solusi"]
        S3 --> S4["Masalah Tuntas Sebelum Membengkak"]
    end
```

### Indikator Tim yang Memiliki Keamanan Psikologis Tinggi:
1. Anggota tim tidak ragu bertanya: *"Saya belum paham maksud spesifikasi ini, bisakah dijelaskan kembali?"*
2. Pengembang berani mengoreksi PM jika estimasi jadwal tidak realistis.
3. Anggota tim berani mengakui kesalahan tanpa takut dihina atau diancam sanksi karir.

---

## 4. Servant Leadership: Melayani untuk Memimpin

Filosofi *Servant Leadership* (Robert K. Greenleaf) membalik piramida organisasi tradisional. Di mata seorang Servant Leader, **tugas Project Manager adalah melayani kebutuhan tim**, bukan menyuruh tim melayani kemauan PM.

```
PIRAMIDA TRADISIONAL (KUNO):             PIRAMIDA SERVANT LEADERSHIP (MODERN):
        [ PM / Boss ]                                [ PENGGUNA / PASIEN ]
             ▲                                                 ▲
       [ Supervisor ]                                   [ TIM PENGEMBANG ]
             ▲                                                 ▲
   [ Tim Pelaksana Kerja ]                              [ PROJECT MANAGER ]
(Tim melayani instruksi bos)                 (PM menjadi bantalan & pelayan tim)
```

### 3 Tugas Pokok Servant Leader dalam Menjalankan Proyek:
1. **Shielding the Team (Bantalan Politik)**: Melindungi tim pengembang dari interupsi eksternal, perubahan kehendak sepihak dari pejabat manajemen, atau komplain liar yang belum diverifikasi.
2. **Removing Friction (Pembersih Hambatan)**: Mengurus birokrasi izin akses server, memfasilitasi lisensi alat pengembangan, dan memastikan lingkungan kerja tim bebas stres non-teknis.
3. **Amplifying Others (Membesarkan Orang Lain)**: Memberikan panggung penghargaan kepada insinyur dan staf lapangan ketika proyek berhasil, serta mengambil tanggung jawab utama ketika proyek menghadapi kritik dewan.

---

## 5. Studi Kasus Riil: Mengatasi "Project Fatigue" pada Proyek SIMRS

### Konteks Skenario
- **Inisiatif Proyek**: Peluncuran Modul Rekam Medis Elektronik (RME) Rawat Inap & Bridging BPJS Kesehatan.
- **Tantangan Lapangan**:
  - Proyek telah berjalan selama 4 bulan. Tim pengembang dan tim rekam medis mulai mengalami kelelahan mental akut (*project fatigue*).
  - Hubungan kerja memburuk: Pengembang software merasa staf rumah sakit terlalu banyak menuntut revisi kecil, sementara perawat bangsal merasa sistem baru membingungkan dan menambah beban kerja shift malam.
  - Dua insinyur kunci mengajukan cuti panjang karena merasa tidak dihargai dan sering dimarahi saat demo sistem.

### Intervensi Kepemimpinan oleh PM (Dessy Rahmawati Chairullina):

```mermaid
flowchart TD
    Step1["1. Hentikan Tekanan Deadline Sementara (Time-Out 24 Jam)"] --> Step2["2. Reconnecting to Purpose (Melihat Dampak Langsung di Bangsal)"]
    Step2 --> Step3["3. Redefinisi Lingkup & Eliminasi Beban Kerja Semu"]
    Step3 --> Step4["4. Pengakuan Personal & Pemulihan Moral Tim"]
    Step4 --> Result["HASIL: Retensi Tim 100%, Moral Bangkit, Go-Live Sukses Tepat Waktu"]
```

1. **Jeda Kemanusiaan (*Human Time-Out*)**:
   - PM menghentikan sprint selama 1 hari penuh. Seluruh pembicaraan mengenai tiket Jira dan burndown chart dibekukan.
   - Mengadakan sesi makan siang santai di luar area rumah sakit tanpa laptop untuk mendengarkan keluh kesah secara personal.
2. **Menghubungkan Kembali dengan Tujuan Mulia (*Reconnecting to Purpose*)**:
   - PM mengajak dua insinyur perangkat lunak mendampingi perawat jaga malam di ruang rawat intensif (ICU).
   - Insinyur menyaksikan sendiri bagaimana lembaran rekam medis kertas yang tebal dan tercecer membuat perawat kesulitan mencari riwayat alergi obat pasien yang sedang kritis.
   - Momen ini mengubah paradigma insinyur secara radikal: mereka menyadari bahwa kode program yang mereka tulis bukan sekadar baris sintaks Java, melainkan alat penyelamat nyawa manusia.
3. **Penyederhanaan Ruang Lingkup (*De-scoping Non-Essentials*)**:
   - PM bernegosiasi dengan Komite Medis untuk menunda 12 permintaan fitur kosmetik yang tidak mendesak ke rilis fase kedua.
   - Beban kerja tim pengembang berkurang 30%, memungkinkan mereka fokus membereskan stabilitas koneksi data bridging BPJS.
4. **Hasil**:
   - Moral tim pulih total; kedua insinyur membatalkan rencana pengunduran diri.
   - Siklus rilis kembali stabil, dan implementasi modul rawat inap diluncurkan dengan tingkat adopsi perawat mencapai 98% dalam 14 hari pertama.

---

## 6. Actionable Checklist Kepemimpinan Tim Eksekusi

```
[ ] 1. Diagnosa Tingkat Kematangan: Apakah Anda menerapkan gaya kepemimpinan yang sesuai (Directing / Coaching / Supporting / Delegating) untuk setiap anggota tim?
[ ] 2. Cek Keamanan Psikologis: Kapan terakhir kali seorang anggota tim berani mengakui kesalahan atau ketidaktahuannya di depan Anda tanpa takut dihakimi?
[ ] 3. Audit Perisai Tim: Apakah Anda telah menyaring interupsi liar dari pemangku kepentingan luar sebelum mencapai meja kerja tim pengembang?
[ ] 4. Pembersihan Hambatan Harian: Apakah seluruh 'blocker' yang dilaporkan pada daily standup pagi ini sudah memiliki rencana aksi sebelum jam kerja berakhir?
[ ] 5. Apresiasi Spesifik: Apakah Anda telah memuji kontribusi konkret salah satu anggota tim hari ini secara tulus dan spesifik?
```
