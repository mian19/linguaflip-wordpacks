# LinguaFlip Word Packs

Готовые наборы слов для приложения LinguaFlip.

## 📦 Содержимое

- **10 паков** по 20 слов каждый
- **6 базовых паков** (en↔es, en↔ru, en↔zh)
- **4 тематических пака** (Travel, Food)

## 🚀 Как загрузить на GitHub

### Шаг 1: Создай репозиторий

1. Зайди на https://github.com
2. Нажми **New repository**
3. Название: `linguaflip-wordpacks`
4. Описание: `Word packs for LinguaFlip language learning app`
5. Выбери **Public**
6. ✅ Поставь галочку **Add a README file**
7. Нажми **Create repository**

### Шаг 2: Загрузи файлы

#### Вариант А: Через веб-интерфейс (проще)

1. В репозитории нажми **Add file** → **Upload files**
2. Перетащи всю папку `WordPacks` в окно браузера
3. Напиши commit message: `Add initial word packs`
4. Нажми **Commit changes**

#### Вариант Б: Через терминал (для профи)

```bash
cd "/Users/mac/Desktop/MAV Apps/LinguaFlip_release/WordPacks"

# Инициализируй git
git init

# Добавь все файлы
git add .

# Сделай первый коммит
git commit -m "Add initial word packs"

# Добавь remote (замени YOUR_USERNAME на свой)
git remote add origin https://github.com/YOUR_USERNAME/linguaflip-wordpacks.git

# Загрузи на GitHub
git branch -M main
git push -u origin main
```

### Шаг 3: Получи ссылки

После загрузки твои файлы будут доступны по ссылкам:

```
https://raw.githubusercontent.com/YOUR_USERNAME/linguaflip-wordpacks/main/packs_catalog.json
https://raw.githubusercontent.com/YOUR_USERNAME/linguaflip-wordpacks/main/packs/en_es_basic_20.json
https://raw.githubusercontent.com/YOUR_USERNAME/linguaflip-wordpacks/main/packs/es_en_basico_20.json
...
```

### Шаг 4: Используй в приложении

В коде приложения замени `YOUR_USERNAME` на свой GitHub username:

```swift
let baseURL = "https://raw.githubusercontent.com/YOUR_USERNAME/linguaflip-wordpacks/main"
```

## 📊 Статистика

- **Всего слов:** 200
- **Языковых пар:** 6
- **Категорий:** 3 (General, Travel, Food)
- **Размер:** ~100 KB

## 🔄 Как обновить паки

1. Отредактируй JSON файлы локально
2. Загрузи изменения на GitHub
3. Приложение автоматически получит новые версии

## 📝 Структура файлов

```
WordPacks/
├── packs_catalog.json          # Каталог всех паков
├── packs/
│   ├── en_es_basic_20.json     # English → Spanish: Basics
│   ├── es_en_basico_20.json    # Español → Inglés: Básico
│   ├── en_ru_basic_20.json     # English → Russian: Basics
│   ├── ru_en_basic_20.json     # Русский → Английский: Базовый
│   ├── en_zh_basic_20.json     # English → Chinese: Basics
│   ├── zh_en_basic_20.json     # 中文 → 英语：基础
│   ├── en_es_travel_20.json    # English → Spanish: Travel
│   ├── en_es_food_20.json      # English → Spanish: Food
│   ├── en_ru_travel_20.json    # English → Russian: Travel
│   └── en_zh_food_20.json      # English → Chinese: Food
└── README.md                   # Эта инструкция
```

## ✅ Готово!

Теперь можно интегрировать эти паки в приложение LinguaFlip.
