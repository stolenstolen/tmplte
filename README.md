# Проект

Быстрый клон без инициализации git (копия без истории):

```bash
npx degit https://github.com/<githubUser>/<project> my-project
cd my-project
```

Инструкции по клонированию, установке зависимостей и базовому просмотру проекта.

**Требования**

- Node.js (рекомендуется v18+)
- npm (входит в комплект Node) или `pnpm` / `yarn`
- git (только если хотите иметь историю репозитория)

**Клонирование репозитория (обычный способ)**

```bash
git clone <repository-url>
cd template
```

**Установка зависимостей**

```bash
npm install
# или
# pnpm install
# yarn install
```

**Просмотр проекта**

В текущей конфигурации сборщика (bundler) нет — поэтому:

- можно открыть `index.html` напрямую в браузере (простые статические страницы);
- или запустить лёгкий статический сервер, например:

```
npm install
npm run dev
```


```bash
# открыть файл в macOS
open index.html

# или запустить простой http сервер в папке проекта
npx http-server -c-1 .

# или
npx serve .
```


**Структура проекта (кратко)**

- `index.html` — входной HTML-файл
- `src/index.js` — точка входа JavaScript
- `src/style.css`, `src/reset.css` — основные стили
- `src/assets/` — изображения, иконки и прочие ассеты
- `components/` — компоненты проекта
- `public/` — статические файлы (например, шрифты)
- `stylelint.config.js` — конфигурация Stylelint
- `package.json` — зависимости и скрипты

**Полезные команды**

- `npm run lint` — запуск линтинга CSS (`stylelint`)
- `npm run format` / `npm run check` — запуск `prettier`
- `npm run fix` / `npm run fixall` — автопочинка через `prettier` + `stylelint`

---
