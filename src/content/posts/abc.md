---
title: Markdown ABC
published: 2020-03-16
updated: 2020-03-16
description: 'Read more about Markdown features in Fuwari'
image: ''
tags: [Demo, Example, Markdown, Fuwari]
category: 'Examples'
draft: false 
---


Markdown trong ví dụ này được mở rộng với các tính năng tùy chỉnh, có thể được hỗ trợ bởi một trình biên dịch Markdown đặc biệt (ví dụ: Fuwari). Dưới đây là giải thích chi tiết bằng tiếng Việt:

1. Thẻ GitHub Repository

Tính năng này tạo ra một thẻ động hiển thị thông tin của một repository trên GitHub bằng cách lấy dữ liệu từ API của GitHub.

Cú pháp
::github{repo="<owner>/<repo>"}

Thay <owner> bằng tên người dùng hoặc tổ chức trên GitHub.
Thay <repo> bằng tên repository.
Ví dụ
::github{repo="saicaca/fuwari"}


Khi sử dụng, đoạn này sẽ tạo ra một thẻ hiển thị thông tin về repository fuwari thuộc sở hữu của saicaca.

2. Admonitions (Khung chú thích)

Admonitions là các khung được định dạng đặc biệt để làm nổi bật nội dung quan trọng. Có các loại khung chú thích sau:

note: Thông tin chung.
tip: Mẹo hoặc lời khuyên hữu ích.
important: Thông tin quan trọng.
warning: Cảnh báo về rủi ro tiềm ẩn.
caution: Cảnh báo về hậu quả tiêu cực.
Cú pháp cơ bản
:::<type>
Nội dung của bạn.
:::

Thay <type> bằng một trong các loại: note, tip, important, warning, hoặc caution.
Ví dụ
:::note
Thông tin mà người dùng nên chú ý, ngay cả khi chỉ lướt qua.
:::

:::tip
Thông tin tùy chọn để giúp người dùng thành công hơn.
:::

:::important
Thông tin quan trọng cần thiết để người dùng đạt được mục tiêu.
:::

:::warning
Nội dung quan trọng yêu cầu sự chú ý ngay lập tức do rủi ro tiềm ẩn.
:::

:::caution
Hậu quả tiêu cực có thể xảy ra từ một hành động.
:::

3. Tùy chỉnh tiêu đề cho Admonitions

Bạn có thể tùy chỉnh tiêu đề của khung chú thích bằng cách thêm tiêu đề trong dấu ngoặc vuông [] sau loại khung.

Cú pháp
:::<type>[Tiêu đề tùy chỉnh]
Nội dung của bạn.
:::

Ví dụ
:::note[TIÊU ĐỀ TÙY CHỈNH]
Đây là một ghi chú với tiêu đề tùy chỉnh.
:::

4. Cú pháp Admonition kiểu GitHub

Cú pháp này lấy cảm hứng từ các khung chú thích trong phần thảo luận của GitHub. Nó sử dụng ký hiệu blockquote (>) với một nhãn đặc biệt như [!NOTE] hoặc [!TIP].

Cú pháp
> [!TYPE]
> Nội dung của bạn.

Thay TYPE bằng NOTE, TIP, v.v.
Ví dụ
> [!NOTE]
> Cú pháp kiểu GitHub cũng được hỗ trợ.

> [!TIP]
> Đây là một mẹo hữu ích.

5. Kết hợp các tính năng

Bạn có thể kết hợp các tính năng này để tạo nội dung Markdown phong phú. Ví dụ:

:::tip[Mẹo hay]
Sử dụng `::github{repo="<owner>/<repo>"}` để hiển thị thông tin repository GitHub một cách động.
:::

> [!IMPORTANT]
> Hãy luôn kiểm tra Markdown của bạn trên trình biên dịch để đảm bảo tương thích.

Tóm tắt
Các tính năng này không phải là một phần của Markdown tiêu chuẩn mà là các mở rộng được cung cấp bởi một trình biên dịch đặc biệt (ví dụ: Fuwari).
Admonitions và thẻ GitHub giúp tăng tính trực quan và tương tác cho nội dung.
Tiêu đề tùy chỉnh và cú pháp kiểu GitHub mang lại sự linh hoạt trong việc trình bày và tổ chức nội dung.

Nếu bạn cần thêm ví dụ hoặc giải thích chi tiết hơn, hãy cho mình biết nhé!