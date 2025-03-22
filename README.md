# WordPress Docker Compose Setup

This repository contains a `docker-compose.yml` file for setting up a WordPress development environment.

## Setup

1.  **Clone the repository:** `git clone <repository_url>`
2.  **Create a `.env` file:**

    ```
    MYSQL_ROOT_PASSWORD=your_root_password
    MYSQL_DATABASE=wordpress
    MYSQL_USER=wordpress_user
    MYSQL_PASSWORD=wordpress_password
    ```

3.  **Run Docker Compose:** `docker-compose up -d`

4.  **Access:**
    *   WordPress: `http://localhost:8080`
    *   phpMyAdmin: `http://localhost:8081`
