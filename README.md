# Qarjy — күнделікті шығындарды есептеу веб-қосымшасы

## Жоба файлдары
- `index.html` — басты бет
- `login.html` — тіркелу және кіру
- `dashboard.html` — негізгі мазмұн / қаржы панелі
- `style.css` — адаптивті дизайн
- `auth.js` — тіркелу және кіру логикасы
- `dashboard.js` — операциялар, баланс, бюджет, әмияндар

## GitHub Pages-ке жариялау
1. GitHub.com → New repository → атауы `qarjy-expenses` → Public → Create repository.
2. Add file → Upload files. Осы папкадағы барлық файлды жүктеп, Commit changes бас.
3. Repository → Settings → Pages.
4. Build and deployment бөлімінде Deploy from a branch таңда.
5. Branch: `main`, Folder: `/(root)` → Save.
6. Бірнеше минуттан кейін GitHub Pages көрсеткен сілтемені аш.

## ER-диаграммамен сәйкестік
- Users: аты, email және кіру деректері.
- Categories: операция санаттары (тамақ, көлік, сауда, жалақы т.б.).
- Wallets: Kaspi, Halyk, қолма-қол әмияндары және баланс.
- Budgets: айлық шығын лимиті (демо-нұсқада 200 000 ₸).
- Transactions: операция түрі, user/category/wallet байланысына арналған өрістер, сома, сипаттама және күн.
- Currencies: демо-нұсқада негізгі валюта — KZT (₸).

**Ескерту:** Бұл — frontend статикалық демо. Мәліметтер браузердің localStorage/sessionStorage жадында сақталады. Нақты MySQL дерекқоры, серверлік авторизация және бірнеше құрылғы арасында синхрондау жоқ. ER-диаграммадағы кестелердің логикасы интерфейсте көрсетілген; толық дерекқор байланыстары backend кезеңінде қосылады.
