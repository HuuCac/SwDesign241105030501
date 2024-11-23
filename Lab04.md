# 1. Ca sử dụng cho Nhân viên
### Ca sử dụng 1: Xem thông tin cá nhân
  Diễn viên: Nhân viên <br> 
  Tiền điều kiện: Nhân viên đã đăng nhập vào hệ thống. <br> 
  Các bước: <br> 
    - Nhân viên chọn mục "Thông tin cá nhân" trên menu chính. <br> 
    - Hệ thống hiển thị đầy đủ thông tin cá nhân của nhân viên (họ tên, ngày sinh, địa chỉ, số điện thoại, email, phòng ban, chức vụ, ...). <br> 
    - Hậu điều kiện: Nhân viên đã xem được thông tin cá nhân của mình. <br> 

### Ca sử dụng 2: Cập nhật thông tin cá nhân
  Diễn viên: Nhân viên <br> 
  Tiền điều kiện: Nhân viên đã đăng nhập vào hệ thống. <br> 
  Các bước: <br> 
    - Nhân viên chọn mục "Cập nhật thông tin cá nhân". <br> 
    - Hệ thống hiển thị form để nhân viên nhập thông tin cần cập nhật. <br> 
    - Nhân viên nhập thông tin mới và nhấn "Lưu". <br> 
    - Hệ thống cập nhật thông tin và hiển thị thông báo xác nhận. <br> 
    - Hậu điều kiện: Thông tin cá nhân của nhân viên đã được cập nhật. <br> 

### Ca sử dụng 3: Xem lịch sử bảng lương
  Diễn viên: Nhân viên <br> 
  Tiền điều kiện: Nhân viên đã đăng nhập vào hệ thống và hệ thống đã tính toán lương cho các kỳ trước. <br> 
  Các bước: <br> 
    - Nhân viên chọn mục "Lịch sử bảng lương". <br> 
    - Hệ thống hiển thị danh sách các bảng lương đã được tính toán cho nhân viên. <br> 
    - Nhân viên chọn một bảng lương cụ thể để xem chi tiết. <br> 
    - Hậu điều kiện: Nhân viên đã xem được chi tiết bảng lương của kỳ đã chọn.<br> 

# 2. Ca sử dụng cho Quản lý
### Ca sử dụng 1: Thêm mới nhân viên
  Diễn viên: Quản lý <br> 
  Tiền điều kiện: Quản lý đã đăng nhập vào hệ thống. <br> 
  Các bước: <br> 
    - Quản lý chọn mục "Quản lý nhân viên" và chọn "Thêm mới". <br> 
    - Hệ thống hiển thị form để nhập thông tin nhân viên mới. <br> 
    - Quản lý nhập đầy đủ thông tin và nhấn "Lưu". <br> 
    - Hậu điều kiện: Nhân viên mới đã được thêm vào hệ thống. <br> 

### Ca sử dụng 2: Sửa thông tin nhân viên
  Diễn viên: Quản lý <br> 
  Tiền điều kiện: Quản lý đã đăng nhập vào hệ thống. <br> 
  Các bước: <br> 
    - Quản lý chọn mục "Quản lý nhân viên" và chọn nhân viên cần sửa. <br> 
    - Hệ thống hiển thị thông tin hiện tại của nhân viên. <br> 
    - Quản lý sửa các thông tin cần thiết và nhấn "Lưu". <br> 
    - Hậu điều kiện: Thông tin nhân viên đã được cập nhật. <br> 

### Ca sử dụng 3: Phê duyệt bảng lương
  Diễn viên: Quản lý <br> 
  Tiền điều kiện: Bảng lương đã được tính toán và chờ phê duyệt. <br> 
  Các bước: <br> 
    - Quản lý chọn mục "Phê duyệt bảng lương". <br> 
    - Hệ thống hiển thị danh sách các bảng lương chờ phê duyệt. <br> 
    - Quản lý xem chi tiết từng bảng lương và chọn "Phê duyệt" hoặc "Từ chối". <br> 
    - Hậu điều kiện: Bảng lương đã được phê duyệt hoặc từ chối. <br> 

### Ca sử dụng 4: Xem báo cáo tổng hợp
  Diễn viên: Quản lý <br> 
  Tiền điều kiện: Quản lý đã đăng nhập vào hệ thống. <br> 
  Các bước: <br> 
    - Quản lý chọn mục "Báo cáo". <br> 
    - Hệ thống hiển thị danh sách các loại báo cáo (ví dụ: báo cáo lương theo phòng ban, báo cáo thuế TNCN). <br> 
    - Quản lý chọn loại báo cáo cần xem và chọn khoảng thời gian. <br> 
    - Hệ thống hiển thị báo cáo theo yêu cầu. <br> 
    - Hậu điều kiện: Quản lý đã xem được báo cáo. <br> 

# 3. Ca sử dụng cho Kế toán
### Ca sử dụng 1: Xuất hóa đơn lương
  Diễn viên: Kế toán <br> 
  Tiền điều kiện: Bảng lương đã được phê duyệt. <br> 
  Các bước: <br> 
    - Kế toán chọn mục "Xuất hóa đơn lương". <br> 
    - Hệ thống hiển thị danh sách các bảng lương đã được phê duyệt. <br> 
    - Kế toán chọn bảng lương cần xuất hóa đơn và nhấn "Xuất". <br> 
    - Hệ thống tạo và xuất file hóa đơn lương. <br> 
    - Hậu điều kiện: Hóa đơn lương đã được xuất thành công. <br> 

### Ca sử dụng 2: Nộp thuế
  Diễn viên: Kế toán <br> 
  Tiền điều kiện: Bảng lương đã được phê duyệt và đã xuất hóa đơn. <br> 
  Các bước: <br> 
    - Kế toán chọn mục "Nộp thuế". <br> 
    - Hệ thống tính toán số thuế phải nộp và tạo file khai thuế. <br> 
    - Kế toán kiểm tra và nộp file khai thuế. <br> 
    - Hậu điều kiện: Thuế đã được nộp. <br> 

### Ca sử dụng 3: Đối chiếu số liệu với ngân hàng
  Diễn viên: Kế toán <br> 
  Tiền điều kiện: Bảng lương đã được thanh toán. <br> 
  Các bước: <br> 
    - Kế toán chọn mục "Đối chiếu số liệu". <br> 
    - Hệ thống so sánh số liệu thanh toán trên hệ thống với số liệu từ ngân hàng. <br> 
    - Kế toán kiểm tra và đối chiếu các khoản chênh lệch. <br> 
    - Hậu điều kiện: Số liệu đã được đối chiếu. <br> 

# 4. Ca sử dụng cho Hệ thống
### Ca sử dụng 1: Tự động tính lương hàng tháng
  Diễn viên: Hệ thống <br> 
  Tiền điều kiện: Đến ngày cuối tháng hoặc ngày được cấu hình. <br> 
  Các bước: <br> 
    - Hệ thống tự động thu thập dữ liệu chấm công, thông tin nhân viên. <br> 
    - Hệ thống tính toán lương theo công thức đã được cài đặt. <br> 
    - Hệ thống tạo bảng lương và gửi thông báo cho quản lý để phê duyệt. <br> 
    - Hậu điều kiện: Bảng lương đã được tính toán và sẵn sàng để phê duyệt. <br> 

### Ca sử dụng 2: Gửi email thông báo bảng lương
  Diễn viên: Hệ thống <br> 
  Tiền điều kiện: Bảng lương đã được phê duyệt. <br> 
  Các bước: <br> 
    - Hệ thống gửi email thông báo đến từng nhân viên về bảng lương của họ. <br> 
    - Hậu điều kiện: Nhân viên đã nhận được email thông báo. <br> 

### Ca sử dụng 3: Lưu trữ lịch sử bảng lương
  Diễn viên: Hệ thống <br> 
  Tiền điều kiện: Bảng lương đã được tính toán và lưu trữ. <br> 
  Các bước: <br> 
    - Hệ thống lưu trữ bảng lương vào cơ sở dữ liệu. <br> 
    - Hậu điều kiện: Bảng lương đã được lưu trữ để tra cứu sau này. 
