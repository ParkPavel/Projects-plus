# Contributing to Projects Plus

Спасибо за интерес к развитию Projects Plus! Этот документ поможет вам начать участие в проекте.

## 🤝 Как внести вклад

### Сообщения об ошибках

Перед созданием нового issue:
1. Проверьте [существующие issues](https://github.com/ParkPavel/Projects-plus/issues)
2. Убедитесь, что используете последнюю версию плагина
3. Воспроизведите ошибку с минимальными шагами

При создании issue включите:
- Версию Obsidian
- Версию Projects Plus
- Операционную систему
- Подробные шаги воспроизведения
- Скриншоты (если применимо)
- Логи консоли разработчика

### Предложения функций

1. Проверьте [Discussions](https://github.com/ParkPavel/Projects-plus/discussions)
2. Опишите проблему, которую решает предложение
3. Предложите детальное решение
4. Рассмотрите альтернативы

### Pull Requests

1. **Fork** репозитория
2. Создайте feature branch: `git checkout -b feature/amazing-feature`
3. Внесите изменения
4. Добавьте тесты (если применимо)
5. Убедитесь, что код соответствует стилю проекта
6. Commit: `git commit -m 'feat: add amazing feature'`
7. Push: `git push origin feature/amazing-feature`
8. Создайте Pull Request

## 🏗️ Настройка среды разработки

### Требования
- Node.js (v16+)
- npm или yarn
- Git

### Установка
```bash
# Клонируйте репозиторий
git clone https://github.com/ParkPavel/Projects-plus.git
cd Projects-plus

# Установите зависимости
npm install

# Соберите плагин
npm run build

# Для разработки с hot reload
npm run dev
```

### Структура проекта
```
Projects-plus/
├── src/                    # Исходный код
│   ├── components/        # React компоненты
│   ├── stores/           # Управление состоянием
│   ├── utils/            # Утилиты
│   └── main.ts           # Главный файл плагина
├── styles/               # CSS стили
├── docs/                 # Документация
├── tests/               # Тесты
└── manifest.json        # Манифест плагина
```

## 📝 Стандарты кода

### TypeScript
- Используйте строгую типизацию
- Избегайте `any`, предпочитайте `unknown`
- Документируйте публичные API с JSDoc

### Стиль кода
- Используйте Prettier для форматирования
- ESLint для проверки кода
- Именование: camelCase для переменных, PascalCase для классов

### Commits
Используйте [Conventional Commits](https://www.conventionalcommits.org/):
- `feat:` новая функция
- `fix:` исправление бага
- `docs:` изменения документации
- `style:` форматирование кода
- `refactor:` рефакторинг
- `test:` добавление тестов
- `chore:` обновление зависимостей

## 🧪 Тестирование

```bash
# Запуск тестов
npm test

# Запуск тестов с покрытием
npm run test:coverage

# Запуск линтера
npm run lint

# Исправление линтера
npm run lint:fix
```

## 📖 Документация

- Обновляйте README.md при добавлении функций
- Добавляйте JSDoc комментарии к публичным методам
- Создавайте примеры использования
- Обновляйте CHANGELOG.md

## 🎨 UI/UX Guidelines

### Принципы дизайна
- **Минимализм**: убирайте лишнее
- **Консистентность**: используйте единый стиль
- **Доступность**: поддерживайте accessibility
- **Производительность**: оптимизируйте рендеринг

### Цвета и темы
- Используйте CSS custom properties
- Поддерживайте светлую и темную темы
- Следуйте дизайн-системе Obsidian

## 🌍 Интернационализация

При добавлении текста:
1. Используйте i18n ключи вместо хардкода
2. Добавляйте переводы в `src/i18n/`
3. Тестируйте с разными языками

## 📦 Релизы

### Подготовка релиза
1. Обновите `manifest.json` и `versions.json`
2. Обновите CHANGELOG.md
3. Создайте git tag: `git tag v1.0.0`
4. Push tag: `git push origin v1.0.0`
5. GitHub Action автоматически создаст релиз

### Версионирование
Используем [Semantic Versioning](https://semver.org/):
- MAJOR.MINOR.PATCH
- MAJOR: breaking changes
- MINOR: новые функции
- PATCH: исправления багов

## 🤔 Вопросы?

- Создайте [Discussion](https://github.com/ParkPavel/Projects-plus/discussions)
- Посмотрите [документацию](docs/)
- Изучите существующий код

## 📜 Лицензия и атрибуция

Участвуя в проекте, вы соглашаетесь:
- Лицензировать ваш вклад под Apache License 2.0
- Следовать принципам открытого исходного кода
- Уважать оригинальную работу Marcus Olsson

---

**Спасибо за вклад в Projects Plus! 🚀**