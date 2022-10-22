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
# If Condition
Below code Detect Number is Odd or Even : </br>
```golang
package main

import "fmt"

func main() {
    var n int
    fmt.Scan(&n)
    if n % 2 == 0 {
        fmt.Println("Even")
    } else {
        fmt.Println("Odd")
    }
}
```
# Palindrom Number
Below code Detect Number is Palindrom Or Not :</br>
```golang
// Golang program to check whether a number is palindrome or not

package main
import "fmt"

func main() {
	var number,remainder,temp int
	var reverse int = 0

	fmt.Print("Enter any positive integer : ")
	fmt.Scan(&number)

	temp=number

	// For Loop used in format of While Loop
	for{
		remainder = number%10
		reverse = reverse*10 + remainder
		number /= 10

		if(number==0){
			break // Break Statement used to exit from loop
		}
	}

	if(temp==reverse){
		fmt.Printf("%d is a Palindrome",temp)
	}else{
		fmt.Printf("%d is not a Palindrome",temp)
	}

}
```
# For Loop (Only Loop in Go)
All Part of For Loop are Optional </br>
Below Code sum all number form one to n </br>
```golang
package main

import "fmt"

func main() {
    var n int
    fmt.Scan(&n)
    sum := 0
    for i := 1; i <= n; i++ {
        sum += i
    }
    fmt.Println(sum)
}
```
Below Code is equal While Loop in Other Language :</br>
while n!=0 the result is sum of all numbers
```golang
package main

import "fmt"

func main() {
    var n int
    fmt.Scan(&n)
    sum := 0
    for n != 0 {
        sum += n
        fmt.Scan(&n)
    }
    fmt.Println(sum)
}
```
# array In GO
```golang
package main

import "fmt"

func main() {
    var a [2]string
    a[0] = "Hello"
    a[1] = "World"
    fmt.Println(a[0], a[1])
    fmt.Println(a)

    primes := [6]int{2, 3, 5, 7, 11, 13}
    fmt.Println(primes)
    for i, prime := range primes {
        fmt.Println(i, prime)
    }
}
```
OutPut Will Be :</br>
Hello World </br>
[Hello World] </br>
[2 3 5 7 11 13] </br>
0 2 </br>
1 3 </br>
2 5 </br>
3 7 </br>
4 11 </br>
5 13 </br>
# Function in Go 
calculate average of two  decimal number 3 and 6 <br>
```golang
package main

import "fmt"

func avg(x float64, y float64) float64 {
    return (x + y) / 2
}

func main() {
    fmt.Println(avg(3, 6))
}
```
