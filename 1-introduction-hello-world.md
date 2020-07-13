### This file covers starter point introduction in Go.

```
package main

import "fmt"

func main() {
	fmt.Println("Hello World")
}
```

A function to print out hello world.

Run with `go run main.go`

Notes:
The package `main` tells the Go compiler that the package should compile as an executable program instead of a shared library, also the main entry point.

----------------
You can import multiple packages like this:

```
import "package1"
import "package2"
```

OR

```
import (
  "package1"
  "package2"
)
```

You can also provide an alias to a package by including the alias name before the file:

```
import (
  p1 "package1"
  "package2"
)
```

Since we have aliased package1 as p1, we can call functions from package 1 uisng the alias -p1
So instead of calling something typically like this: `package1.SampleFunc()` it can be this: `p1.SampleFunc()`

another example:

```
package main

import "fmt"
import t "time"

func main() {
   fmt.Println("Hello World")
   fmt.Println(t.Now())
}
```

#### comments(types)
```
// Are we racing or coding?
  /*
  fmt.Println("Ready")
  fmt.Println("Set")
  ```
  */
  
  #### docs
  To do quick cjeck on Go's doc/syntac/library
  
  `go doc fmt` `go doc fmt.Println`
