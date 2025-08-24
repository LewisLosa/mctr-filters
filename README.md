# mctr-filters 
uBlock Origin filtresi ile **MC-TR forumundaki reklamları engelleyin**.  

## 🔧 Nasıl Eklenir?

1. Tarayıcınızda **uBlock Origin** kurulu olmalı.  
2. uBlock simgesine tıklayın → **Dashboard (Kumanda Paneli)** açın.  
3. **My Filters** sekmesine gidin.  
4. Aşağıdaki **Kurallar** bölümündeki kuralları kopyalayın.
5. Ardından ublock eklentisindeki **My Filters** bölümüne yapıştırın
6. Sol üstteki (mavi) **Apply changes** butonuna basın.
7. Tadını çıkarın.

## 📜 Kurallar
```txt
! MC-TR reklam filtresi
! Güncelleme: Ağustos 24, 2025

! Sabit class’lar
www.mc-tr.com##div.reklam-kutu
www.mc-tr.com##.reklam-sidebar
www.mc-tr.com##.popup-reklam
www.mc-tr.com##.sol-reklam

! Scroll
www.mc-tr.com##body:style(overflow: visible !important; height: auto !important; position: static !important;)

! Bazı reklam divleri (fixed kullananlar)
www.mc-tr.com##body > div[style*="position: fixed"][style*="width: 100%"][style*="height: 100%"]

! Reklam containeri
www.mc-tr.com##body > div[id][style="display: block;"]
```
