# SQL Samples
```sql

-- ユーザーの追加
create user user@localhost identified by password;

-- ユーザーに権限を付与
GRANT ALL PRIVILEGES ON * . * TO user@localhost;

-- データベースの追加
create database testdb;

-- テーブルの作成
CREATE TABLE USER (
    ID INT AUTO_INCREMENT PRIMARY KEY,
    NAME VARCHAR(255) NOT NULL,
    MAILADDRESS VARCHAR(255) UNIQUE NOT NULL,
    CREATED_AT TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    UPDATED_AT TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP
);

-- テーブルの削除
DROP TABLE USER;

-- テーブルのレコードを全て削除
TRUNCATE TABLE USER;

-- レコードの登録
INSERT INTO USER (NAME, MAILADDRESS)
VALUES
    ('Jane Smith', 'jane.smith@example.com');

```
