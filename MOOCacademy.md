# MOOCacademy SQL DB

## Tables

Courses :

| id  | title | description |
| --- | ----- | ----------- |
| KEY | TEXT  | TEXT        |

Lessons :

| id  | title | body | course_id                |
| --- | ----- | ---- | ------------------------ |
| KEY | TEXT  | TEXT | FOREIGN_KEY (courses.id) |
