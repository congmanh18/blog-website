---
title: Microsoft Chọn Go Để Tái Thiết TypeScript - Tại sao không phải C# hay Rust?
published: 2025-03-13
description: Microsoft đã quyết định sử dụng Go để tái thiết TypeScript, một quyết định bất ngờ nhưng có cơ sở. Hãy cùng tìm hiểu lý do và kết quả của dự án này!
tags: [microsoft, typescript, go]
image: "./cover.jpg"
category: Tech
draft: false
---

Microsoft đã gây bất ngờ lớn vào đầu tháng 3 khi công bố một quyết định đầy táo bạo: **Viết lại toàn bộ trình biên dịch TypeScript bằng Go** – ngôn ngữ lập trình do Google phát triển. Quyết định này đi ngược lại những dự đoán phổ biến, khi nhiều chuyên gia cho rằng Microsoft sẽ chọn **C#** hoặc **Rust**, hai công nghệ nổi bật trong cộng đồng lập trình.

## **Tại Sao Lại Là Go?**

TypeScript hiện là một trong những ngôn ngữ quan trọng nhất đối với Microsoft, đặc biệt trong phát triển web. Việc chọn một công nghệ từ đối thủ cạnh tranh để cải tiến sản phẩm của mình thực sự là một bước đi táo bạo.

**Anders Hejlsberg**, người sáng lập TypeScript và C#, chia sẻ trong video giới thiệu dự án **“Corsa”** rằng nhóm phát triển đã thử nghiệm với nhiều ngôn ngữ khác nhau trước khi quyết định chọn **Go**. Ông giải thích rằng Go sở hữu nhiều lợi thế nổi bật:

- **Hiệu suất cao**, đặc biệt khi xử lý các tác vụ song song.
- **Bộ thu gom rác tự động**, giúp tối ưu hóa quản lý bộ nhớ.
- **Cấu trúc cú pháp tương đồng với JavaScript**, giúp quá trình chuyển đổi trở nên dễ dàng và mượt mà hơn so với các ngôn ngữ khác.

## **Hiệu Suất Đột Phá Với TypeScript Viết Bằng Go**

Kết quả của việc chuyển đổi TypeScript sang Go thật sự ấn tượng. Theo Microsoft, phiên bản mới của trình biên dịch TypeScript mang lại hiệu suất **gấp 10 lần so với bản hiện tại**.

Ví dụ điển hình là dự án **VS Code**, thời gian biên dịch đã giảm mạnh từ **78 giây xuống chỉ còn 7,5 giây** – một cải tiến vượt bậc mà bất kỳ lập trình viên nào cũng ao ước. Điều này hứa hẹn sẽ **tăng năng suất làm việc**, đặc biệt đối với các dự án lớn với nhiều tệp TypeScript.

## **Lộ Trình Phát Hành TypeScript 7.0**

Microsoft dự kiến phát hành **phiên bản beta** của trình biên dịch TypeScript mới vào giữa năm **2025**, với bản chính thức sẽ được ra mắt vào cuối năm. Phiên bản này sẽ mang tên **TypeScript 7.0**, trong khi vẫn duy trì nhánh **6.x** của TypeScript cũ để đảm bảo tính ổn định trong suốt quá trình chuyển đổi.

## **Cộng Đồng Phản Ứng Như Thế Nào?**

Quyết định của Microsoft đã nhận được rất nhiều phản ứng trái chiều. Một số lập trình viên **C#** bày tỏ sự thất vọng vì Microsoft không chọn ngôn ngữ của mình cho dự án quan trọng này. Tuy nhiên, **Ryan Cavanaugh**, trưởng nhóm phát triển TypeScript, đã giải thích rằng việc sử dụng **Rust** có thể khiến họ mất **nhiều năm** để hoàn thiện và có thể phá vỡ tính tương thích với hệ thống hiện tại. Ngược lại, với **Go**, nhóm có thể hoàn thành dự án trong vòng một năm và đảm bảo **tính tương thích cao nhất**.

## **Kết Luận**

Microsoft quyết định sử dụng **Go** để tái thiết TypeScript là một bước đi đầy bất ngờ, nhưng hoàn toàn có cơ sở. Với những lợi ích vượt trội về **hiệu suất, tốc độ biên dịch và khả năng tương thích**, quyết định này có thể sẽ là một cột mốc quan trọng giúp TypeScript trở nên mạnh mẽ hơn trong tương lai.

**Liệu quyết định này có mang lại thành công lớn cho Microsoft?** Hãy cùng chờ đón và xem liệu điều này có thay đổi diện mạo của TypeScript trong thế giới lập trình! 🚀
