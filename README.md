# README

#usersテーブル
| Column      | Type      |  Options    |
| ------      | --------  | ----------- |
| emails      | string    | null: false |
| password    | string    | null: false |
| name        | string    | null: false |
| profile     | text      | null: false |
| occupation  | text      | null: false |
| position    | text      | null: false |

#prototypeテーブル
| Column      | Type      |  Options    |
| ------      | --------  | ----------- |
| title       | string    | null: false |
| catch_copy  | text    | null: false |
| concept     | text    | null: false |
| image     | ActiveStorage| 
| user  | references |

＃commentsテーブル
| Column      | Type      |  Options    |
| ------      | --------  | ----------- |
| text       | string    | null: false |
| user  | references    | null: false, foreign_key: true |
| prototype | reference | null: false, foreign_key: true |