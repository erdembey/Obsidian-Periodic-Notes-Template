---
created: <% tp.file.creation_date() %>
mood: 🔴 🟡 🟢
airmood: 🌞 ⛅ 🌧️ ❄️ 
günnerede: 💼 🏫 👨‍👩‍👧 🏡 🆓
tarih: <% tp.file.creation_date("YYYY-MM-DD") %>
---
---
## 📅 Güne Özel Sorular
### 🌜 Bugüne yönelik öngördüklerim ...
- 
---
### 🚀 Bugün gerçekleştirmek istediklerim ...
- [ ] 
---
### 🙌 Bugün dikkatimi çeken konu ...
- 
---
### 👎 Bugün zorlandığım konu ...
- 
---
## 📝 Notlar
-  <% tp.file.cursor() %>
---
## 🏷️ Etiketler
#Düzenli-Notlar/Günlük

---
##  🔗 Bağlantılar
Günlük: < [[<% tp.date.now("DD-MM-YYYY-dddd", -1, tp.file.title, "DD-MM-YYYY-dddd") %>]] | [[<% tp.date.now("DD-MM-YYYY-dddd", 1, tp.file.title, "DD-MM-YYYY-dddd") %>]] >
Haftalık: [[<% tp.date.now("YYYY-[Hafta]-ww", 0, tp.file.title, "DD-MM-YYYY-dddd") %>]]
Aylık: [[<% tp.date.now("YYYY-MMMM", 0, tp.file.title, "DD-MM-YYYY-dddd") %>]]

Güncelleme: `=this.file.mtime`

---
## 📝 Bugün Yazdıklarım
```dataview
list WHERE striptime(file.cday) = date(this.tarih) SORT file.ctime asc
```