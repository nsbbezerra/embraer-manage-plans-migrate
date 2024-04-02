# Migrate Manage Plans

- First Install GO
- Change in 73 line database connection:
  ```
  db, err := sqlx.Connect("postgres", "user=svq dbname=services_quotation sslmode=disable password=svq host=localhost")
  ```
- Install Dependences
  ```
  go mod tidy
  ```
- Run importer
  ```
  go run plans.go
  ```
