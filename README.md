#Практическая работа №6.2. Создание автоматизированного UNIT-теста

##Таблица пользователей

SQL-скрипт базы данных:

CREATE TABLE Users (
    Id INTEGER PRIMARY KEY AUTOINCREMENT,
    FirstName TEXT NOT NULL,
    LastName TEXT NOT NULL,
    Username TEXT NOT NULL UNIQUE,
    Email TEXT NOT NULL UNIQUE,
    Phone TEXT,
    PasswordHash TEXT NOT NULL,
    RegisteredAt DATETIME DEFAULT CURRENT_TIMESTAMP
);

Скриншот создания таблицы:

![image](https://github.com/user-attachments/assets/c05fb683-7d50-47a9-b24e-1f840fdd10c3)

Скриншот окна «Обозреватель тестов», демонстрирующий успешное выполнение всех тестов:

![image](https://github.com/user-attachments/assets/f7556b6e-e488-4177-aa0b-d5b616596a67)

Капча которая появляеться после 3-х не правильных попыток входа:

![image](https://github.com/user-attachments/assets/fb92988a-701c-4c5c-b442-bf8d08c18789)


Вывод о проведенном тестировании
Автоматизированные тесты, связанные с регистрацией и авторизацией пользователей в WPF-приложении, выполнены успешно.

Причинами успешного выполнения тестов являются:

Корректная реализация логики регистрации и авторизации пользователей в интерфейсе приложения.
Правильная работа с базой данных Microsoft SQL Server (корректное добавление, хранение и выборка пользовательских данных).
Ошибок и сбоев в работе приложения в ходе проведения тестирования не выявлено.
