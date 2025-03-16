---
title: Hãy là một kỹ sư, đừng chỉ là người dùng framework
published: 2025-03-16T12:46:37.121Z
description: Bài viết này là một lời kêu gọi bạn hãy tự nâng cao kỹ năng. Bạn làm được mà. Trở thành một kỹ sư thực thụ nhé. Như thường lệ, trước hết phải nói rõ - Các kỹ sư chắc chắn nên (và thực tế vẫn) sử dụng framework...
tags: [framework, programmer, engineer]
image: "./cover.webp"
category: Tech
draft: false
---

**Tác giả** [John Raines](https://johndanielraines.medium.com/)  
**Nguồn** [Medium](https://johndanielraines.medium.com/be-an-engineer-not-a-frameworker-c58fe28d0c88)

Bài viết này là một lời kêu gọi bạn hãy tự nâng cao kỹ năng. Bạn làm được mà. Trở thành một **kỹ sư thực thụ** nhé. Như thường lệ, trước hết phải nói rõ: Các kỹ sư chắc chắn nên (và thực tế vẫn) sử dụng framework. Chúng là những sản phẩm tuyệt vời của kỹ thuật, giúp hoàn thành công việc một cách có tính bảo trì cao. Các framework không phải là “kẻ thù” của bài viết này. **Hoan hô các framework!** Được rồi, đủ rồi.

# Vậy framework là gì?

**Framework** là các công cụ phần mềm cung cấp một “bộ khung” để hoàn thành các dự án phần mềm nhất định. Ví dụ, nếu bạn muốn viết một single-page web app bằng TypeScript, bạn không cần phải tự làm từ đầu vì đã có **Angular**. Bạn muốn làm Machine Learning bằng Python? Mình xin giới thiệu **Scikit-Learn** và **Keras**. Muốn viết backend bằng C#? (Ồ, bạn sành điệu quá đó). Chắc hẳn bạn đã biết **ASP.NET**. Mình có thể tiếp tục liệt kê đến 1500 từ, nhưng ý chính bạn cũng hiểu rồi.

Nếu bạn thành thạo một framework, bạn thường có thể kiếm được công việc mang danh “engineer” (kỹ sư) trong chức danh, đôi khi cả “machine learning”. Nếu bạn biết hai framework, bạn thậm chí có thể tìm được việc làm có thêm cụm “full stack” vào chức danh. Nhưng bộ kỹ năng của bạn phải “đào sâu” hơn nhiều so với các framework, nếu bạn muốn thành công ở công việc kế tiếp — nơi họ tuyển bạn vì bạn có 3-5 năm kinh nghiệm “kỹ sư”. Nếu không, bạn sẽ ngồi vào một chiếc ghế rất khó chịu khi đến buổi đánh giá 90 ngày.

# Bạn có thể phải trải qua một hành trình:

#### Từ `Frameworker` (người chuyên dựa vào framework) thành `Programmer` (người lập trình chuyên sâu) rồi trở thành `Engineer` (kỹ sư).

## **The Frameworker (Người chuyên dùng framework)**

Việc bạn chủ yếu dùng một (hoặc vài) framework không đương nhiên có nghĩa bạn là “Frameworker”. Nhưng bạn có thể đang ở trạng thái đó.

Các framework cho phép một “Frameworker” xây dựng sản phẩm phần mềm tương tự như cách IKEA cho phép mình lắp ráp kệ tủ. Khi xong việc, mình đã lắp được một chiếc kệ? Đúng vậy. Mình có nên gọi bản thân là “Kỹ sư kệ tủ” không? Có lẽ không.

### **Frameworker thiếu điều gì?**

1. **Kiến thức về ngôn ngữ lập trình**: Thông thường, Frameworker chỉ có kiến thức khá cơ bản về ngôn ngữ lập trình mà framework đó sử dụng. Tệ hơn, họ có thể không tự nhận thức được lỗ hổng này, vì framework vốn được thiết kế để cung cấp các tầng trừu tượng, giúp người dùng không phải bận tâm đến nhiều khía cạnh lập trình.

2. **Độ sâu về kiến thức**: Frameworker cũng thiếu độ sâu về vấn đề phần mềm mà họ dùng framework để giải quyết. Một framework phản ánh một cách (tức là một cách triển khai) để hiện thực hóa một ý tưởng sản phẩm phần mềm.

### **Tác hại của việc chỉ là một Frameworker**

1. **Ảnh hưởng đến sự nghiệp**: Frameworker làm việc trong vùng “lơ lửng”: viết code dựa vào framework, đủ ổn để merge, nhưng không đủ vững để vượt qua các bài kiểm tra khả năng bảo trì và mở rộng lâu dài.

2. **Tác động dài hạn**: Từ góc nhìn sự nghiệp, tương lai của một Frameworker kém tươi sáng. Rất nhiều lập trình viên với bộ kỹ năng “chung chung” đang được đào tạo ồ ạt.

## **Vậy nếu một Frameworker muốn trở thành Kỹ sư thì sao?**  
Mình đề xuất họ nên bắt đầu bằng việc trở thành **Programmer**.

## **The Programmer (Người lập trình)**

Thuật ngữ “Programmer” ở đây mình dùng theo nghĩa riêng của bài viết. Một **Programmer** là người “sống trong code”. Mà cụ thể là hai điều:

1. **Họ đọc rất nhiều code**.
2. **Họ viết đủ loại code khác nhau**.

### **1. Programmer đọc rất nhiều code**
Có một câu nói quen thuộc: “Đọc code giỏi sẽ giúp bạn viết code giỏi.” Khi bạn mới bắt đầu, đọc code là cách tuyệt vời để học cú pháp mới. Đó cũng là chìa khóa để viết code “idiomatic” (chuẩn mực) cho một ngôn ngữ cụ thể.

### **2. Programmer viết đủ loại code khác nhau**
Để thoát khỏi “vùng Frameworker”, một cách là thử viết code khác lạ với công việc thường ngày của bạn. Bạn nên “làm việc” với ngôn ngữ lập trình ở mức “thấp” hơn thường lệ, rồi tự tạo tầng trừu tượng cho riêng mình.

## **Khi nào tôi trở thành một Engineer?**

Cứ cho là với vai trò Programmer, bạn có thể làm những điều mà trước đó, khi còn là Frameworker, bạn không thể. Nhưng bạn vẫn có thể làm được nhiều thứ “ấn tượng” mà vẫn chưa phải là một **Engineer** đúng nghĩa.

Hãy tưởng tượng bạn đang tự lắp một chiếc ô tô từ các bộ phận. Nhưng hễ bạn cần gắn hai bộ phận cố định với nhau, thay vì dùng ốc vít, bạn hàn cứng chúng lại. Bạn có thể tạo ra một chiếc ô tô hoạt động khá tốt lúc đầu. Nhưng rồi một bộ phận hỏng — lại ở chỗ khó tiếp cận — buộc bạn phải gỡ bỏ một số bộ phận khác để đến được bộ phận hỏng.

## **The Engineer (Kỹ sư)**

Vậy sự chuyển đổi ưu tiên bí ẩn nào định nghĩa một Engineer? **Engineer** sẽ lên kế hoạch và viết phần mềm sao cho cân bằng giữa tính **ổn định** (stability) và tính **linh hoạt thay đổi** (change).

### **Stability (Tính ổn định)**

Phần mềm phải làm đúng chức năng. Không bị lỗi nhiều. Tin cậy. Cách người dùng tương tác với phần mềm không nên thay đổi nhanh và liên tục.

### **Change (Tính thay đổi linh hoạt)**

Engineer viết code có khả năng thích ứng với thay đổi. Engineer luôn giả định rằng bất kỳ phần mềm nào mình làm cũng có lỗi ở đâu đó. Để sửa lỗi, code cần được tổ chức tốt, dễ đọc, có logging.

# **Kết luận**

Vậy bạn đang ở đâu trên hành trình này? Đã sẵn sàng vượt qua cái “resume cấp nhập môn” để làm cho danh xưng “kỹ sư” (có khi bạn đã có trong title) trở nên xứng đáng chưa? Trở thành **Engineer** không phải đích cuối cùng, nhưng là lựa chọn tuyệt vời nếu bạn muốn vươn khỏi tầm “chỉ dùng framework”.
