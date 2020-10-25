# golang-handlebook

## hello world

```go
package main
import (
	"fmt"
)
func main()  {
	fmt.Println("hello world")	
}
```

## 变量

```go
package main
import (
	"fmt"
)
func main()  {
	var a int
	var b string = "字符串"
	fmt.Println("hello world")	
	fmt.Println(a)	
	fmt.Println(b)	
}
```

## 类型推断

```go
package main
import (
	"fmt"
)
func main()  {
	var a int
	var b string = "字符串"
	c := "字符串c"
	d := 14
	fmt.Println("hello world")	
	fmt.Println(a)	
	fmt.Println(b)	
	fmt.Println(c)	
	fmt.Println(d)
}
```

## 元组

```go
func main() {
	var arr [3]int
	arr1 := [3]int{1, 2, 3}
	fmt.Println(arr)
	fmt.Println(arr1)
	arr1[0] = 10
	fmt.Println(arr1)
}
```

## 切片

```go
func main() {
	arr := []int{1, 2, 3}
	fmt.Println(arr)
	arr = append(arr, 10)
	fmt.Println(arr)
}
```

## 词典

```go
func main()  {
	numbers := make(map[string]int)	
	numbers["one"] = 1	
	numbers["two"] = 2
	fmt.Println(numbers)
	delete(numbers, "one")
	fmt.Println(numbers)
}
```

## 遍历

```go
func main() {
	i := 0
	for ; i < 5; {
		fmt.Println(i)
		i ++
	}
}
```
遍历数组
```go
func main()  {
	a := []int{1, 2, 3, 4}
	for k, v := range a {
		fmt.Println(k, v)
	}
}
```
遍历词典
```go
func main()  {
	numbers := make(map[string]int)	
	numbers["one"] = 1
	numbers["two"] = 2
	numbers["three"] = 3
	for k, v := range numbers {
		fmt.Println(k, v)
	}
}
```