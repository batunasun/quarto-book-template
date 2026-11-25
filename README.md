# Quarto Book Template

Шинэ цахим ном (Quarto HTML Book) үүсгэж, GitHub Pages дээр автоматаар нийтлэх загвар.

## Шинэ ном үүсгэх дараалал (5 алхам)

1. **GitHub дээр шинэ репозитори үүсгэх:**
   - Энэ хуудасны баруун дээд буланд байрлах **Use this template** $\rightarrow$ **Create a new repository** дарна.
   - Шинэ номынхоо нэрийг өгнө (жишээ нь: `induc-book`).

2. **Компьютер дээрээ татаж авах (Clone):**
   - Positron дээр **Terminal** нээж, богино замтай хавтас руу орно (`D:\Documents\positron`):
     ```powershell
     cd D:\Documents\positron
     git clone [https://github.com/batunasun/](https://github.com/batunasun/)<шинэ-номын-нэр>.git
     ```

3. **Номын мэдээлэл болон бүлгүүдийг шинэчлэх:**
   - `_quarto.yml` файл доторх номын гарчиг (`title`), зохиогч (`author`), бүлгийн жагсаалт (`chapters`)-ыг өөрчилнө.
   - `index.qmd` болон бүлгийн `.qmd` файлуудаа бичнэ / хуулна.
   - Зургуудыг `images/` хавтсанд хийнэ.

4. **GitHub дээр автомат нийтлэх тохиргоог 1 удаа асаах:**
   - Шинэ репозиторийн **Settings $\rightarrow$ Actions $\rightarrow$ General** хэсэгт **Read and write permissions**-ийг сонгож **Save** дарна.
   - **Settings $\rightarrow$ Pages** хэсэгт **Branch** дээр **`gh-pages`** (`/ (root)`) сонгож **Save** дарна (эхний `push`-ийн дараа `gh-pages` салбар автоматаар үүснэ).

5. **Нийтлэх ба шинэчлэх:**
   - Локал дээр урьдчилан харах бол: `quarto preview`
   - Веб хуудсыг шинэчлэх бол Positron дээр зөвхөн **Commit & Push** дарна (GitHub Actions автоматаар хөрвүүлж нийтэлнэ).
