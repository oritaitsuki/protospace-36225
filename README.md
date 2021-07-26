#テーブル設計


##users テーブル

| Column      | Type    | Options    |
| ----------  | ------  | ---------  |
|email        |string   |null:false  |
|password     |string   |null:false  |
|name         |string   |null:false  |
|profile      |text     |null:false  |
|occupation   |text     |null:false  |
|position     |text     |null:false  |

##prototypes テーブル

| Colum       | Type     | Options                     |
| ----------- | -------  | --------------------------- |
|title        |string    |null: false                  |
|catch_copy   |text      |null: false                  |
|concept      |text      |null: false                  |
|image        |          |null: false                  |
|user         |references|null: false,foreign_key: true|

##comments　テーブル

| Colum       | Type     | Options                     |
| ----------- | -------- | --------------------------- |
|text         |text      |null:false                   |
|user         |references|null: false,foreign_key: true|
|prototype    |references|null: false,foreign_key: true|