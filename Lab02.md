1. Phân tích tất cả các ca sử dụng còn lại trong hệ thống Payroll System.
# Create Administrative Report <br>
##  1. Các lớp phân tích:
   - PayrollAdministrator: Đại diện cho Quản trị viên Lương, người sẽ thực hiện việc tạo báo cáo.
   - ReportGenerator: Lớp chịu trách nhiệm tạo ra các báo cáo hành chính.
   - Report: Lớp đại diện cho báo cáo được tạo ra.
   - DataAccess: Lớp chịu trách nhiệm truy cập dữ liệu cần thiết để tạo báo cáo.
   - ReportParameters: Lớp chứa các tham số cần thiết để tạo báo cáo.

####   Biểu đồ sequence cho "Create Administrative Report":
![Diagram](https://www.planttext.com/api/plantuml/png/T9112W8n34NtdYBB3kW5kX061RSYNY2qKGkTQKapYvxDXKVo2ZhjGaVg9e77_p_aF--F8sOEtlTsSADBmYY1ORE54yN0Sg2H2j9Wc52eOiLbdNEaDKHa74Y8KxVwSSr1UnJiZQ6KD5n8p6q6wjlqKJGFCyd4Ot7PzsWUgKZ3jK9QAF-apc1NdhAg6TggHeDrANhCYoAw5m000F__0m00)

 ##   2. Nhiệm vụ của từng lớp phân tích:
   PayrollAdministrator:
   - Nhiệm vụ: Khởi tạo quá trình tạo báo cáo bằng cách gọi phương thức createReport với loại báo cáo và các tham số cần thiết.
   
   ReportGenerator:
   - Nhiệm vụ: Nhận yêu cầu từ Quản trị viên, truy cập dữ liệu cần thiết thông qua lớp DataAccess, và tạo ra báo cáo từ dữ liệu nhận được.
   
   Report:
   - Nhiệm vụ: Đại diện cho báo cáo được tạo ra, chứa thông tin về báo cáo (ví dụ: tiêu đề, nội dung, định dạng).
   
   DataAccess:
   - Nhiệm vụ: Truy cập và cung cấp dữ liệu cần thiết từ cơ sở dữ liệu để tạo báo cáo.
   
   ReportParameters:
   - Nhiệm vụ: Chứa các tham số cần thiết (ví dụ: khoảng thời gian, phòng ban) để tạo báo cáo.
     
##    3. Nhiệm vụ của từng lớp phân tích:
   PayrollAdministrator:
   - Nhiệm vụ: Khởi tạo quá trình tạo báo cáo bằng cách gọi phương thức createReport với loại báo cáo và các tham số cần thiết.
   
   ReportGenerator:
   - Nhiệm vụ: Nhận yêu cầu từ Quản trị viên, truy cập dữ liệu cần thiết thông qua lớp DataAccess, và tạo ra báo cáo từ dữ liệu nhận được.
   
   Report:
   - Nhiệm vụ: Đại diện cho báo cáo được tạo ra, chứa thông tin về báo cáo (ví dụ: tiêu đề, nội dung, định dạng).
   
   DataAccess:
   - Nhiệm vụ: Truy cập và cung cấp dữ liệu cần thiết từ cơ sở dữ liệu để tạo báo cáo.
   
   ReportParameters:
   - Nhiệm vụ: Chứa các tham số cần thiết (ví dụ: khoảng thời gian, phòng ban) để tạo báo cáo.

  ##  4. Thuộc tính và quan hệ giữa các lớp phân tích:
   a. Thuộc tính:
       PayrollAdministrator:
           - username: Tên người dùng của Quản trị viên.
           - role: Vai trò của người dùng (Quản trị viên Lương).
       ReportGenerator:
           - reportType: Loại báo cáo cần tạo.
           - data: Dữ liệu cần thiết để tạo báo cáo.
       Report:
           - title: Tiêu đề của báo cáo.
           - content: Nội dung của báo cáo.
           - format: Định dạng của báo cáo (PDF, Excel, v.v.).
       DataAccess:
           - databaseConnection: Kết nối với cơ sở dữ liệu.
       ReportParameters:
           - startDate: Ngày bắt đầu cho báo cáo.
           - endDate: Ngày kết thúc cho báo cáo.
           - department: Phòng ban liên quan.
   
  b. Quan hệ giữa các lớp:
       - PayrollAdministrator sử dụng ReportGenerator để tạo báo cáo.
       - ReportGenerator sử dụng DataAccess để lấy dữ liệu.
       - ReportGenerator tạo ra Report từ dữ liệu đã lấy.
       - ReportGenerator nhận các tham số từ ReportParameters để tạo báo cáo.

 ##   5. Biểu đồ lớp mô tả phân tích:
   ![Diagram](https://www.planttext.com/api/plantuml/png/R5F1JiCm3BttAtA4Gt-W1xI9IHmPOp_WfMO4fKdbk1FLn9Tnu9Fu1LoQfLlQ7gBesNxFpt5_ltzMWO6uQsnHQ0iXg2tqvArTrurn9Z01UrBdGibNgYuWEMYmKgzCnXqZB0Mta5AQ41Xts7hYk_i81hIeUGJtVOifO5pRyHP8g1af2FvrwMVCVaA7jwrGOicQgO6XKi-73v6AzCUnUj8xWJMIXpUIO-ZDKmES6i_wIF9isERAsZj6nnaw4cRZ2N3AXzDAU45t8tRMMgDSprSE3n3mqJid9ertbPhk5n_8-dqeJW9wJDdxJQnF4Vn4tJ6-T4ZztFCqfDJ1_z88ZKnWE2EAhfvXDRQIsboFHUWNbwmi7sQlNGqh5ueS7bAl1bCDCg8UbDXVoesFLyMrN2QSkOtYnKgevG_v0m00__y30000)

   ---
   
  # Create Employee Report <br>
  ## 1. Các lớp phân tích:
   - PayrollAdministrator: Đại diện cho Quản trị viên Lương, người sẽ thực hiện việc tạo báo cáo.
   - ReportGenerator: Lớp chịu trách nhiệm tạo ra các báo cáo hành chính.
   - Report: Lớp đại diện cho báo cáo được tạo ra.
   - DataAccess: Lớp chịu trách nhiệm truy cập dữ liệu cần thiết để tạo báo cáo.
   - ReportParameters: Lớp chứa các tham số cần thiết để tạo báo cáo.

---

 #  Login <br>


---

 #  Maintain Employee Information <br>


---

 #  Maintain Purchase Order <br>


---

 #  Run Payroll <br>


---

