# Djangoプロジェクトスタート

## 1.プロジェクト作成コマンドを実行

```
docker-compose run web django-admin.py startproject "プロジェクト名" .
```


## 2.DB設定ファイルを編集

```python:/setting.py
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'django-db',
        'USER': 'user',
        'PASSWORD': 'pass',
        'HOST': 'db',
        'PORT': '3306'
    }
}
```

## 3.コンテナ起動
```
docker-compose up -d
```