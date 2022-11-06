# killdren

Do best to kill your children.

[![Go Reference](https://pkg.go.dev/badge/gopkg.ilharper.com/x/killdren.svg)](https://pkg.go.dev/gopkg.ilharper.com/x/killdren)
[![Go Report Card](https://goreportcard.com/badge/github.com/ifrstr/killdren)](https://goreportcard.com/report/github.com/ifrstr/killdren)

This package tries to kill child process and "grandchild process" when main process shutdown or panic.

## Install

```sh
go get gopkg.ilharper.com/x/killdren
```

## Usage

```go
// Starting
cmd := &exec.Cmd{
	// ...
}
killdren.Set(cmd)
err := cmd.Run()

// Stopping
err := killdren.Stop(cmd)
```

[![Go Reference](https://pkg.go.dev/badge/gopkg.ilharper.com/x/killdren.svg)](https://pkg.go.dev/gopkg.ilharper.com/x/killdren)

## LICENSE

[MIT](https://github.com/ifrstr/killdren/blob/master/LICENSE)
