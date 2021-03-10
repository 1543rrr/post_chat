# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
## usersテーブル
|colum      |type        |options                           |
|-----------|------------|----------------------------------|
|email      |string      |null: false                       |
|password   |string      |null: false                       |
|name       |string      |null: false                       |

### Association

- has_many :commnts
- has_many :likes
- has_many :posts

## comments テーブル

|colum      |type         |options                           |
|-----------|-------------|----------------------------------|
|user_id    |integer      |null: false                       |
|post_id    |integer      |null: false                       |
|comment    |text         |null: false                       |

### Association

## likesテーブル

|colum      |type         |options                            |
|-----------|-------------|-----------------------------------|
|user_id    |integer      |null: false                        |
|post_id    |integer      |null: false                        |

### Associations

## postsテーブル

|colum　　　|type         |options                            |
|----------|-------------|-----------------------------------|
|user_id   |integer      |null: false                        |
|post_id   |integer      |null: false                        |

## Associations

- has_many :likes
- has_many :comments



