## Sites:
https://grpc.io/ <br>
https://grpc.io/docs/languages/go/quickstart/ <br>
https://developers.google.com/protocol-buffers <br>
https://developers.google.com/protocol-buffers/docs/gotutorial <br>
https://github.com/ktr0731/evans <br>


## Repositórios:
https://github.com/robsoninocencio/grpc <br>
https://github.com/codeedu/fc2-grpc <br>

## Rodar estes comandos após criar ou alterar um arquivo.proto

```
protoc --proto_path=proto proto/*.proto --go_out=pb
protoc --proto_path=proto proto/*.proto --go_out=pb --go-grpc_out=pb
```

## Rodar o servidor GRPC
```
go run cmd/server/server.go
```

## Como instalar client grpc do evans:
### Site para baixar o client do evans: 
https://github.com/ktr0731/evans/releases/tag/0.9.3
```
tar xvzf evans_linux_amd64.tar.gz
mv evans /usr/local/bin/evans
export PATH=$PATH:/usr/local/bin/evans
source ~/.zshrc
```

## Rodar o client GRPC do evans
```
evans -r repl --host localhost --port 50051
service UserService
call AddUser
```

## Rodar nosso client GRPC
```
go run cmd/client/client.go
```
