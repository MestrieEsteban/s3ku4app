
# S3ku4pp


## Requirements

- Docker 🐳

## Stack
Node js + Express + Prisma `./src`
Nginx reverse proxy mode `./nginx/nginx.conf` and `./nginx/conf.d`
Redis with Lua configuration `./nginx/limit.lua` and `./nginx/nginx.conf`
### Without Gizmo CLI
1. Run `docker-compose up -d --build`
2. Go to .env file and replace this line `DATABASE_URL=postgres://root:root@postgres:5432/2d0` to `DATABASE_URL=postgres://root:root@localhost:5434/2d0`
3. Run `npx prisma migrate dev --name "init" --preview-feature`
4. You can add VHost `127.0.0.1 s3ku4pp.com`
5. Got to `https://localhost:10443/` or `https://s3ku4pp.com:10443/`

### Postman
https://we.tl/t-lM4IZ305ts

### N-tier api token
`xQW0WqkBXUzcLc6u4trmGSTXUrx2grLp`
`WpKaV4URA66YknzDK5qvKlMWJrwvwf8N`
