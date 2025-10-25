# Django ToDo App with Docker

これは Django × Docker × MariaDB を使ったログイン機能付き ToDo アプリです。

## 📦 使用技術

- Django 5.x
- MariaDB
- Docker / Docker Compose
- Python 3.11
- Bootstrap（任意）

## 🚀 起動方法

```bash
docker-compose up --build
```

## 🛠 初期設定
```bash
docker-compose exec web python manage.py migrate
docker-compose exec web python manage.py createsuperuser
```

## 🔐 ログイン
/accounts/login/ でログイン

/todo/ でタスクリスト表示

## 📁 ディレクトリ構成（例）
```
django-todo-docker/
├── backend/
│   ├── config/         # Django プロジェクト
│   ├── todo/           # ToDo アプリ
│   ├── templates/      # HTML テンプレート
│   ├── Dockerfile
│   └── requirements.txt
├── .env
├── .gitignore
├── docker-compose.yml
└── README.md
```

## 📝 ライセンス
MIT