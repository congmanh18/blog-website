---
title: Làm quen với Golang cơ bản
published: 2025-03-18
description: 'Chi tiết cách sử dụng biến, hằng, vòng lặp, điều kiện và thư viện trong Go'
image: './golang.png'
tags: [golang, guide, backend]
category: 'Golang'
draft: false 
--- 
# Gọi lệnh từ một gói (package) thư viện khác bên ngoài
:::tip
Nếu bạn muốn sử dụng một package do người khác viết, bạn có thể tìm các thư viện phù hợp trên trang: [**pkg.go.dev**](https://pkg.go.dev)
:::

Ví dụ, để sử dụng module **"quote"** và gọi function `Go()`, bạn có thể tạo một file Go, ví dụ `ex7.go`, với nội dung như sau:

```go
package main

import (
    "fmt"
    "rsc.io/quote"
)

func main() {
    fmt.Println(quote.Go())
}
```

:::note[NOTE]
:::
Như trong đoạn code trên, chúng ta sử dụng function `Go()` từ module **"quote"**. Để sử dụng được module này, bạn cần tải về thư viện bằng lệnh:
```bash
$ go mod tidy
```
Lệnh này sẽ định vị và tải module **"quote"** về máy. Sau đó, chạy chương trình bằng lệnh:
```bash
$ go run .
```
Kết quả sẽ là:
```
Don't communicate by sharing memory, share memory by communicating.
```
Bạn có thể tìm thêm nhiều package và module hữu ích khác tại:  
[**pkg.go.dev**](https://pkg.go.dev)

# Những kiểu giá trị thông dụng trong Go

Golang hỗ trợ nhiều kiểu giá trị khác nhau, bao gồm:

- **string**: Chuỗi, có thể kết hợp các chuỗi với nhau bằng dấu `+`.
- **numeric**: Kiểu số, bao gồm số nguyên (integers) và số thập phân (floats).
- **boolean**: Kiểu luận lý, với hai giá trị `true` và `false`.

Ví dụ minh họa:

```go
package main

import "fmt"

func main() {
    fmt.Println("go" + "lang")
    fmt.Println("1+1 =", 1+1)
    fmt.Println("7.0/3.0 =", 7.0/3.0)
    fmt.Println(true && false)
    fmt.Println(true || false)
    fmt.Println(!true)
}
```

Chạy chương trình bằng lệnh:

```bash
$ go run .
```

Kết quả:

```
golang
1+1 = 2
7.0/3.0 = 2.3333333333333335
false
true
false
```
# Sử dụng biến (Variables) trong Go

Biến là các phần tử lưu trữ dữ liệu. Trong Go, có nhiều loại biến như:

- **int**: Lưu trữ số nguyên, ví dụ: `-111` hoặc `111`.
- **float32**: Lưu trữ số thập phân, ví dụ: `20.1` hoặc `-20.1`.
- **string**: Lưu trữ chuỗi, ví dụ: `"Hello world"`.
- **bool**: Lưu trữ giá trị luận lý, `true` hoặc `false`.

### **Cách khai báo biến**

1. **Cách khai báo đầy đủ**:
   ```go
   var variablename type = value
   ```

2. **Cách khai báo ngắn gọn**:
   ```go
   variablename := value
   ```
   - Cách này chỉ sử dụng được bên trong function.
   - Go sẽ tự suy luận kiểu dữ liệu dựa trên giá trị.

3. **Khai báo nhiều biến cùng lúc**:
   ```go
   var b, c int = 1, 2
   ```

### **Ví dụ minh họa**

```go
package main

import "fmt"

func main() {
    var a = "initial"
    fmt.Println(a)

    var b, c int = 1, 2
    fmt.Println(b, c)

    var d = true
    fmt.Println(d)

    var e int
    fmt.Println(e)

    f := "apple"
    fmt.Println(f)
}
```

Chạy chương trình:

```bash
$ go run variables.go
```

Kết quả:

```
initial
1 2
true
0
apple
```

# Giới thiệu về hằng (Constants) trong Go

Hằng số là các giá trị cố định không thể thay đổi. Để khai báo hằng, sử dụng từ khóa `const`:

```go
const CONSTNAME type = value
```

Hằng số có thể là kiểu ký tự, chuỗi, luận lý hoặc số. Ví dụ:

```go
package main

import (
    "fmt"
    "math"
)

const s string = "constant"

func main() {
    fmt.Println(s)

    const n = 500000000
    const d = 3e20 / n

    fmt.Println(d)
    fmt.Println(int64(d))
    fmt.Println(math.Sin(n))
}
```

Chạy chương trình:

```bash
$ go run constant.go
```

Kết quả:

```
constant
6e+11
600000000000
-0.28470407323754404
```

# Vòng lặp FOR trong Go

Vòng lặp `for` là cấu trúc lặp duy nhất trong Go. Dưới đây là các loại vòng lặp:

### **1. Vòng lặp 1 yếu tố**
```go
i := 1
for i <= 3 {
    fmt.Println(i)
    i = i + 1
}
```

### **2. Vòng lặp 3 yếu tố**
```go
for j := 7; j <= 9; j++ {
    fmt.Println(j)
}
```

### **3. Vòng lặp vô hạn**
```go
for {
    fmt.Println("loop")
    break
}
```

### **4. Sử dụng `continue`**
```go
for n := 0; n <= 5; n++ {
    if n%2 == 0 {
        continue
    }
    fmt.Println(n)
}
```

# Câu lệnh điều kiện If/Else trong Go

Câu lệnh `if/else` trong Go rất đơn giản. Ví dụ:

### **1. Câu lệnh `if`**
```go
if 7%2 == 0 {
    fmt.Println("7 is even")
}
```

### **2. Câu lệnh `if/else`**
```go
if 7%2 == 0 {
    fmt.Println("7 is even")
} else {
    fmt.Println("7 is odd")
}
```

### **3. Câu lệnh `if/else if`**
```go
if num := 9; num < 0 {
    fmt.Println(num, "is negative")
} else if num < 10 {
    fmt.Println(num, "has 1 digit")
} else {
    fmt.Println(num, "has multiple digits")
}
```

# Câu lệnh switch trong Go

Câu lệnh `switch` được sử dụng để thay thế nhiều nhánh `if/else if`. Ví dụ:

### **1. Cơ bản**
```go
switch i {
case 1:
    fmt.Println("one")
case 2:
    fmt.Println("two")
case 3:
    fmt.Println("three")
}
```

### **2. Gộp nhiều điều kiện**
```go
switch time.Now().Weekday() {
case time.Saturday, time.Sunday:
    fmt.Println("It's the weekend")
default:
    fmt.Println("It's a weekday")
}
```

### **3. Không có biểu thức**
```go
t := time.Now()
switch {
case t.Hour() < 12:
    fmt.Println("It's before noon")
default:
    fmt.Println("It's after noon")
}
```

### **4. So sánh kiểu**
```go
whatAmI := func(i interface{}) {
    switch t := i.(type) {
    case bool:
        fmt.Println("I'm a bool")
    case int:
        fmt.Println("I'm an int")
    default:
        fmt.Printf("Don't know type %T\n", t)
    }
}

whatAmI(true)
whatAmI(1)
whatAmI("hey")
```

Kết quả:

```
I'm a bool
I'm an int
Don't know type string
```

Nguồn tham khảo: [go.dev](https://go.dev), [w3schools](https://www.w3schools.com), [tutorialspoint](https://www.tutorialspoint.com)