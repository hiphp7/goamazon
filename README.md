# Amazon non official API lib By Golang


## Usage

```go
go get -u -v github.com/hunterhug/goamazon
```


## Example

```go
package main

import (
	"fmt"
	"github.com/hunterhug/goamazon"
)

func main() {
	// New Amazon API Client
	client := goamazon.New()

	asin := "B07PBJB3R4"
	if client.ExistASIN(asin) {
		fmt.Println("exist asin:", asin)
	} else {
		fmt.Println("not exist asin:", asin)
	}
}

```