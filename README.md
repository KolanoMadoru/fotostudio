# Studio Foto Website

Website studio foto profesional yang dibuat dengan HTML, CSS, dan JavaScript vanilla. Website ini dioptimalkan untuk deployment di Netlify.

## 🚀 Deployment di Netlify

Website ini sudah dikonfigurasi untuk deployment otomatis di Netlify dengan fitur-fitur berikut:

### Konfigurasi yang Tersedia:

1. **netlify.toml** - Konfigurasi build dan headers
2. **_redirects** - Handle routing untuk single page application
3. **package.json** - Metadata dan scripts untuk development

### Cara Deployment:

#### Option 1: Drag & Drop
1. Buka [netlify.com](https://netlify.com)
2. Drag & drop folder proyek ini ke area deployment
3. Website akan langsung live

#### Option 2: Git Integration
1. Push kode ke repository GitHub/GitLab/Bitbucket
2. Connect repository ke Netlify
3. Netlify akan otomatis detect sebagai static site
4. Deploy dengan klik tombol "Deploy site"

### Fitur yang Tersedia:

- ✅ Static HTML/CSS/JS hosting
- ✅ HTTPS otomatis
- ✅ Global CDN
- ✅ Continuous deployment
- ✅ Custom domain support
- ✅ Form handling (bisa ditambahkan Netlify Forms)
- ✅ Security headers
- ✅ Cache optimization

## 📁 Struktur File

```
/
├── index.html          # Halaman utama
├── styles.css          # Stylesheet
├── netlify.toml        # Konfigurasi Netlify
├── _redirects          # Routing rules
├── package.json        # Metadata dan scripts
├── .gitignore          # Git ignore rules
└── README.md           # Dokumentasi
```

## 🛠️ Development Lokal

### Cara menjalankan lokal:

```bash
# Option 1: Dengan Python (jika Python 3 terinstall)
python3 -m http.server 8080

# Option 2: Dengan Node.js (jika Node.js terinstall)
npm install
npm start
```

Kemudian buka `http://localhost:8080` di browser.

## 🔧 Konfigurasi Tambahan

### Menambahkan Netlify Forms

Untuk mengaktifkan form handling di Netlify, tambahkan attribute berikut pada form:

```html
<form name="contact" method="POST" data-netlify="true">
  <!-- form fields -->
</form>
```

### Custom Domain

1. Buka dashboard Netlify
2. Pilih Site settings → Domain management → Custom domains
3. Tambahkan domain kustom
4. Update DNS records sesuai instruksi Netlify

### Environment Variables

Untuk menambahkan environment variables:
1. Site settings → Build & deploy → Environment
2. Tambahkan variables yang dibutuhkan

## 📝 Notes

- Website ini adalah static site, tidak memerlukan build process
- Semua asset sudah dioptimalkan untuk production
- Security headers sudah dikonfigurasi
- Cache strategy sudah diatur untuk performa optimal

## 🐛 Troubleshooting

### Common Issues:

1. **404 errors** - Pastikan file `_redirects` sudah ada
2. **CORS issues** - Pastikan external resources menggunakan HTTPS
3. **Form not working** - Tambahkan `data-netlify="true"` pada form
4. **Slow loading** - Periksa ukuran images dan optimasi

### Deployment Logs:

Check deployment logs di dashboard Netlify untuk debugging:
1. Buka site dashboard
2. Deploys → Pilih deployment → View deploy log

## 📞 Support

Jika ada masalah dengan deployment, hubungi:
- Netlify documentation: https://docs.netlify.com
- Netlify support: https://www.netlify.com/contact/