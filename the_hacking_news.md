# The Hacking News

## Tables

Users :

| id  | name |
| --- | ---- |
| KEY | TEXT |

Posts :

| id  | content | url  | user_id                |
| --- | ------- | ---- | ---------------------- |
| KEY | TEXT    | TEXT | FOREIGN_KEY (users.id) |

Comments :

| id  | content | user_id                | post_id                |
| --- | ------- | ---------------------- | ---------------------- |
| KEY | TEXT    | FOREIGN_KEY (users.id) | FOREIGN_KEY (posts.id) |

Subcomments :

| id  | content | comment_id                |
| --- | ------- | ------------------------- |
| KEY | TEXT    | FOREIGN_KEY (comments.id) |
