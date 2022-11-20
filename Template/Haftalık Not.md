---
created: <% tp.file.creation_date() %>
mood: 🔴 🟡 🟢
---
---
## 📅 Haftaya Özel Sorular
### 🌜 Bu haftaya yönelik düşündüklerim ...
- 
---
### 🚀 Bu hafta gerçekleştirmek istediklerim ...
- [ ] 
---
### 🙌 Bu hafta dikkatimi çeken konular ...
- 
---
### 👎 Bu hafta zorlandığım konu ...
- 
---
## 📝 Notlar
-  <% tp.file.cursor() %>
---
## 📝 Bu Haftanın Notları
```dataview
LIST FROM [[]] where contains(file.folder, this.file.folder)
```

## 🏷️ Etiketler
#Düzenli-Notlar/Haftalık

---
##  🔗 Bağlantılar
Aylık: [[<% tp.date.now("YYYY-MMMM", 0, tp.file.title, "YYYY-[Hafta]-ww") %>]]
Çeyrek: [[<% tp.date.now("YYYY-Q", 0, tp.file.title, "YYYY-[Hafta]-ww") %>]]
Yıllık: [[<% tp.date.now("YYYY", 0, tp.file.title, "YYYY-[Hafta]-ww") %>]]

Güncelleme: `=this.file.mtime`
