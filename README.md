# Lamp Example 
This is a repo for deployment of LAMP stack using docker-compose.

## Prerequisites
- Docker
- Docker Compose

## How to run
1. Clone the repo
2. Run `docker-compose up -d` in the root directory of the repo

## How to access
- Apache: http://localhost:8080
- PHPMyAdmin: http://localhost:8080

## Edit PHP files
- Edit the PHP files in the `www` directory

## Interact with MySQL
Give the command to run mysql inside container:
```bash
docker exec -it mysql -u root -p
```

# Try you at home:

If you want to try this at home you can access this URL:

[W3Schools Sandbox](https://www.w3schools.com/sql/trysql.asp?filename=trysql_select_like_not)