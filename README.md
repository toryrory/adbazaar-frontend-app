This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.js`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.


## File Strcuture

- app это главная страница, "/". Внутри нее создаем папки, названия страницы берутся из названия папки. Внутри каждой папки(страницы) должен быть файл page.jsx, в этом файле добавляем содержимое страницы. Страницу можем формировать из компонентов. 
Для динамических страниц по типу /books/book-1 создаем данимаческий маршрут. Создаем: book(папка) и внутри нее файл page.jsx -> внутри папки book создаем папку с названием например [id], динамический маршрут который идет по айди или категори и т.п. обьязательно пишется в квадратных скобках. Далее в папке [id] создаем файл page.jsx и заполняем его данными одного товара.
https://nextjs.org/_next/image?url=%2Fdocs%2Flight%2Fdefining-routes.png&w=1920&q=75&dpl=dpl_6KUi7SsiRYPCp7E367Sqa7pwstjU

- components для файлов компонентов и файлов для их стилей
- data для хранения данных в JSON формате
- utils для мелких функций по типу отформатировать отображение даты и т.п.
- public для хранения картинок 

- layout.jsx это макет который создается для нескольких страниц. Обьязательно должен быть корневой макет (который лежит в папке app). В нем обьязательно должен быть тег html и body. Макеты так же можно создавать и для других страниц.