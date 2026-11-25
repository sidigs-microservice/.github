<div align="center">

<img src="./assets/banner.svg" alt="SIDIGS Microservices — Sekolah Jadi Mudah" width="100%" />

[English](./README.md) · **Bahasa Indonesia**

### Rumah engineering SIDIGS — satu platform untuk menjalankan seluruh sekolah.

Dari pendaftaran hingga rapor, presensi hingga kasir kantin: SIDIGS menghubungkan
yayasan, sekolah, guru, siswa, dan orang tua dalam satu ekosistem terpadu.

<a href="https://sidigs.com"><img src="./assets/btn-website.svg" alt="sidigs.com" height="44" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-architecture"><img src="./assets/btn-architecture.svg" alt="Architecture" height="44" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-service-template"><img src="./assets/btn-template.svg" alt="Service Template" height="44" /></a>

</div>

## 🏫 Apa yang kami bangun

SIDIGS adalah platform sekolah digital yang dipakai **yayasan, sekolah, dan keluarga** di seluruh Indonesia.
Organisasi ini menampung generasi berikutnya: layanan mandiri per domain di balik satu gateway,
dan satu aplikasi web dengan ruang kerja khusus untuk setiap peran.

<img src="./assets/features.id.svg" alt="Yang kami bangun: akademik, penilaian, keuangan, kepegawaian, layanan sekolah, komunikasi" width="100%" />

## 🧭 Arsitektur

<img src="./assets/architecture.svg" alt="Arsitektur: Web App masuk lewat API Gateway, yang meneruskan ke layanan inti dan domain" width="100%" />

**Prinsip yang kami pegang**

- 🧩 **Satu domain, satu layanan, satu database** — setiap layanan memiliki datanya sendiri dan berkomunikasi lewat panggilan antarlayanan yang ditandatangani.
- 🚪 **Satu pintu masuk** — setiap request melewati API Gateway: identitas, tenant, izin akses, dan feature flag.
- 🔐 **Aman sejak awal** — identitas berbasis token (JWKS), izin per rute, kredensial terenkripsi, validasi input di setiap batas.
- 📱 **Mobile first** — sebagian besar pengguna memakai ponsel; setiap halaman harus berfungsi di lebar 375 px.
- 🧪 **Aturan yang teruji** — aturan uang, nilai, dan akses ada di modul kecil yang punya unit test.

## 🗂️ Repositori

<table>
<tr><th colspan="2" align="left">🌐 Front end &amp; gateway</th></tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-web-app"><b>sidigs-web-app</b></a><br/><sub>Aplikasi web dengan ruang kerja untuk setiap peran</sub></td>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-api-gateway"><b>sidigs-api-gateway</b></a><br/><sub>Routing, identitas, tenant, izin akses, feature flag</sub></td>
</tr>
<tr><th colspan="2" align="left">🔑 Layanan inti</th></tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-iam-service"><b>sidigs-iam-service</b></a><br/><sub>Akun, autentikasi, notifikasi, chat</sub></td>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-organization-service"><b>sidigs-organization-service</b></a><br/><sub>Yayasan, sekolah, partner, branding</sub></td>
</tr>
<tr><th colspan="2" align="left">🧩 Layanan domain</th></tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-academic-service"><b>sidigs-academic-service</b></a><br/><sub>Siswa, kelas, kurikulum, presensi, rapor</sub></td>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-exam-service"><b>sidigs-exam-service</b></a><br/><sub>Bank soal, runtime CBT, penilaian</sub></td>
</tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-finance-service"><b>sidigs-finance-service</b></a><br/><sub>Tagihan, pembayaran, e-money, tabungan, akuntansi</sub></td>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-hr-service"><b>sidigs-hr-service</b></a><br/><sub>Pegawai, presensi staf, penggajian, kinerja</sub></td>
</tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-content-service"><b>sidigs-content-service</b></a><br/><sub>Persuratan, pengumuman, dokumen, unggahan</sub></td>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-infrastructure-service"><b>sidigs-infrastructure-service</b></a><br/><sub>Sarpra, perpustakaan, klinik, laundry, pesantren</sub></td>
</tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-canteen-service"><b>sidigs-canteen-service</b></a><br/><sub>Merchant dan kasir kantin</sub></td>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-registration-service"><b>sidigs-registration-service</b></a><br/><sub>Pendaftaran dan onboarding sekolah</sub></td>
</tr>
<tr><th colspan="2" align="left">🧰 Platform &amp; dokumen</th></tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-platform"><b>sidigs-platform</b></a><br/><sub>Runtime lokal, konfigurasi, seed, alat developer</sub></td>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-service-template"><b>sidigs-service-template</b></a><br/><sub>Titik awal setiap layanan baru</sub></td>
</tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-architecture"><b>sidigs-architecture</b></a><br/><sub>Keputusan arsitektur, sumber kebenaran</sub></td>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-api-collection"><b>sidigs-api-collection</b></a><br/><sub>Koleksi API untuk pengujian dan integrasi</sub></td>
</tr>
</table>

## 🛠️ Teknologi

<img src="./assets/tech.svg" alt="Teknologi. Backend: TypeScript, Node.js, NestJS, Better Auth. Frontend: Next.js 16, React, Tailwind CSS v4, Lucide. Data: MySQL 8.4, Prisma, Redis, BullMQ. Kualitas dan CI: Jest, Vitest, ESLint, GitHub Actions." width="100%" />

## 🔄 Cara kami bekerja

<img src="./assets/workflow.svg" alt="Alur kerja: tiket Linear, branch, pull request, CI, review, merge" width="100%" />

- 📋 **Linear** adalah tempat pekerjaan direncanakan dan dilacak. GitHub Issues tidak dipakai.
- 🔍 **Setiap perubahan direview** lewat pull request sebelum di-merge.
- 🤖 **GitHub Actions** menjalankan lint, test, build, dan pemeriksaan keamanan di setiap pull request.
- 🔒 **Tidak ada rahasia di kode** — konfigurasi datang dari environment, tidak pernah dari repositori.
- 📐 **Keputusan penting dicatat** di [`sidigs-architecture`](https://github.com/sidigs-microservice/sidigs-architecture).

---

[<img src="./assets/footer.svg" alt="SIDIGS Engineering — sidigs.com" width="100%" />](https://sidigs.com)
