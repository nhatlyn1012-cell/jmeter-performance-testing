# BÁO CÁO THỰC HÀNH APACHE JMETER

## 1. Mục tiêu

- Tìm hiểu công cụ kiểm thử hiệu năng Apache JMeter.
- Xây dựng và thực hiện kịch bản kiểm thử tải website.
- Thu thập kết quả và tạo báo cáo HTML.

## 2. Công cụ sử dụng

- Apache JMeter 5.6.3
- Java OpenJDK 25
- GitHub Codespaces
- GitHub Repository

## 3. Nội dung thực hành

**Website kiểm thử:** https://jmeter.apache.org/

Em tạo file `jmeter-test-plan.jmx` với các thông số:

| Thông số | Giá trị |
|---|---|
| Phương thức HTTP | GET |
| Số người dùng ảo | 5 |
| Số vòng lặp | 2 |
| Thời gian tăng tải | 5 giây |
| Tổng yêu cầu dự kiến | 10 |

Lệnh thực hiện kiểm thử:

```bash
./apache-jmeter-5.6.3/bin/jmeter -n -t jmeter-test-plan.jmx -l results.jtl -e -o report
```

## 4. Kết quả

Kết quả kiểm thử được lưu trong file `results.jtl`. Báo cáo HTML được tạo trong thư mục `report`.

## 5. Kết luận

Qua bài thực hành, em đã biết cách sử dụng Apache JMeter để xây dựng kịch bản kiểm thử tải, gửi yêu cầu HTTP, lưu kết quả và tạo báo cáo HTML. GitHub Codespaces giúp thực hiện bài thực hành trực tiếp trên trình duyệt mà không cần cài đặt JMeter trên máy tính cá nhân.

## 6. Tài liệu tham khảo

- Apache JMeter: https://jmeter.apache.org/
- JMeter User Manual: https://jmeter.apache.org/usermanual/
