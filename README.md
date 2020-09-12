# Usage
Running `docker-compose up -d --build site`.

Stopped `docker-compose down`

Servers:

- **nginx** - `:8080`
- **mysql** - `:3306`
- **php** - `:9000`

Do not exits installed apps run this.

- `docker-compose run --rm composer update`
- `docker-compose run --rm npm run dev`
- `docker-compose run --rm artisan migrate` 

## Persistent MySQL Storage

```
volumes:
  - ./mysql:/var/lib/mysql
```