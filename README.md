## Sites:
https://grpc.io/
https://grpc.io/docs/languages/go/quickstart/
https://developers.google.com/protocol-buffers
https://developers.google.com/protocol-buffers/docs/gotutorial
https://github.com/ktr0731/evans


## Repositório:
https://github.com/codeedu/fc2-grpc
https://github.com/robsoninocencio/grpc

## Rodar estes comandos após criar ou alterar um arquivo.proto
protoc --proto_path=proto proto/*.proto --go_out=pb
protoc --proto_path=proto proto/*.proto --go_out=pb --go-grpc_out=pb

## Rodar o servidor GRPC
go run cmd/server/server.go

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
evans -r repl --host localhost --port 50051
service UserService
call AddUser

## Rodar nosso client GRPC
go run cmd/client/client.go
