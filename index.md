---
title       : Web programming
subtitle    : Module 1. Introduction and Backgroung
author      : Huynh Xuan Phung
job         : Lecturer
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides

---

## Nội dung

>1. Lịch sử phát triển
>2. Ứng dụng web là gì?
>3. Kiến trúc Web 1.0, 2.0, 3.0
>4. Các mẫu thiết kế
>5. Cài đặt môi trường phát triển
>6. Đồ án

---

## Lịch sử phát triển

- Arpanet: ra đời vào năm 1963
- TCP/ IP: năm 1985
- World Wide Web: 1989
- Amazon: 1995
- Google: 1996
- Facebook: 2004
- Ajax: 2005
- Amazon EC2: 2006
- HTML5: 2012

---

## Web 1.0, 2.0, 3.0

- Web 1.0 - Tạo ra các trang web tĩnh, là thế hệ đầu tiên
- Web 2.0 - Tạo ra các trang web tương tác, mạng xã hội, ...
- Web 3.0 - Wen thông minh, có tính tương tác cao với người dùng

---

## Một số công nghệ nền tảng của Web 2.0, 3.0

- JavaScript, XML, JSON
- Dịch vụ web
- Điện toán đám mây
- Ứng dụng di động
- Siêu dữ liệu và máy học

---

## Ứng dụng web là gì?

- Khóa hoc này tập trung vào kiến trúc web hiện đại
- Chỉ tập trung vào kiến trúc tổng quan
- Các nội dung thực hành tập trung trên kiến trúc này
- Đây là những giao thức và chuẩn cơ bản

---

## Mô hình Client - Server

- Là mô hình cơ bản mô tả quan hệ tương tác giữa các chương trình trong ứng dụng web
- Có hai phần chính:
Server: lắng nghe các yêu cầu và trả về các tài nguyên tương ứng
Client: tạo kết nối và gởi các yêu cầu

---

## Ứng dụng web

Được truy xuất bởi người dùng thông qua mạng bằng trình duyệt web, bao gồm tập hợp các kịch bản trên server và client. Ứng dụng này được truy xuất thông qua một đường dẫn cụ thể liên kết với máy chủ web

---

## Ứng dụng web

1. Network 
- Mạng internet là hệ thống kết nối tất cả các máy tính
- Sử dụng tập giao thức chuẩn

2. Web
-  Hệ thống các liên kết tuy xuất qua giao thức HTTP
- Chứa các nội dung media
- Cấu trúc website được quy định bởi tập hợp các siêu liên kết
- Cấu trúc này làm cho website có ý nghĩa và giá trị

---

## Một số ưu và nhược điểm của ứng dụng web

---

## Kiến trúc web 1.0, 2.0, 3.0
### Web 1.0

- Đơn giản, tương tự mô hình Client - Server
- Không có nhiều tương tác, đa số là web tĩnh
- Không có phân tách về dữ liệu
- Trình duyệt wen rất đơn giản

---

## Web 1.0

- Khi ứng dụng càng phát triển, xử lý phía server càng tốt thì Web 1.0 trở nên khó khăn trong bảo trì
- Cuộc chiến giữa các trình duyệt web làm cho các chức năng phía client phát triển
- Người phát triển tạo ra nhiều ứng dụng tương tác với nhau cần phải lưu lại trạng thái
- Sự phát triển của công nghệ

---

## Ứng dụng wen

- Web 2.0, 3.0 được tổ chức tốt hơn để giải quyết độ phức tạp này
- Các chức năng trên server được xử lý thông minh hơn
- Trình duyệt web ngày càng được cải tiến

---

## Các mẫu thiết kế (Design Patterns)

- Các ứng dụng web sử dụng nhiều giao thức, ngôn ngữ lập trình và công nghệ
- Rất khó để phát triển, bảo trì và mở rộng các ứng dụng web nếu không có những nguyên lý thiết kế hợp lý
- các kỹ sư phần mềm dùng những nguyên lý chung để giải quyết cấu trúc phức tạp
- Các mẫu thiết kế cung cấp các thiết kế chung cho các hệ thống hướng đối tượng

---

## Mẫu thiết kế

- Mô tả sự tương tác giữa các đối tượng và lớp để giải quyết những vấn đề chung trong những trường hợp cụ thể
- Mẫu thiết kế được sử dụng lặp đi lặp lại nhiều lần

--- 

## Mô hỉnh Client - Server

- Phân tán các thành phần của một ứng dụng giữa client và server
- Chúng ta dùng nhiều mẫu thiết kế khác nhau để tổ chức các phần của 1 hệ thống phức tạp theo kiến trúc client - server

---

## Kiến trúc n- Lớp

- Được mô phỏng theo mô hình Client - Server, mẫu thiết kế này có tính hữu dụng cao
- Phân tách hệ thống thành các lớp khác nhau có thể cài đặt trên các phần cứng tách rời
- Mỗi lớp có 1 chức năng
- Mỗi lớp tương tác với lớp liền kề thông qua các giao diện
- Ví dụ

---

## Kiến trúc 3 lớp

- Lớp giao diện
- Lớp ứng dụng
- Lớp dữ liệu

---

## Kiến trúc 6 lớp

- Lớp ứng dụng tách thành 2 lớp: lớp dịch vụ và lớp truy xuất dữ liệu
- Lớp giao diện chia thành 2 lớp: lớp Client và lớp logic giao diện
- Web server tạo thành lớp Web







