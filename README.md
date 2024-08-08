# Аренда городских пространств

## Описание проекта

Проект представляет собой платформу, предоставляющую почасовую возможность арендовать помещение в Москве и МО. Основные функциональности включают в себя: выбор помещения с возможностью фильтрации и картой, выбор дополнительных помещений или опций, выбор часов для бронирования, форма для бронирования и оплаты, генерация популярных подборок помещений в различных учреждениях. Пользователи могут фильтровать помещения, искать подходящее помещение на карте, а также просматривать детальную информацию по каждому пространству, переходя на соответствующую детальную страницу. Цель проекта — обеспечить удобный и эффективный инструмент для аренды пространств в городе, сокращая время и усилия, затрачиваемые на эти процессы.

## Назначение проекта

Этот проект был разработан с целью предоставления удобного и интуитивно понятного инструмента для почасовой аренды помещений в Москве.

## Галерея

![Изображение 1](https://github.com/BrandonWF1/arenda/blob/main/screen%201.png)
![Изображение 2](https://github.com/BrandonWF1/arenda/blob/main/screen%202.png)
![Изображение 3](https://github.com/BrandonWF1/arenda/blob/main/screen%203.png)
![Изображение 4](https://github.com/BrandonWF1/arenda/blob/main/screen%204.png)
![Изображение 5](https://github.com/BrandonWF1/arenda/blob/main/screen%205.png)
![Изображение 6](https://github.com/BrandonWF1/arenda/blob/main/screen%206.png)
![Изображение 7](https://github.com/BrandonWF1/arenda/blob/main/screen%207.png)


## Моя роль в проекте

В рамках данного проекта я отвечал за поддержку Front-end части и разработку нового функционала. Мои обязанности включали в себя поддержку пользовательского интерфейса, обеспечение его корректного взаимодействия с серверной частью, а также проектирование и разработка соверешнно нового функционала. Я тесно сотрудничал с разработчиками серверной части, аналитиками , дизайнерами и тестировщиками, чтобы гарантировать бесперебойную работу всего приложения, и оптимизировал Front-end для обеспечения высокой производительности и отзывчивости и инклюзивности интерфейса. Мой вклад в проект также включал создание нового функционала скидок и системы лояльности, системы возвравтов за отмену бронирования, а также добавление инклюзивности для слепых и слабовидящих, используя возможности собственной дизайн-системы.


## Технологии, используемые в проекте

  ![NextJS](https://img.shields.io/badge/-NextJS-black?style=for-the-badge&logo=next.js)
  ![Typescript](https://img.shields.io/badge/-Typescript-white?style=for-the-badge&logo=typescript)
  ![SCSS](https://img.shields.io/badge/-SCSS-pink?style=for-the-badge&logo=sass)
  ![Redux Toolkit](https://img.shields.io/badge/-Redux_Toolkit-purple?style=for-the-badge&logo=redux)
  ![Reakit](https://img.shields.io/badge/-Ant_Design-blue?style=for-the-badge&logo=antdesign)

## Принципы и инструменты разработки
- Код-стиль и форматирование: Prettier
- Система контроля версий: Git + GitLab
- Прочие инструменты: maki (Собственная devOps разработка), Cypress, Sonar
- Линтер: ESLint
  <details>
  <summary>Конфиг linter`а</summary>
  
  ```javascript
  {
  "parser": "@typescript-eslint/parser",
  "parserOptions": {
    "ecmaVersion": 2018,
    "ecmaFeatures": {
      "jsx": true
    },
    "useJSXTextNode": true
  },
  "env": {
    "browser": true,
    "node": true,
    "commonjs": true,
    "jest": true
  },
  "extends": [
    "plugin:@typescript-eslint/recommended",
    "react-app",
    "airbnb",
    "prettier"
  ],
  "plugins": ["@typescript-eslint", "react-hooks", "jsx-a11y"],
  "rules": {
    "no-use-before-define": 0,
    "react/require-default-props": 0,
    "@typescript-eslint/ban-ts-ignore": 0,
    "no-shadow": 0,
    "arrow-body-style": "warn",
    "@typescript-eslint/ban-types":0,
    "@typescript-eslint/ban-ts-comment":0,
    "@typescript-eslint/no-unused-vars": 1,
    "@typescript-eslint/no-empty-function": 1,
    "@typescript-eslint/no-use-before-define": 2,
    "@typescript-eslint/no-explicit-any": [2, {"ignoreRestArgs": false}],
    "@typescript-eslint/interface-name-prefix": 0,
    "@typescript-eslint/explicit-member-accessibility": 0,
    "import/no-extraneous-dependencies": [2, { "devDependencies": true }],
    "spaced-comment": ["error", "always", { "markers": ["/"] }],
    "react/jsx-filename-extension": [
      1,
      { "extensions": [".js", ".jsx", ".tsx"] }
    ],
    "react-hooks/rules-of-hooks": "error",
    "react-hooks/exhaustive-deps": "warn",
    "@typescript-eslint/explicit-function-return-type": 0,
    "@typescript-eslint/prefer-function-type": 2,
    "no-param-reassign": ["error", { "props": true, "ignorePropertyModificationsFor": ["state"] }],
    "jsx-a11y/label-has-associated-control": [
      2,
      {
        "labelComponents": ["CustomInputLabel"],
        "labelAttributes": ["label"],
        "controlComponents": ["CustomInput"],
        "depth": 3
      }
    ],
    "jsx-a11y/label-has-for": 0,
    "react/jsx-props-no-spreading": 0,
    "import/extensions": ["error", "ignorePackages", {
        "js": "never",
        "jsx": "never",
        "ts": "never",
        "tsx": "never"
      }
    ],
    "react/destructuring-assignment": 1
  },
  "overrides": [
    {
      "files": ["*.js"],
      "rules": {
        "@typescript-eslint/no-var-requires": "off"
      }
    },
    {
      "files": ["style.ts"],
      "rules": {
        "import/no-unresolved": 0
      }
    },
    {
      "files": ["*.ts", "*.tsx"],
      "rules": {
        "no-undef": 0
      }
    }
  ],
  "settings": {
    "import/resolver": {
      "node": {
        "extensions": [".js", ".jsx", ".ts", ".tsx"]
      }
    }
  }
}

</details>

## Команда
- Общее количество человек: 12
- Роли в команде:
  - Разработчиков: 4
  - Дизайнеров: 1
  - Тестировщиков: 2
  - Lead: 1
  - Аналитиков: 2
  - Product & Project Managment: 2
    
# Основные достижения и результаты

- Успешная реализация функционала скидок для каждого учреждения и системы лояльностей пользователей.
- Реализация инклюзивного пользовательского интерфейса, который позволяет эффективно работать со скринридерами VoiceOver и NVDA.
- Ежедневная поддержка проекта и доработка существующего функционала.
- Оптимизация производительности Front-end части, гарантирующая быструю и отзывчивую работу приложения.
- Доработка детальных страниц помещений и форм для бронирования.
- Реализация пользовательской части функционала возвратов.


## Особые вызовы и преодоленные препятствия

- **Интеграция с Back-end при разработке нового функционала**: Столкнулись с трудностями синхронизации Front-end и Back-end при внедрении нового функционала, решили через тесное взаимодействие и использование мок-данных для отладки.
- **Инклюзивность**: Настройка корректной работы скринридеров для полностью инклюзивного проекта.
- **Синхронизация при разработке крупного функционала**: Грамотная и отлаженная работа команды при реализации крупных нововведений в сжатые сроки.


## Ссылки

- **Проект**: mos.ru/arenda.
- **Код проекта**: Код находится под защитой соглашения о неразглашении (NDA), из-за чего, к сожалению, не может быть предоставлен для общего доступа или просмотра.
