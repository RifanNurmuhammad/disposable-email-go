# Disposable email list using Golang

Disposable email is a Golang library for dealing with blocked disposable email list.

## Installation

```bash
$ go get github.com/RifanNurmuhammad/disposable-email-go
```

## Usage

```golang
package main

import (
	"fmt"

	disposableemail "github.com/RifanNurmuhammad/disposable-email-go"
)

func main() {
	disposable := disposableemail.IsDisabledEmail("temp@getnada.com")
	fmt.Println(disposable) // true

	disposable := disposableemail.IsDisabledEmail("temp@google.com")
	fmt.Println(disposable) // false

	disposable = disposableemail.IsDisabledDomain("getnada.com")
	fmt.Println(disposable) // true

	disposable = disposableemail.IsDisabledDomain("gmail.com")
	fmt.Println(disposable) // false
}
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

