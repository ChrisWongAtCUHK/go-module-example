## [Create a Go module](https://go.dev/doc/tutorial/create-module)
```greetings
go mod init example.com/greetings
```

## [Call your code from another module](https://go.dev/doc/tutorial/call-module-code)
```hello
go mod init example.com/hello
go mod edit -replace example.com/greetings=../greetings
go mod tidy
go run .
```