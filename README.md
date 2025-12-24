
## 1. Donasi Diterima (Donor)
**Template Name:** `product_donation_received`

**Sample Content untuk Qontak:**
- `{{donor_name}}` → `Budi Santoso`
- `{{product_name}}` → `Paket Sembako 5kg`
- `{{donation_code}}` → `DON-2024-001`
- `{{donation_date}}` → `24 Desember 2025`

```
Halo {{donor_name}},

Terima kasih atas donasi produk Anda: *{{product_name}}*.
Donasi Anda telah kami terima dan sedang diproses oleh tim Belas Kasih.

Kode Donasi: {{donation_code}}
Tanggal Donasi: {{donation_date}}

Kami akan menginformasikan perkembangan selanjutnya melalui WhatsApp ini.

Salam hangat,
Tim Belas Kasih
```

---

## 2. Donasi Diklaim Mitra (Donor)
**Template Name:** `product_donation_claimed`

**Sample Content untuk Qontak:**
- `{{donor_name}}` → `Budi Santoso`
- `{{product_name}}` → `Paket Sembako 5kg`
- `{{mitra_name}}` → `Yayasan Peduli Kasih`
- `{{donation_code}}` → `DON-2024-001`
- `{{claim_date}}` → `25 Desember 2025`

```
Halo {{donor_name}},

Donasi produk Anda: *{{product_name}}* telah diklaim oleh mitra kami: {{mitra_name}}.

Kode Donasi: {{donation_code}}
Tanggal Klaim: {{claim_date}}

## 3. Donasi Disetujui (Mitra)
**Template Name:** `product_claim_approved`

**Sample Content untuk Qontak:**
- `{{mitra_name}}` → `Yayasan Peduli Kasih`
- `{{product_name}}` → `Paket Sembako 5kg`
- `{{donation_code}}` → `DON-2024-001`
- `{{approval_date}}` → `25 Desember 2025`

```
Halo {{mitra_name}},

Pengajuan klaim Anda untuk donasi produk *{{product_name}}* telah disetujui.

Kode Donasi: {{donation_code}}
Tanggal Persetujuan: {{approval_date}}

Silakan menunggu informasi jadwal pengambilan/pengiriman.

Terima kasih telah menjadi bagian dari Belas Kasih.
```
Kode Donasi: {{donation_code}}
Tanggal Persetujuan: {{approval_date}}

Silakan menunggu informasi jadwal pengambilan/pengiriman.
## 4. Donasi Ditolak (Mitra)
**Template Name:** `product_claim_rejected`

**Sample Content untuk Qontak:**
- `{{mitra_name}}` → `Yayasan Peduli Kasih`
- `{{product_name}}` → `Paket Sembako 5kg`
- `{{donation_code}}` → `DON-2024-001`
- `{{rejection_reason}}` → `Lokasi penerima tidak sesuai dengan jangkauan mitra`

```
Halo {{mitra_name}},

Mohon maaf, klaim Anda untuk donasi produk *{{product_name}}* dengan kode {{donation_code}} belum dapat kami setujui.

Alasan penolakan: {{rejection_reason}}

Silakan hubungi tim Belas Kasih untuk informasi lebih lanjut.
```
Mohon maaf, klaim Anda untuk donasi produk *{{product_name}}* dengan kode {{donation_code}} belum dapat kami setujui.

Alasan penolakan: {{rejection_reason}}
## 5. Jadwal Pengambilan/Pengiriman (Donor & Mitra)
**Template Name:** `product_pickup_schedule`

**Sample Content untuk Qontak:**
- `{{recipient_name}}` → `Budi Santoso`
- `{{product_name}}` → `Paket Sembako 5kg`
- `{{donation_code}}` → `DON-2024-001`
- `{{pickup_or_delivery}}` → `pengambilan`
- `{{pickup_date}}` → `26 Desember 2025, 10:00 WIB`
- `{{pickup_location}}` → `Jl. Merdeka No. 123, Jakarta Pusat`

```
Halo {{recipient_name}},

Donasi produk *{{product_name}}* dengan kode {{donation_code}} akan dijadwalkan untuk {{pickup_or_delivery}} pada:
Tanggal: {{pickup_date}}
Lokasi: {{pickup_location}}

Pastikan Anda siap pada waktu dan tempat yang telah ditentukan.

Terima kasih atas partisipasi Anda.
```ggal: {{pickup_date}}
Lokasi: {{pickup_location}}
## 6. Donasi Selesai/Didistribusikan (Donor & Mitra)
**Template Name:** `product_donation_completed`

**Sample Content untuk Qontak:**
- `{{recipient_name}}` → `Budi Santoso`
- `{{product_name}}` → `Paket Sembako 5kg`
- `{{donation_code}}` → `DON-2024-001`

```
Halo {{recipient_name}},

Donasi produk *{{product_name}}* dengan kode {{donation_code}} telah berhasil didistribusikan.

Terima kasih telah menjadi bagian dari kebaikan bersama Belas Kasih.

Salam hangat,
## 7. Donasi Dibatalkan (Donor & Mitra)
**Template Name:** `product_donation_cancelled`

**Sample Content untuk Qontak:**
- `{{recipient_name}}` → `Budi Santoso`
- `{{product_name}}` → `Paket Sembako 5kg`
- `{{donation_code}}` → `DON-2024-001`

```
Halo {{recipient_name}},

Donasi produk *{{product_name}}* dengan kode {{donation_code}} telah dibatalkan.

Jika ada pertanyaan, silakan hubungi tim Belas Kasih.

Terima kasih.
```

## 7. Donasi Dibatalkan (Donor & Mitra)
**Template Name:** `product_donation_cancelled`

```
Halo {{recipient_name}},

Donasi produk *{{product_name}}* dengan kode {{donation_code}} telah dibatalkan.

Jika ada pertanyaan, silakan hubungi tim Belas Kasih.

Terima kasih.
```

---

> **Catatan:**
> - Ganti variabel dalam kurung kurawal (misal: {{donor_name}}, {{product_name}}) dengan data dinamis dari sistem.
> - Template name dapat digunakan sebagai referensi di dashboard Qontak dan pada konfigurasi aplikasi.
> - Silakan sesuaikan gaya bahasa sesuai kebutuhan brand.
