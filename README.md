# go_cheet_sheet
Install Golang from here : <a>https://golang.org/doc/install</a></br>
Print Hello World : (make hello.go file)
```golang
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
```
For Runing Program do <b>go run hello.go</b> in your command line </br>
# Variables
```golang
package main

import "fmt"

func main() {
    name := "Quera"
    number := 123
    fmt.Println(name)
    fmt.Println(number)
    number = 1234
    fmt.Println(number)
}
```
Output:
```golang
Quera
123
1234
```
# Get Input
For Get Input From User , Use Scan Function From fmt Package</br>
Below Program Get Two Number and Calculate sum of them 
```golang
package main

import "fmt"

func main() {
    var a, b int
    fmt.Scan(&a, &b)
    fmt.Println(a + b)
}
```
