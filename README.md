# README

## users テーブル

| Column                    | Type   | Options     |
| --------------------------| -------|-------------|     
| username                  | string | null: false | 
| email                     | string | null: false |
| password                  | string | null: false |
| profile                   | text   | null: false |            
| profile_image_id          | string | null: false |               
| created_at                | string | null: false |                 
| updated_at                | string | null: false |            


### Association
 
- has_many :recipes


## recipes テーブル

| Column           | Type       | Options     |    
| ------           | ------     | ----------- |
| user_id          | references | foreign_key: true|
| title            |  text      | null: false |
| body             | string     | null: false |
| created_at       | integer    | null: false |
| updated_at       | integer    | null: false |


### Association

- belongs_to :user


