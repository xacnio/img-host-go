# img-host-go

It's a image hosting script in Golang. It's have http server and images can be uploaded from here but uploaded images are sending to Telegram Cloud Storage by bot and they aren't stored in your server. In this way, there will be no storage problems on your server. When we want to reach some image from our http server, the server forwarding you to telegram http server with reverse proxy.

- Storage on Telegram Cloud Storage
- Simple data management with Redis

# Screenshots

- [1](assets/1.png) 
- [2](assets/2.png)
- [3](assets/3.png)
- [4](assets/4.png)

## Config

Create .env file and edit ([Sample](.env.sample))

## Run

```
> go run main.go
```

### Docker

```
> docker-compose --env-file ./.env.dev up -d
```