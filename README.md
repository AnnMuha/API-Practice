# 📌 Встановлення та налаштування проєкту

Для налаштування середовища та запуску проєкту виконайте наступні кроки.

1. Встановіть **PHP**:
    - Для **macOS/Linux** використовуйте **Homebrew**:
    ```bash
    brew install php@8.2
    ```
    - Для **Windows** завантажте PHP з офіційного сайту [php.net](https://windows.php.net/download).

2. Встановіть **Symfony CLI**:
    - Для **macOS/Linux** виконайте:
    ```bash
    curl -sS https://get.symfony.com/cli/installer | bash
    ```
    - Для **Windows** завантажте інсталятор з [офіційного сайту Symfony](https://symfony.com/download).

3. Встановіть **Composer**:
    - Для **macOS/Linux** виконайте:
    ```bash
    curl -sS https://getcomposer.org/installer | php
    sudo mv composer.phar /usr/local/bin/composer
    ```
    - Для **Windows** завантажте інсталятор з [офіційного сайту Composer](https://getcomposer.org/).

4. Встановіть **Postman**: Завантажте Postman з [Postman](https://www.postman.com/downloads/).

5. Встановіть **OpenSSL**:
    - Для **macOS/Linux** OpenSSL зазвичай вже встановлений. Якщо ні, виконайте:
    ```bash
    brew install openssl
    ```

6. Клонуйте репозиторій:
    ```bash
    git clone https://github.com/AnnMuha/API-Practice.git
    cd API-Practice
    ```

7. Встановіть залежності:
    ```bash
    composer install
    ```
    Додайте залежність для **JWT аутентифікації**:
    ```bash
    composer require "lexik/jwt-authentication-bundle"
    ```

8. Генеруйте пару ключів для JWT:
    ```bash
    php bin/console lexik:jwt:generate-keypair
    ```

9. Запустіть сервер Symfony:
    ```bash
    symfony serve
    ```

10. Ваше API буде доступне за наступним посиланням:
    ```
    http://127.0.0.1:8000/api/v1/users/
    ```

Тепер ваше середовище готове до роботи, і ви можете почати розробку та тестування API.



# 📄 Documentation: 
https://documenter.getpostman.com/view/41722316/2sAYX3rPBE
