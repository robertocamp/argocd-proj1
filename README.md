# argocd-proj1
demo project for working with argocd 


## setup

starting from which ever Go repository you are working from (AWS or Github):

(eg) /Users/robertc/go/src/github/argocd-proj1



1. git clone git clone git@github.com:robertocamp/argocd-proj1.git
2. cdargocd-proj1

$ go mod init myapp
$ go get github.com/labstack/echo/v4



I have the following simple Go server using the Echo framework:

```
package main

import (
	"net/http"
	"github.com/labstack/echo/v4"
)

func main() {
	e := echo.New()
	e.GET("/", func(c echo.Context) error {
		return c.String(http.StatusOK, "Hello, World!")
	})
	e.Logger.Fatal(e.Start(":3000"))
}
```

Can you show me how I would add the slog logger to this server?