# WhatsApp Notification Message Templates - Product Donation Flow

Berikut adalah template pesan WhatsApp untuk setiap notifikasi pada alur donasi produk. Silakan copy-paste ke dashboard Qontak dan sesuaikan variabel.

---

## FLOW DIAGRAM

```
1. Donatur Bayar → Notif ke Mitra (ada donasi baru)
2. Relawan Klaim → (pending approval)
3. Admin Approve/Reject → Notif ke Relawan + Notif ke Donatur (diproses)
4. Relawan Jadwal Pickup → Notif ke Mitra (siapkan barang)
5. Relawan Distribusi Selesai → Notif ke Donatur (terima kasih)
```

---

## 1. DONASI DITERIMA - NOTIF KE MITRA
**Recipient:** Mitra (Pemilik Produk)  
**Trigger:** Donatur selesai bayar  
**Template Name:** `donation_paid_to_mitra`

**Sample Content untuk Qontak:**
- `{{1}}` → `Toko Berkah Jaya` (nama mitra)
- `{{2}}` → `Paket Sembako 5kg` (nama produk)
- `{{3}}` → `2` (quantity)
- `{{4}}` → `Rp 150.000` (total)
- `{{5}}` → `24 Desember 2025` (tanggal)

```
Halo {{1}},

Ada kabar baik! Produk Anda telah dibeli untuk donasi 🎉

*Detail Donasi:*
📦 Produk: {{2}}
📊 Jumlah: {{3}} unit
💰 Total: {{4}}
📅 Tanggal: {{5}}

Mohon siapkan produk untuk dijemput oleh relawan. Kami akan menginformasikan jadwal penjemputan secepatnya.

Terima kasih atas partisipasi Anda! 🙏

_Tim Belas Kasih_
```

---

## 2. KLAIM DIPROSES - NOTIF KE DONATUR
**Recipient:** Donatur  
**Trigger:** Admin approve klaim relawan  
**Template Name:** `claim_approved_to_donatur`

**Sample Content untuk Qontak:**
- `{{1}}` → `Budi Santoso` (nama donatur)
- `{{2}}` → `Paket Sembako 5kg` (nama produk)
- `{{3}}` → `Yayasan Peduli Kasih` (nama relawan/organisasi)
- `{{4}}` → `25 Desember 2025` (tanggal approve)

```
Halo {{1}},

Donasi Anda sedang dalam proses penyaluran! ✅

*Detail:*
📦 Produk: {{2}}
🏢 Disalurkan oleh: {{3}}
📅 Tanggal Proses: {{4}}

Relawan kami akan segera menjemput dan menyalurkan donasi Anda kepada yang membutuhkan.

Terima kasih atas kepedulian Anda! ❤️

_Tim Belas Kasih_
```

---

## 3. KLAIM DISETUJUI - NOTIF KE RELAWAN
**Recipient:** Relawan  
**Trigger:** Admin approve klaim  
**Template Name:** `claim_approved_to_relawan`

**Sample Content untuk Qontak:**
- `{{1}}` → `Ahmad Relawan` (nama relawan)
- `{{2}}` → `Paket Sembako 5kg` (nama produk)
- `{{3}}` → `2` (quantity)
- `{{4}}` → `Toko Berkah Jaya` (nama mitra)
- `{{5}}` → `081234567890` (no HP mitra)

```
Halo {{1}},

Klaim Anda telah disetujui! 🎉

*Detail Donasi:*
📦 Produk: {{2}}
📊 Jumlah: {{3}} unit
🏪 Lokasi Pickup: {{4}}
📞 Kontak Mitra: {{5}}

Silakan atur jadwal penjemputan dengan mitra dan pastikan tim Anda siap untuk distribusi.

Terima kasih sudah menjadi relawan! 🙏

_Tim Belas Kasih_
```

---

## 4. KLAIM DITOLAK - NOTIF KE RELAWAN
**Recipient:** Relawan  
**Trigger:** Admin reject klaim  
**Template Name:** `claim_rejected_to_relawan`

**Sample Content untuk Qontak:**
- `{{1}}` → `Ahmad Relawan` (nama relawan)
- `{{2}}` → `Paket Sembako 5kg` (nama produk)
- `{{3}}` → `Lokasi tidak sesuai dengan jangkauan tim` (alasan)

```
Halo {{1}},

Mohon maaf, klaim Anda untuk donasi produk *{{2}}* belum dapat disetujui ❌

*Alasan:*
{{3}}

Silakan ajukan klaim untuk donasi lain yang sesuai dengan kapasitas tim Anda.

Terima kasih atas pengertian Anda 🙏

_Tim Belas Kasih_
```

---

## 5. JADWAL PENJEMPUTAN - NOTIF KE MITRA
**Recipient:** Mitra  
**Trigger:** Relawan atur jadwal pickup  
**Template Name:** `pickup_schedule_to_mitra`

**Sample Content untuk Qontak:**
- `{{1}}` → `Toko Berkah Jaya` (nama mitra)
- `{{2}}` → `Paket Sembako 5kg` (nama produk)
- `{{3}}` → `2` (quantity)
- `{{4}}` → `Yayasan Peduli Kasih` (nama relawan)
- `{{5}}` → `26 Desember 2025, 10:00 WIB` (tanggal & waktu)
- `{{6}}` → `081298765432` (no HP relawan)

```
Halo {{1}},

Jadwal penjemputan donasi telah ditentukan! 📅

*Detail Penjemputan:*
📦 Produk: {{2}}
📊 Jumlah: {{3}} unit
🏢 Dijemput oleh: {{4}}
🕐 Waktu: {{5}}
📞 Kontak Relawan: {{6}}

Mohon siapkan produk sesuai jadwal. Hubungi relawan jika ada perubahan.

Terima kasih! 🙏

_Tim Belas Kasih_
```

---

## 6. PENJEMPUTAN SELESAI - NOTIF KE MITRA (OPSIONAL)
**Recipient:** Mitra  
**Trigger:** Relawan confirm pickup  
**Template Name:** `pickup_completed_to_mitra`

**Sample Content untuk Qontak:**
- `{{1}}` → `Toko Berkah Jaya` (nama mitra)
- `{{2}}` → `Paket Sembako 5kg` (nama produk)
- `{{3}}` → `26 Desember 2025, 10:30 WIB` (waktu pickup)

```
Halo {{1}},

Penjemputan donasi telah selesai! ✅

*Detail:*
📦 Produk: {{2}}
🕐 Waktu Pickup: {{3}}

Donasi Anda akan segera disalurkan kepada yang membutuhkan.

Terima kasih atas kontribusi Anda! ❤️

_Tim Belas Kasih_
```

---

## 7. DISTRIBUSI SELESAI - NOTIF KE DONATUR
**Recipient:** Donatur  
**Trigger:** Relawan selesai distribusi  
**Template Name:** `distribution_completed_to_donatur`

**Sample Content untuk Qontak:**
- `{{1}}` → `Budi Santoso` (nama donatur)
- `{{2}}` → `Paket Sembako 5kg` (nama produk)
- `{{3}}` → `2` (quantity)
- `{{4}}` → `Yayasan Peduli Kasih` (nama relawan)
- `{{5}}` → `27 Desember 2025` (tanggal selesai)

```
Halo {{1}},

Donasi Anda telah berhasil disalurkan! 🎉

*Detail:*
📦 Produk: {{2}}
📊 Jumlah: {{3}} unit
🏢 Disalurkan oleh: {{4}}
📅 Tanggal: {{5}}

Terima kasih atas kepedulian Anda. Bersama kita membawa kebaikan! ❤️

_Tim Belas Kasih_
```

---

## 8. DONASI DIBATALKAN - NOTIF KE MITRA (OPSIONAL)
**Recipient:** Mitra  
**Trigger:** Admin batalkan donasi  
**Template Name:** `donation_cancelled_to_mitra`

**Sample Content untuk Qontak:**
- `{{1}}` → `Toko Berkah Jaya` (nama mitra)
- `{{2}}` → `Paket Sembako 5kg` (nama produk)
- `{{3}}` → `Pembayaran gagal diverifikasi` (alasan)

```
Halo {{1}},

Donasi untuk produk *{{2}}* telah dibatalkan.

*Alasan:*
{{3}}

Produk Anda kembali tersedia untuk donasi berikutnya.

Terima kasih 🙏

_Tim Belas Kasih_
```

---

## 9. REMINDER KLAIM BELUM DIJEMPUT - NOTIF KE RELAWAN (OPSIONAL)
**Recipient:** Relawan  
**Trigger:** 3 hari setelah approve, belum pickup  
**Template Name:** `pickup_reminder_to_relawan`

**Sample Content untuk Qontak:**
- `{{1}}` → `Ahmad Relawan` (nama relawan)
- `{{2}}` → `Paket Sembako 5kg` (nama produk)
- `{{3}}` → `Toko Berkah Jaya` (nama mitra)
- `{{4}}` → `081234567890` (no HP mitra)

```
Halo {{1}},

Reminder: Donasi *{{2}}* menunggu penjemputan ⏰

*Detail:*
📦 Produk: {{2}}
🏪 Lokasi: {{3}}
📞 Kontak: {{4}}

Mohon segera koordinasi jadwal penjemputan agar donasi dapat disalurkan tepat waktu.

Terima kasih! 🙏

_Tim Belas Kasih_
```

---

## ENVIRONMENT VARIABLES YANG DIBUTUHKAN

Tambahkan di file `.env`:

```env
# WhatsApp Templates - Product Donation Flow
QONTAK_TEMPLATE_DONATION_PAID_TO_MITRA=template_id_dari_qontak
QONTAK_TEMPLATE_CLAIM_APPROVED_TO_DONATUR=template_id_dari_qontak
QONTAK_TEMPLATE_CLAIM_APPROVED_TO_RELAWAN=template_id_dari_qontak
QONTAK_TEMPLATE_CLAIM_REJECTED_TO_RELAWAN=template_id_dari_qontak
QONTAK_TEMPLATE_PICKUP_SCHEDULE_TO_MITRA=template_id_dari_qontak
QONTAK_TEMPLATE_PICKUP_COMPLETED_TO_MITRA=template_id_dari_qontak
QONTAK_TEMPLATE_DISTRIBUTION_COMPLETED_TO_DONATUR=template_id_dari_qontak
QONTAK_TEMPLATE_DONATION_CANCELLED_TO_MITRA=template_id_dari_qontak
QONTAK_TEMPLATE_PICKUP_REMINDER_TO_RELAWAN=template_id_dari_qontak
```

---

## CATATAN PENTING

1. **Variabel menggunakan angka**: `{{1}}`, `{{2}}`, `{{3}}`, dst (sesuai format Qontak)
2. **Setiap template dimulai dari {{1}}** (tidak melanjutkan dari template sebelumnya)
3. **Sample content** harus diisi di dashboard Qontak saat buat template
4. **Emoji** boleh digunakan di template WhatsApp
5. **Bold text** menggunakan `*text*` (markdown WhatsApp)
6. **Line break** otomatis dihandle oleh Qontak

---

## PRIORITAS IMPLEMENTASI

### Phase 1 - Critical (Harus ada):
1. ✅ Donasi Paid → Notif ke Mitra
2. ✅ Klaim Approved → Notif ke Donatur
3. ✅ Klaim Approved → Notif ke Relawan
4. ✅ Klaim Rejected → Notif ke Relawan
5. ✅ Distribusi Selesai → Notif ke Donatur

### Phase 2 - Important (Sangat disarankan):
6. Jadwal Pickup → Notif ke Mitra
7. Pickup Selesai → Notif ke Mitra

### Phase 3 - Optional (Tambahan):
8. Donasi Cancelled → Notif ke Mitra
9. Reminder Pickup → Notif ke Relawan
