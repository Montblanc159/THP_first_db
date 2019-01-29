# The Hacking Pinterest

## Tables

Users :

| id  | name |
| --- | ---- |
| KEY | TEXT |

Pins :

| id  | URL  | user_id                |
| --- | ---- | ---------------------- |
| KEY | TEXT | FOREIGN_KEY (users.id) |

Comments :

| id  | content | user_id                | pin_id                |
| --- | ------- | ---------------------- | --------------------- |
| KEY | TEXT    | FOREIGN_KEY (users.id) | FOREIGN_KEY (pins.id) |
