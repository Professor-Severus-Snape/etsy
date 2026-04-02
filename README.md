[![Vite CI/CD](https://github.com/professor-severus-snape/etsy/actions/workflows/vite_ci-cd.yml/badge.svg)](https://github.com/professor-severus-snape/etsy/actions/workflows/vite_ci-cd.yml)

# Список предложений Etsy

React-приложение для отображения активных предложений с Etsy.com в виде карточек с названием, изображением, ценой и количеством.

![Список предложений](./docs/preview.png)

## Демо

Посмотреть демо можно [здесь](https://professor-severus-snape.github.io/etsy/).

## Возможности

- отображение карточек товаров
- обрезка длинных названий (50 символов)
- форматирование цен по валюте
- подсветка остатка товара (low / medium / high)
- переиспользуемые компоненты

## Архитектура компонентов

- **App** — загружает и фильтрует данные, передаёт массив `catalog` в `Listing`  
- **Listing** — рендерит список карточек товаров через `ProductItem`  
- **ProductItem** — презентационный компонент, отображает одну карточку с данными 

## Пример использования

```jsx
<Listing catalog={catalog} />
```

## Технологии

- React 18
  - JSX
  - functional components
  - props
- типизация - TypeScript
- линтинг - ESLint 
- сборка - Vite

## CI/CD

- GitHub Actions - линтинг и сборка проекта (CI)
- GitHub Pages - автоматический деплой приложения (CD)
