# LearngGRPC

## Quick start examples/helloworld

### Run the code

1. Compile and execute the server code

```bash
cd examples/helloworld
go run greeter_server/main.go
```

2. From a different terminal, compile and execute the client code to see the client output:
 ```bash
 go run .\greeter_client\main.go
 Greeting: Hello world
```

### Regenerate gRPC code

```bash
protoc --go_out=. --go_opt=paths=source_relative     --go-grpc_out=. --go-grpc_opt=paths=source_relative     helloworld/helloworld.proto
```