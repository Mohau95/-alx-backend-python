# Python Decorators - 0x01

This project covers the implementation of **Python decorators** for database operations.  
Each task demonstrates a different use case of decorators in handling database queries.

---

## Files

### 0-log_queries.py
- **Objective:** Create a decorator `log_queries` that logs SQL queries before executing them.
- **Usage:** Logs queries passed to functions, e.g. `fetch_all_users`.

### 1-with_db_connection.py
- **Objective:** Implement a decorator `with_db_connection` that automatically handles opening and closing of database connections.
- **Usage:** Functions only focus on queries, connection management is automatic.

### 2-transactional.py
- **Objective:** Implement a `transactional` decorator to manage transactions (commit/rollback).
- **Usage:** Ensures database operations are atomic.

### 3-retry_on_failure.py
- **Objective:** Implement a `retry_on_failure` decorator to retry failed queries due to transient errors.
- **Usage:** Retries function calls with delay.

### 4-cache_query.py
- **Objective:** Implement a `cache_query` decorator to cache query results and avoid redundant DB calls.
- **Usage:** Uses in-memory caching dictionary `query_cache`.

---

## Requirements
- Python 3.x
- `sqlite3` (standard library)
- Database file: `users.db`

---

## How to Run
Each file is executable directly:
```bash
./0-log_queries.py
./1-with_db_connection.py
./2-transactional.py
./3-retry_on_failure.py
./4-cache_query.py
```

Make sure a valid **users.db** exists with a `users` table before testing.

---
