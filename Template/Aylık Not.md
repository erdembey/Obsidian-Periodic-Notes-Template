---
created: <% tp.file.creation_date() %>
mood: 🔴 🟡 🟢
---
---
## 📅 Aylık Özel Sorular
### 🌜 Bu aya yönelik düşündüklerim ...
- 
---
### 🙌 Bu ay dikkatimi çeken konular ...
- 
---
### 🚀 Bu ay gerçekleştirmek istediklerim ...
- [ ] 
---
### 👎 Bu ay zorlandığım konu ...
- 
---
## 📝 Notlar
-  <% tp.file.cursor() %>
---

## ⚙️ Bu Ay Tamamlanmamış İşler
```tasks
not done
short mode
path includes <% tp.file.path() %>
group by filename
```


## 🏷️ Etiketler
#Düzenli-Notlar/Aylık

---
##  🔗 Bağlantılar
Çeyrek: [[<% tp.date.now("YYYY-Q", 0, tp.file.title, "YYYY-MMMM") %>]]
Yıllık: [[<% tp.date.now("YYYY", 0, tp.file.title, "YYYY-MMMM") %>]]

Güncelleme: `=this.file.mtime`
