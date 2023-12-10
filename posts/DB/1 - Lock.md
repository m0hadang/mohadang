#  잠금 확인 

information_schema 테이블에서 확인 가능

```sql
MariaDB [(none)]> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mydb               |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
5 rows in set (0.001 sec)
```

# 배타 잠금(Exclusive Locks)

현재 상태

```sql
MariaDB [mydb]> SELECT * FROM users;
+----+---------+----------+------+---------------------+
| id | user_id | pwd      | name | created_at          |
+----+---------+----------+------+---------------------+
|  3 | user1   | test1234 | AAAA | 2023-10-02 21:57:34 |
+----+---------+----------+------+---------------------+
1 row in set (0.000 sec)
```