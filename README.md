# giocamole
Go ioc container

Modified version of github.com/golobby/container/v3

### Installation
To install this package, run the following command in your project directory.

```bash
go get github.com/ClementLaval/giocamole
```

Additional method: 

```go
// DeepFill recursively injects dependencies into the target struct.
// You can also provide additional direct dependencies as a second argument (a struct pointer).
// The container will prioritize injecting the provided direct dependencies over those in the container.
// This is useful for passing temporary dependencies, such as (w, *r, session).
func DeepFill(structure interface{}, dependencies interface{}) error {}
```