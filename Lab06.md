# 1. **BankSystem:deposit**
**Xác định lớp và thuộc tính**:
   - `BankSystem`: Đại diện hệ thống ngân hàng.
   - `BankTransaction`: Quản lý giao dịch.
   - `Paycheck`: Đại diện bảng lương, chứa số tiền và thông tin nhân viên.
   - `BankInformation`: Thông tin ngân hàng (tên, số định tuyến).

**Xác định phương thức (operations)**:
   - `BankSystem.deposit(Paycheck, BankInformation)`
   - `BankTransaction.create(op, amount, routingNum)`
   - `BankTransaction.submit()`
  
## Class diagram:
![Diagram](https://www.planttext.com/api/plantuml/png/T95DJiCm48NtFiKiMocvW1UeOe7KJOLKBZ1n1eWQ_yWpNaI8atNH8t45uk84jmYlhEStdz-plywN7Gj6INPKPaHcU4HtEauiPE53mNNr53mFiWaucNSo9mtFPTT0DzltxjNhws3UHOioUBTLdwf2laHqZ2QVh5mJ2OKsFcWuIXpSMmDeVNAYuMdqA0r4dsJM3yakbcsPvTJPEL9rovAfuDjRLj78Xj5FHFj-0Tx6h0gid5pnW9RMYH_vDrj7iQPLBzYs3t_QQqXChExbR5qhQ0ZH6-B_ZFTH2tD7hiy_-Gq00F__0m00).

**Biểu đồ trạng thái**:
Trạng thái của giao dịch từ *Khởi tạo* → *Đang xử lý* → *Hoàn tất*. <br>
![Diagram](https://www.planttext.com/api/plantuml/png/UhzxlqDnIM9HIMbk3bUqLgo2hgwTWcTUPabcOavcLM99PduU5nSg7wmae2W_ERMuE3ClNS5A8HXa098G5v8iIB5pVcv1Jcf9QWfGRKXHObvnOZBOeE3IP92ojD8ST1reDg9gSqlCp4bDuU9260lI0dGybqDgNWh88m00003__mC0)

---

# 2. **PrintService:print**
**Xác định lớp và thuộc tính**:
   - `PrintService`: Quản lý việc in.
   - `PaycheckPrinterImage`: Tạo hình ảnh in từ bảng lương.
   - `PrinterInterface`: Kết nối với máy in.
   - `Employee`: Thông tin nhân viên.

**Xác định phương thức (operations)**:
   - `PrintService.print(Paycheck, String)`
   - `PaycheckPrinterImage.buildPrintImage(fromPaycheck)`
## Class diagram:
![Diagram](https://www.planttext.com/api/plantuml/png/R98zRiCm38LtdOB8P0Frq5L3aI4TkXb9By38Z2jKFuOa5p2Adgn3ZzGhL7PanOsjGH383-yzaFhz_jdxW2xqMZ6Xq7kedJJXHEv32e9F1jFfncBHuI3UIBnpgDFhuTeXzz9mE8NuRalsnMQfHDM9qTZU9C-zLCtKcUh5nLbThmnA3bDx8Ph4nkk2Yup26aCYlDf451lHhgGdqzmmEUedcqNuPzqfEz2iNu7CEgbWKDDToQD2Dt1eR7zMbEnQ2WSAA9KloiolXfHzA1dp724rEdBInX0737H4qyvrrBOtOMqQbJTz_ssugfwszyIXz-GtuFlvp-2Mo58zWWrrSVGUhCduXEHPSzWzxiPDnjZ6CxQF-FWr_m000F__0m00)

**Biểu đồ trạng thái**:
Trạng thái in: *Chuẩn bị in* → *Đang in* → *Hoàn thành*. <br>
![Diagram](https://www.planttext.com/api/plantuml/png/UhzxlqDnIM9HIMbk3bUqLgo2hgwTGa1HQa5YKMPUEXSNKAua5I6WKCsb00G8XPbv9I1rjLnSC3POmZa_jo0djIGrHS5AmIqpBxCuGw40fXPX6B8HG8N1gNaf2YNv49MfHLnS25D0Ae6MSZa0bO1S2W000F__0m00)

---

# 3. **ProjectManagementDatabase:getChargeNumbers**
**Xác định lớp và thuộc tính**:
   - `ProjectManagementDatabase`: Đại diện hệ thống cơ sở dữ liệu.
   - `ChargeNumList`: Danh sách số tính phí.
   - `ChargeNum`: Đối tượng số tính phí, chứa tên dự án và giá trị.

**Xác định phương thức (operations)**:
   - `getChargeNumbers(String)`: Truy vấn danh sách số tính phí.
   - `ChargeNumList.add(theChargeNum)`.
  
## Class diagram:
![Diagram](https://www.planttext.com/api/plantuml/png/T55B3e8m4Dtt55t2WWiGOqnqgOJ4nFr09r03nNIcRemdS-6Hl885aO-VBj-ytqmVj_kA62oxkX9v1KGojSqHSzw1WG9hDBm1XWm8vKN8xXN8wn9iWOchCxGKd5wI16gCvPwjDaKOou6prSJYAdh_6TnxHZ9_enJBTh0OQCi-5PGAkCG1dmJui7EZrOzw58JVVjzLXXe_DfaLF43b_4GrBgjmp4j7MHiu4KxgTDfstAjzZV-tZgBbnwLYQP6TDIJc-8pfMNbZ6BIdhT2ezbkV0000__y30000)

**Biểu đồ trạng thái**:
Trạng thái danh sách số: *Rỗng* → *Đang cập nhật* → *Hoàn tất*. <br>
![Diagram](https://www.planttext.com/api/plantuml/png/UhzxlqDnIM9HIMbk3bUqLgo2hgwTWcjkGKab5nUO0Wk45gGabcJcfIjOAGI35CC5kE0o86NE-Ra5EQabgIb0TM29L8NWqkJarEBYjD8SLAKGi-7At18pSr9JkBWG9e0K0Tt3vP2Qbm9o6m000F__0m00)

---

# 4. **ProjectManagementDatabase::initialize**
**Xác định lớp và thuộc tính**:
   - `DBChargeNumbers`: Kết nối cơ sở dữ liệu.
   - `DriverManager`: Quản lý kết nối.

**Xác định phương thức (operations)**:
   - `initialize()`: Thiết lập kết nối.
   - `getConnection(url, user, pass)`: Lấy kết nối đến cơ sở dữ liệu.

## Class diagram:
![Diagram](https://www.planttext.com/api/plantuml/png/N8yn3i8m34NtdC9ZaUW5Cg2AiiB22Knh1KkfWvoa0uYJCN0aha23L2hLsn_U-z-Vrxk92JNbmPlEOunmsBTNL4UdF5n88pmC_8w54wFdErKR2sFWtZpDp2YFf4SKTAH_mb5gWmXrYODKMRs5Sr8MjuKSIPTqcnnpcjmBL1hMU-fwj-gpHHTDGzANDxu0003__mC0)

**Biểu đồ trạng thái**:
Trạng thái kết nối: *Chưa kết nối* → *Đang kết nối* → *Kết nối thành công*. <br>
![Diagram](https://www.planttext.com/api/plantuml/png/UhzxlqDnIM9HIMbk3bUqLgo2hgwTWbz-YND-NbvgSabg2XSNCWyi3ULbvgKhM2a4WpGZ2N4XoI8f1cgrWglAprC8BarEJYqkJYlDGTU0OXsA7hV4p1oGWr1T0tGqbqDgNWh80m00003__mC0)

---
