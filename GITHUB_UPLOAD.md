# GitHub'a Yükleme Talimatları 🚀

## Adım 1: GitHub Hesabı Oluştur (eğer yoksa)
- https://github.com adresine git
- "Sign up" düğmesine tıkla
- E-mail ve şifreyi gir
- Hesabı doğrula

## Adım 2: Yeni Repository Oluştur

### Web Interface ile:
1. GitHub'a giriş yap
2. Sol tarafta "+" simgesine tıkla → "New repository"
3. Repository adı: `tyt-takip`
4. Açıklama: "TYT sınav sonuçlarını takip etmek için web uygulaması"
5. "Public" seç (herkes görsün diye)
6. **MARKDOWN'İ TIKLA: "Initialize this repository with: Skip this step"** (README'yi kendimiz yapacağız)
7. "Create repository" düğmesine tıkla

### Komut satırı ile:
```bash
gh repo create tyt-takip --public --remote=origin --source=.
```

## Adım 3: Dosyaları Hazırla

1. Bu klasördeki tüm dosyaları al:
   - `index.html` (ana dosya)
   - `README.md` (açıklama)
   - `LICENSE` (MIT Lisansı)
   - `package.json` (bilgi dosyası)
   - `.gitignore` (hangi dosyaların yüklenmeyeceği)

## Adım 4: Git İle Yükle

### Bilgisayarına Git Kur (eğer yoksa):
- https://git-scm.com adresinden indir
- Kur ve yeniden başlat

### Terminal/CMD'de (Bu klasörde):

```bash
# Git'i başlat
git init

# GitHub'daki repository'ini ekle
git remote add origin https://github.com/KULLANICIADIN/tyt-takip.git

# Dosyaları staging area'ya ekle
git add .

# Değişiklikleri commit et
git commit -m "İlk commit: TYT Takip uygulaması"

# GitHub'a yükle
git push -u origin main
```

**Not:** Eğer branch adı "main" değil de "master" ise:
```bash
git push -u origin master
```

## Adım 5: GitHub Pages ile Yayınla (Opsiyonel)

Repository ayarlarında:
1. Settings → Pages
2. "Build and deployment" kısmında:
   - Source: "Deploy from a branch" seç
   - Branch: "main" (veya master)
   - Folder: "/" (root)
3. "Save"

Birkaç dakika sonra şurada erişebilirsin:
```
https://KULLANICIADIN.github.io/tyt-takip
```

## Adım 6: README.md'yi Düzenle (Opsiyonel)

Eğer GitHub'daki README'yi özelleştirmek istersen:
1. Repository'ye git
2. README.md dosyasının yanındaki kalem simgesine tıkla
3. Düzenle ve commit et

## Sık Sorulan Sorular

### Q: Verilerim kaybolur mu?
**A:** Hayır! Veriler tarayıcıda localStorage'da tutulur. Her cihazın kendi verileri vardır.

### Q: Başkalarının verilerine erişebilir mi?
**A:** Hayır! Her kullanıcının verileri kendisinin tarayıcısında tutulur.

### Q: Dosyaları güncellemek istersen?
```bash
git add .
git commit -m "Açıklama yaz"
git push
```

### Q: Repository'yi Private yapmak istersen?
GitHub → Repository Settings → Visibility → Change to Private

---

**Başarılar! TYT Takip uygulamanız GitHub'da yayında! 🎉**
