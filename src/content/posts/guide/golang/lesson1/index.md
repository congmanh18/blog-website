---
title: GO là gì? Tại sao nên học GO?
published: 2025-03-17
description: 'Chia sẻ về Golang và lý do tại sao bạn nên học Golang.'
image: './golang.png'
tags: [golang, guide, backend]
category: 'Golang'
draft: false 
--- 

:::note[GO là gì?]

GO (hay gọi là Golang) là một ngôn ngữ lập trình được phát triển tại Google vào năm 2007 bởi Robert Griesemer, Rob Pike và Ken Thompson.  
Nó là một ngôn ngữ kiểu tĩnh với cú pháp tương tự ngôn ngữ C. GO cung cấp các tính năng như:
- Thu gom rác tự động (garbage collection).
- An toàn kiểu dữ liệu.
- Khả năng nhập động.
- Các kiểu dữ liệu tích hợp nâng cao như mảng có độ dài thay đổi và bản đồ key-value.
- Thư viện chuẩn phong phú.

Ngôn ngữ lập trình GO được ra mắt vào tháng 11 năm 2009 và hiện được sử dụng trong nhiều hệ thống sản phẩm của Google.
:::

## Những thế mạnh của GO

:::tip
GO có các tính năng quan trọng đáng chú ý nhất:
:::

1. Hỗ trợ môi trường sử dụng các mẫu (pattern) tương tự như ngôn ngữ động.  
   Ví dụ: kiểu suy luận (`x := 0` là khai báo hợp lệ của một biến `x` kiểu `int`).
2. Thời gian biên dịch nhanh chóng.
3. Hỗ trợ sẵn việc xử lý đồng thời (concurrency): các xử lý dễ dàng (thông qua **Go Routine**), kênh (channel), câu lệnh chọn (select).
4. Các chương trình GO rất đơn giản, ngắn gọn và an toàn.
5. Hỗ trợ giao diện (interface) và kiểu nhúng (embedded).
6. Tạo ra tệp nhị phân gốc được liên kết tĩnh mà không phụ thuộc các thư viện bên ngoài.  
   Nói cách khác, GO biên dịch ra một file nhị phân gom tất cả các thư viện vào trong file này.

## Những tính năng GO chủ ý loại bỏ

:::important
Để giữ cho ngôn ngữ đơn giản và ngắn gọn, GO đã loại bỏ một số tính năng thường có trong các ngôn ngữ khác:
:::

1. Hỗ trợ kiểu kế thừa.
2. Hỗ trợ overload cho phương thức hoặc toán tử.
3. Hỗ trợ sự phụ thuộc vòng tròn (circular dependencies) giữa các gói.
4. Hỗ trợ số học con trỏ.
5. Hỗ trợ kiểm định giả thuyết (assertion).
6. Hỗ trợ lập trình generic (tuy nhiên, từ phiên bản 1.18, GO đã hỗ trợ generic).

## Cài đặt môi trường phát triển GO

:::note
Bạn có thể tải và cài đặt GO nhanh chóng với các bước sau:
:::

1. **Tải bản cài đặt**:  
   - Với môi trường Windows, tải file cài đặt tại:  
     [https://go.dev/dl/go1.19.3.windows-amd64.msi](https://go.dev/dl/go1.19.3.windows-amd64.msi)  
   - Với các môi trường khác, tham khảo các bản cài đặt tại:  
     [https://go.dev/dl/](https://go.dev/dl/)

2. **Chạy bản cài đặt**:  
   - Với Windows, bộ cài đặt sẽ cài GO vào thư mục `Program Files` hoặc `Program Files (x86)`.  
   - Sau khi cài đặt, mở dòng lệnh (Command Line hoặc PowerShell) và kiểm tra phiên bản GO:

     ```bash
     $ go version
     ```

3. **Hoàn tất**:  
   Bây giờ bạn đã sẵn sàng để bắt đầu viết code với GO!

## Trình soạn thảo và phát triển GO

:::tip
Bạn có thể sử dụng bất kỳ trình soạn thảo văn bản nào để viết mã nguồn GO, ví dụ:  
Notepad, OS Edit, Brief, Epsilon, EMACS, vim, vi, Eclipse, Notepad++, ...
:::

Tuy nhiên, để làm việc hiệu quả hơn, bạn nên sử dụng các công cụ hiện đại như **Visual Studio Code**.  
Công cụ này hỗ trợ nhiều plugin giúp:

- Viết code GO dễ dàng hơn.
- Hỗ trợ cú pháp GO.
- Kiểm tra lỗi.

Tải Visual Studio Code tại: [https://code.visualstudio.com/download](https://code.visualstudio.com/download)

## Hello World

Hãy bắt đầu với một chương trình đơn giản: **Hello World**.

### a. Tạo file `hello-world.go`

Với 5 dòng lệnh sau, chương trình sẽ xuất ra chữ "hello world":

```go
package main

import "fmt"

func main() {
    fmt.Println("hello world")
}
```

### b. Thực thi chương trình

Chạy chương trình bằng lệnh:

```bash
$ go run hello-world.go
```

Kết quả sẽ là:

```
hello world
```

### c. Biên dịch chương trình

Bạn cũng có thể biên dịch chương trình thành file nhị phân:

```bash
$ go build hello-world.go
```

Sau khi biên dịch, sẽ tạo ra file nhị phân `hello-world.exe`. Kiểm tra bằng lệnh:

```bash
$ ls -name
hello-world.exe
hello-world.go
```

## Kết luận

GO là một ngôn ngữ lập trình mạnh mẽ, đơn giản và dễ học. Với cú pháp ngắn gọn và hiệu quả, bạn có thể bắt đầu ngay với các ví dụ cơ bản như trên. Hãy tiếp tục khám phá các tính năng nổi bật của GO qua các bài học tiếp theo!