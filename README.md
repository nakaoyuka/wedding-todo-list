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

## userテーブル
|Column|Type|Options|
|------|----|-------|
|nickname|string|nill: false|
|email|string|nill: false|
|password|string|nill: false|
|bigday|date|nill: false|
### Association
- has_many :tasks

## taskテーブル
|Column|Type|Options|
|------|----|-------|
|date|date||
|type|string||
|text|text||
|user_id|integer|null: false, foreign_key: true|
### Association
- belongs_to :user