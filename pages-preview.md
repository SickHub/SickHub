
## Sub 1

### Sub 2
Run on playground: [Try it out!](https://go.dev/play/p/E1fh2kXyZ_4)
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
