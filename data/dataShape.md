```sql

CREATE TABLE `users` (
	`id`	INTEGER PRIMARY KEY AUTOINCREMENT UNIQUE,
	`name`	TEXT NOT NULL,
	`created_at`	INTEGER DEFAULT 'CURRENT_TIMESTAMP'
);

CREATE TABLE `posts` (
	`id`	INTEGER PRIMARY KEY AUTOINCREMENT UNIQUE,
	`user_id`	INTEGER,
	`text`	TEXT NOT NULL,
	`created_at`	NUMERIC DEFAULT CURRENT_TIMESTAMP
);

CREATE TABLE `tags` (
	`id`	INTEGER PRIMARY KEY AUTOINCREMENT UNIQUE,
	`tag`	TEXT UNIQUE,
	`created_at`	TEXT DEFAULT CURRENT_TIMESTAMP
);

```