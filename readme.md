# Mô tả bài tập
- Mô tả bài tập: Bài tập này nhằm mục đích kiểm tra hiệu suất của trang web "fcl.phenikaa-uni.edu.vn" lấy tên Testing .Quan tâm đến thời gian phản hồi, tỉ lệ lỗi, và khả năng xử lý request của máy chủ**
- # Kịch bản kiểm tra:
- - Kịch bản kiểm tra:
-     + Tạo một HTTP Request để truy cập vào trang "fcl.phenikaa-uni.edu.vn".
-     + Sử dụng JMeter để tạo tải trọng với 999 request.
-     + Thu thập dữ liệu về thời gian phản hồi, tỉ lệ lỗi, và khả năng xử lý request của máy chủ.
# Jmeter
+ Tên http request: HomePage
+ Số lượng request đã thực hiện: 999
+ Thời gian phản hồi trung bình: 9313ms
+ Thời gian xử lý request ở giữa: 8319ms
+ 90% Line: 13885ms
+ 95% Line: 14767ms
+ 99% Line: 22295ms
+ Thời gian ngắn nhất: 2722ms
+ Thời gian phản hồi lớn nhất: 24941ms
+ Tỉ lệ % số request bị lỗi (không nhận được phản hồi từ server): 0%
+ Số request mà server có thể xử lý: 999/sec
+ Thông lượng KB nhận được: 2056.94 KB/s
+ Thông lượng KB gửi đi: 8.52 KB/s

![22-1](https://github.com/Ngolinh141/Jmeter-21011613/assets/96857420/9dfe395a-f551-40f8-92d3-053d5883e46e)

# Jmeter
+ Nhóm chủ đề: 1-4
+ Thời gian bắt đầu: 2024-05-30 17:44:57
+ Thời gian tải: 8118ms
+ Thời gian kết nối: 3ms
+ Độ trễ: 5ms
+ Kích thước: 359788 bytes
+ Số bytes đã gửi: 386
+ Kích thước tiêu đề: 789 bytes
+ Kích thước tổng thể: 358999 bytes
+ Số lượng mẫu: 1
+ Số lượng lỗi: 0
+ Kiểu dữ liệu: text
+ Phản hồi: 200
+ Tin nhắn phản hồi: OK

![11-1](https://github.com/Ngolinh141/Jmeter-21011613/assets/96857420/b3aa71b0-8bcd-4b9d-a0bb-fce61b0ef48d)


# Dữ liệu này cung cấp thông tin chi tiết về một yêu cầu cụ thể(Hiệu năng trang web): 
+ Thời gian tải là 8118ms, trong đó thời gian kết nối chiếm 3ms và độ trễ chiếm 5ms.
+ Kích thước tổng thể của yêu cầu là 359788 bytes, trong đó kích thước dữ liệu là 358999 bytes và kích thước tiêu đề là 789 bytes.
+ Yêu cầu này có kiểu dữ liệu là text và nhận được phản hồi mã 200 (OK) từ máy chủ, không có lỗi xảy ra trong quá trình xử lý.
+ Điểm nổi bật là thời gian kết nối ngắn (3ms) và kích thước tổng thể lớn (358999 bytes), cho thấy yêu cầu này có thể là một yêu cầu tải về một tập tin dữ liệu lớn từ máy chủ.
![33](https://github.com/Ngolinh141/Jmeter-21011613/assets/96857420/03118028-0806-41cc-bb00-448431207fe2)

    -->Dựa vào các vấn đề trên, để kiểm tra hiệu năng của trang web, cần thực hiện các bước sau:
- Phân tích và Điều tra nguyên nhân:
    + Xác định nguyên nhân của thời gian phản hồi chậm và tỉ lệ lỗi cao.
    + Kiểm tra xem có vấn đề về cấu hình máy chủ, mã nguồn, hoặc tài nguyên hệ thống không.
- Thử nghiệm và đánh giá lại
    + Thực hiện kiểm tra lại sau khi thực hiện các biện pháp tối ưu hóa để xác định hiệu quả của chúng.
    + Theo dõi và đánh giá lại các chỉ số hiệu suất để đảm bảo rằng đã đạt được cải thiện.
- Giám sát liên tục:
    + Thực hiện giám sát liên tục để phát hiện và xử lý sớm các vấn đề về hiệu suất.
    + Sử dụng các công cụ giám sát hệ thống để theo dõi và phản ứng nhanh chóng khi có vấn đề xảy ra.
# Đề suất biện pháp cải thiện: 
+ Tối ưu hóa cấu hình máy chủ để tăng khả năng xử lý của server.
+ Kiểm tra và tối ưu hóa mã nguồn trang web để giảm thời gian phản hồi.
+ Kiểm tra và sửa các lỗi server để giảm tỉ lệ request bị lỗi.
+ Sử dụng cache để giảm lượng dữ liệu truy cập vào server.
+ Tối ưu hóa kích thước và tối thiểu hóa số lượng tài nguyên (như hình ảnh, tập tin CSS và JavaScript) được tải xuống để giảm thông lượng KB nhận được và gửi đi.


## Kiểm tra hiệu năng API

### Mục tiêu:

- Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập API thời tiết https://openweathermap.org/current.
- Chạy kịch bản kiểm tra và ghi lại kết quả.
- Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
- Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của API.
### Kịch bản kiểm tra:

- Thread Group:
  - Số lượng thread: 100
  - Thời gian chạy: 60 giây
  - Ramp-up period: 10 giây
- HTTP Request:
  - URL: https://openweathermap.org/current
  - Method: GET
  - Content encoding: UTF-8
- Listeners:
  - View Results Tree
  - Aggregate Report
### Kết quả kiểm tra:

![image](https://github.com/Ngolinh141/Jmeter-21011613/assets/96857420/868d7d4a-8229-4122-81d2-0033d7c89efc)


### Phân tích kết quả kiểm tra:

- Số lượng yêu cầu thành công: 996/1000 = 99,6%
- Số lượng yêu cầu thất bại: 4/1000 = 0,4%
- Thời gian phản hồi trung bình: 10
