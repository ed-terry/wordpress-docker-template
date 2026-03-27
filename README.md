# 🐳 Docker WordPress Template

A minimal, ready-to-use Docker Compose setup for spinning up a WordPress site with a MySQL database — zero configuration headaches.

## 📦 Stack

- **WordPress** (latest)
- **MySQL 8.0**

## 🚀 Getting Started

### Prerequisites

- [Docker](https://docs.docker.com/get-docker/) installed
- [Docker Compose](https://docs.docker.com/compose/install/) installed

### Usage

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd <your-repo-folder>
   ```

2. **Start the containers**
   ```bash
   docker compose up -d
   ```

3. **Open WordPress**
   Visit [http://localhost:8080](http://localhost:8080) in your browser and complete the setup wizard.

4. **Stop the containers**
   ```bash
   docker compose down
   ```

## 📁 Project Structure

```
.
├── docker-compose.yml
├── db_data/          # MySQL data (auto-created)
└── wp_data/          # WordPress files (auto-created)
```

## ⚙️ Configuration

You can update the following environment variables in `docker-compose.yml` to suit your setup:

| Variable                  | Default        | Description              |
|---------------------------|----------------|--------------------------|
| `MYSQL_ROOT_PASSWORD`     | `rootpassword` | MySQL root password      |
| `MYSQL_DATABASE`          | `wordpress`    | Database name            |
| `MYSQL_USER`              | `wordpress`    | Database user            |
| `MYSQL_PASSWORD`          | `wordpress`    | Database user password   |
| `WORDPRESS_DB_HOST`       | `db:3306`      | Database host            |

> ⚠️ **Important:** Change all default passwords before deploying to any public-facing environment.

## 🗑️ Removing Everything

To stop containers and remove all volumes (this will delete your data):

```bash
docker compose down -v
```

---

## 👨‍💻 Author

Made with ❤️ by **Edward Terry**

- 🌐 Portfolio: [edwardterry.co.tz](https://edwardterry.co.tz)
- 📸 Instagram: [@m.r_terry](https://instagram.com/m.r_terry)
- ☕ Buy me a coffee: [buymeacoffee.com/edwardterry](https://buymeacoffee.com/edwardterry)

If you found this useful, consider buying me a coffee — it keeps the projects going! ☕
