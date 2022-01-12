# SickHub

...more to come soon...

## Sub 1

### Sub 2
Run on playground: https://go.dev/play/p/D9CY_mCnOon
```go
package main

import (
	"fmt"
	"time"
)

func doWhatIMean(in string) (string, error) {
	switch time.Now().Weekday() {
	case time.Saturday, time.Sunday:
		return "Learning Time?", nil
	default:
		return "Hacking Time?", nil
	}
}

func main() {
	result, err := doWhatIMean("foo")
	if err != nil {
		panic("WTF")
	}
	fmt.Println("Do you mean: " + result)
}

```
