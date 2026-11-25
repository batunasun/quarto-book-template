# Quarto Book Template

Template for creating books with Quarto.

## Create a new book

1. Copy this folder
2. Rename the folder
3. Update `_quarto.yml`
4. Edit `index.qmd`
5. Add chapters
6. Render with

```bash
quarto render




# Quarto Номын Загвар

Quarto, GitHub болон GitHub Pages ашиглан цахим ном бүтээх бэлэн загвар.

## Шинэ ном үүсгэх

### 1. Загварыг ашиглах

GitHub дээрх **Use this template** товчийг дарна.

### 2. Repository-ийн нэр өгөх

Жишээ:

```
discrete-math-book
```

эсвэл

```
forecasting-book
```

### 3. GitHub Pages идэвхжүүлэх

Repository → Settings → Pages

```
Source = GitHub Actions
```

### 4. `_quarto.yml` файлаа засах

```yaml
project:
  type: book
  output-dir: docs

book:
  title: "Миний ном"
  subtitle: "Дэд гарчиг"
```

### 5. `index.qmd` файлаа засах

Номын оршил болон нүүр хуудсын агуулгыг бичнэ.

### 6. Бүлгүүд нэмэх

Жишээ:

```yaml
chapters:
  - index.qmd
  - ch01.qmd
  - ch02.qmd
  - ch03.qmd
```

Шинэ бүлэг бүрийг тусдаа `.qmd` файл болгон үүсгэнэ.

### 7. Номоо нийтлэх

Positron дээр:

1. Файлаа хадгална (`Ctrl+S`)
2. Source Control нээнэ
3. Commit message бичнэ
4. **Commit & Push** дарна

эсвэл терминал ашиглан:

```bash
git add .
git commit -m "Ном шинэчлэв"
git push
```

### 8. Вэб хуудсаа үзэх

GitHub Actions амжилттай ажилласны дараа:

```
https://USERNAME.github.io/REPOSITORY/
```

хаягаар нээгдэнэ.

Жишээ:

```
https://batunasun.github.io/discrete-math-book/
```

эсвэл өөрийн домэйноор:

```
https://meteosociety.org/discrete-math-book/
```

## Төслийн бүтэц

```text
.
├── .github/
│   └── workflows/
│       └── publish.yml
├── images/
├── _quarto.yml
├── index.qmd
├── references.qmd
├── ch01.qmd
├── ch02.qmd
└── ...
```

## Өдөр тутмын ажиллах дараалал

```text
Агуулгаа засах
      ↓
Ctrl + S
      ↓
Commit & Push
      ↓
GitHub Actions
      ↓
Вэб хуудас автоматаар шинэчлэгдэнэ
```

## Түгээмэл алдаа

### docs хавтас үүсэхгүй

```bash
quarto render
```

ажиллуулж шалгана.

### GitHub Actions улаан болох

Actions таб руу орж алдааны мөрийг шалгана.

### Website шинэчлэгдэхгүй байх

GitHub Actions ногоон ✅ болсон эсэхийг шалгана.

---

Амжилт хүсье!
