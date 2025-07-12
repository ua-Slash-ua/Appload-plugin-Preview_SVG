# 🧩 PreviewSvg — Custom Field for Payload CMS

Цей репозиторій містить кастомне поле для [Payload CMS](https://payloadcms.com/), яке дозволяє редагувати HTML/SVG у
текстовому полі з миттєвим попереднім переглядом прямо в адмінці.

---

## 📁 Структура

sl_PreviewSvg

- ├── PreviewField.tsx
- └── index.ts
- └── PreviewField.module.css

---

## 🚀 Функціонал

- Поле для введення HTML або SVG
- Живий превʼю-вивід через `dangerouslySetInnerHTML`
- Використання `@payloadcms/ui` для інтеграції в адмінку
- Стилизоване за допомогою CSS-модулів

---

## 🛠 Використання

### 1. Імпорт компонента

```ts
import { PreviewSvg } from '@/{path_to___sl_PreviewSvg}}'
```

### 2. Використання компонента

```
{
  name: 'customField',
    label: { en: 'Моє кастомне поле' },
    type: 'text',
    required: false,
    admin: {
    components: {
      Field: PreviewSvg,
    },
  },
},
```
