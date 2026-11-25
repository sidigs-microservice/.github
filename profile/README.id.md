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

<div align="center">

<img src="./assets/repos/group-front.svg" alt="FRONT END & EDGE" width="100%" />

<a href="https://github.com/sidigs-microservice/sidigs-web-app"><img src="./assets/repos/sidigs-web-app.svg" alt="sidigs-web-app: Next.js · every role" width="49%" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-api-gateway"><img src="./assets/repos/sidigs-api-gateway.svg" alt="sidigs-api-gateway: routing · auth · flags" width="49%" /></a>

<a href="https://github.com/sidigs-microservice/sidigs-attendance-ingress-service"><img src="./assets/repos/sidigs-attendance-ingress-service.svg" alt="sidigs-attendance-ingress-service (in development): RFID · device attendance" width="49%" /></a>

<img src="./assets/repos/group-core.svg" alt="CORE SERVICES" width="100%" />

<a href="https://github.com/sidigs-microservice/sidigs-iam-service"><img src="./assets/repos/sidigs-iam-service.svg" alt="sidigs-iam-service: accounts · auth · chat" width="49%" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-organization-service"><img src="./assets/repos/sidigs-organization-service.svg" alt="sidigs-organization-service: foundations · schools" width="49%" /></a>

<img src="./assets/repos/group-domain.svg" alt="DOMAIN SERVICES" width="100%" />

<a href="https://github.com/sidigs-microservice/sidigs-academic-service"><img src="./assets/repos/sidigs-academic-service.svg" alt="sidigs-academic-service: classes · attendance · report cards" width="49%" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-exam-service"><img src="./assets/repos/sidigs-exam-service.svg" alt="sidigs-exam-service: question bank · CBT · scoring" width="49%" /></a>

<a href="https://github.com/sidigs-microservice/sidigs-finance-service"><img src="./assets/repos/sidigs-finance-service.svg" alt="sidigs-finance-service: bills · e-money · accounting" width="49%" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-hr-service"><img src="./assets/repos/sidigs-hr-service.svg" alt="sidigs-hr-service: staff · attendance · payroll" width="49%" /></a>

<a href="https://github.com/sidigs-microservice/sidigs-content-service"><img src="./assets/repos/sidigs-content-service.svg" alt="sidigs-content-service: letters · announcements · files" width="49%" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-infrastructure-service"><img src="./assets/repos/sidigs-infrastructure-service.svg" alt="sidigs-infrastructure-service: library · clinic · facilities" width="49%" /></a>

<a href="https://github.com/sidigs-microservice/sidigs-canteen-service"><img src="./assets/repos/sidigs-canteen-service.svg" alt="sidigs-canteen-service: merchants · point of sale" width="49%" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-registration-service"><img src="./assets/repos/sidigs-registration-service.svg" alt="sidigs-registration-service: school onboarding" width="49%" /></a>

<a href="https://github.com/sidigs-microservice/sidigs-pkl-service"><img src="./assets/repos/sidigs-pkl-service.svg" alt="sidigs-pkl-service (in development): internships (PKL)" width="49%" /></a>

<img src="./assets/repos/group-platform.svg" alt="PLATFORM & DOCS" width="100%" />

<a href="https://github.com/sidigs-microservice/sidigs-platform"><img src="./assets/repos/sidigs-platform.svg" alt="sidigs-platform: local runtime · seeds · tooling" width="49%" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-service-template"><img src="./assets/repos/sidigs-service-template.svg" alt="sidigs-service-template: starter for every new service" width="49%" /></a>

<a href="https://github.com/sidigs-microservice/sidigs-architecture"><img src="./assets/repos/sidigs-architecture.svg" alt="sidigs-architecture: decisions · source of truth" width="49%" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-api-collection"><img src="./assets/repos/sidigs-api-collection.svg" alt="sidigs-api-collection: API collections · testing" width="49%" /></a>

</div>

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
