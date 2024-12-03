# Payroll System Operations

## Subsystem: BankSystem
### Lớp: BankTransaction
- **`create(op: BankOperation, amount: float, routingNum: String)`**
  - **Mô tả**: Tạo một giao dịch ngân hàng mới với thông tin cụ thể.
  - **Tham số**:
    - `op`: Loại giao dịch ngân hàng (như nạp tiền, rút tiền).
    - `amount`: Số tiền giao dịch.
    - `routingNum`: Số định tuyến ngân hàng.

### Lớp: Paycheck
- **`getAmount(): float`**
  - **Mô tả**: Truy xuất số tiền từ paycheck.
- **`getEmployee(): Employee`**
  - **Mô tả**: Lấy thông tin nhân viên gắn với paycheck.

### Lớp: BankSystemInterface
- **`submit(theTransaction: BankTransaction)`**
  - **Mô tả**: Gửi một giao dịch ngân hàng để xử lý.
  - **Tham số**:
    - `theTransaction`: Đối tượng giao dịch cần gửi đi.

---

## Subsystem: PrintService
### Lớp: PrintService
- **`print(aPaycheck: Paycheck, onPrinter: String)`**
  - **Mô tả**: In thông tin paycheck lên một máy in được chỉ định.
  - **Tham số**:
    - `aPaycheck`: Paycheck cần in.
    - `onPrinter`: Tên hoặc địa chỉ máy in.

### Lớp: PaycheckPrinterImage
- **`buildPrintImage()`**
  - **Mô tả**: Tạo một hình ảnh để in từ paycheck.
- **`create(fromPaycheck: Paycheck)`**
  - **Mô tả**: Tạo một đối tượng ảnh máy in từ thông tin paycheck.

### Lớp: Employee
- **`getEmployeeID(): int`**
  - **Mô tả**: Truy xuất mã nhân viên.
- **`getEmployeeName(): String`**
  - **Mô tả**: Lấy tên của nhân viên.
- **`getAddress(): String`**
  - **Mô tả**: Lấy địa chỉ của nhân viên.

---

## Subsystem: ProjectManagementDatabase
### Lớp: ProjectManagementDatabase
- **`initialize()`**
  - **Mô tả**: Khởi tạo kết nối đến cơ sở dữ liệu quản lý dự án.
- **`getChargeNumbers(criteria: String): ChargeNumList`**
  - **Mô tả**: Truy xuất danh sách các charge numbers phù hợp với tiêu chí.
  - **Tham số**:
    - `criteria`: Điều kiện tìm kiếm charge numbers.

### Lớp: ChargeNumList
- **`add(theChargeNum: ChargeNum)`**
  - **Mô tả**: Thêm một charge number vào danh sách.
  - **Tham số**:
    - `theChargeNum`: Đối tượng charge number cần thêm.

### Lớp: ChargeNum
- **`getProjectName(): String`**
  - **Mô tả**: Lấy tên dự án liên quan đến charge number.
- **`getValue(): float`**
  - **Mô tả**: Lấy giá trị của charge number.

### Lớp: DBChargeNumbers
- **`getChargeNums(criteria: String): ChargeNumList`**
  - **Mô tả**: Thực hiện truy vấn để lấy danh sách charge numbers dựa trên tiêu chí.
  - **Tham số**:
    - `criteria`: Tiêu chí tìm kiếm charge numbers.

### Lớp: Connection
- **`createStatement(): Statement`**
  - **Mô tả**: Tạo một đối tượng Statement để thực hiện truy vấn SQL.

### Lớp: Statement
- **`executeQuery(query: String): ResultSet`**
  - **Mô tả**: Thực thi truy vấn SQL để trả về một kết quả ResultSet.
  - **Tham số**:
    - `query`: Câu truy vấn SQL.

### Lớp: ResultSet
- **`getString(columnLabel: String): String`**
  - **Mô tả**: Lấy dữ liệu dạng chuỗi từ một cột của kết quả truy vấn.
  - **Tham số**:
    - `columnLabel`: Nhãn cột trong kết quả truy vấn.
