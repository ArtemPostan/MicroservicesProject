Инструкция по запуску

    Сборка проекта:
    В каждой папке микросервиса необходимо собрать проект, чтобы появилась папка target с JAR-файлом:   

    mvn clean package -DskipTests

    Настройка почты:
    Перед запуском необходимо открыть файл docker-compose.yml указать свои реальные данные для отправки писем:

        SPRING_MAIL_USERNAME: ваш email (Gmail)

        SPRING_MAIL_PASSWORD: ваш 16-значный пароль приложения Google

    Запуск в Docker:
    В корне проекта выполните:  

    docker-compose up -d --build
