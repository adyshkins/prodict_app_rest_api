# product_app

Приложение выводит список товаров (ноутбуки). 

Товары выводятся в две колонки. 

Плитка товара представляет собой объект Cart в котором имеется изображение товара, его цена, наименование и описание 

<img width="308" alt="image" src="https://github.com/user-attachments/assets/e174a880-7f57-4dfd-ab02-8b22bc78d45c">


## **Рассмотрим процесс напиcания приложения**

### **1. Настройка окружения**
**Создание проекта:**
```
flutter create product_app
cd product_app
```


**Добавление библиотеки Dio: Открой файл pubspec.yaml и добавь зависимость Dio:**
```
dependencies:
  dio: ^5.0.0
```

**После этого выполните команду для установки зависимостей:**

```
flutter pub get
```

### **2. Модель данных**

Создадим модель для продукта, которую мы будем получать с REST API. Данные о продуктах нужно десериализовать из JSON-формата.

Шаги:
В директории lib создай файл **product_model.dart**
 (Готовый файл и все последующие файлы вы можете найти в данной ветке)

### **3. Получение данных с API**
Теперь создадим функцию для получения списка товаров с помощью Dio.

Шаги:
Создадим файл **api_service.dart**

### **4. Экран вывода товаров**
Теперь создадим основной экран, который будет выводить список продуктов.

Шаги:
Создадим файл **product_list_screen.dart**

### **5. Экран личного кабинета**
Создадим отдельный экран для отображения личной информации пользователя.

Шаги:
Создадим файл **profile_screen.dart**

### **6. Навигация между экранами**
Теперь соединим экран товаров и личного кабинета в главное приложение.

Шаги:
Обновим файл main.dart

Приложение будет отображать список товаров и экран профиля с тестовыми данными.

Детали:
Экран вывода товаров использует FutureBuilder для асинхронного получения данных через Dio.
Экран профиля статически отображает данные пользователя (их можно будет заменить динамическими данными в будущем).






