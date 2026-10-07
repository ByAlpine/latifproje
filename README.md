# GitHub Pages Yayınlama Rehberi

Bu proje tek sayfalık bir HTML sitesidir ve GitHub Pages ile yayınlanabilir.

## 1) GitHub üzerinde repository oluştur

1. GitHub'a giriş yapın.
2. "New repository" seçin.
3. Repository adını yazın.
4. Public veya Private seçin.
5. "Create repository" butonuna basın.

## 2) Yerel klasörü GitHub'a bağla

Aşağıdaki komutları terminalde çalıştırın:

```bash
git init
git branch -M main
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/KULLANICI_ADINIZ/REPO_ADI.git
git push -u origin main
```

## 3) GitHub Pages'i aktifleştir

1. GitHub repository sayfasında "Settings" sekmesine gidin.
2. "Pages" menüsüne tıklayın.
3. "Build and deployment" altında "Source" olarak "GitHub Actions" seçin.
4. Dosya olarak `.github/workflows/deploy-pages.yml` hazırdır.
5. İlk push sonrası otomatik olarak yayınlanacaktır.

## 4) Yayın linki

Yayın adresi şu formatta olur:

```text
https://KULLANICI_ADINIZ.github.io/REPO_ADI/
```

## 5) Yerelde kontrol etme

```bash
python -m http.server 8000
```

Ardından tarayıcıda:

```text
http://localhost:8000
```

adresini açın.
