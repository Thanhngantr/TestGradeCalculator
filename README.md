# Test Grade Calculator

## Mô tả dự án
Tên dự án: Tính toán và phân tích điểm thi (Test Grade Calculator)
Chương trình được viết bằng Python để tính toán và phân tích điểm thi trắc nghiệm từ file txt chứa câu trả lời của học sinh.
Mục đích của chương trình giúp giảm thời gian chấm điểm
Dữ liệu mỗi dòng gồm:
```
N00000001,A,A,D,D,C,D,D,A,,C,D,B,C,,B,C,B,D,A,C,,A,,C,D
```
Trong đó:
- `N00000001` là số ID của sinh viên (bắt đầu bằng 'N' và theo sau là 8 chữ số)
-  25 chữ cái sau là câu trả lời của học sinh cho kỳ thi được phân tách bằng dấu phẩy.

##  Yêu cầu 
- Python 3.9
  Yêu cầu thư viện: 
- pandas
- numpy
##  Chức năng chương trình
Chương trình gồm 4 task chính:

### TASK 1 – Mở file dữ liệu
- Nhập tên lớp (ví dụ: `class1`)
- Đọc file: `class1.txt`
- Xử lý lỗi nếu file không tồn tại
- Đọc từng dòng đầy đủ, không bỏ sót dòng lỗi

###  TASK 2 – Kiểm tra định dạng từng dòng
- Kiểm tra:
- Dòng phải có đúng 26 giá trị (1 ID + 25 câu trả lời)
- ID phải hợp lệ (bắt đầu bằng 'N' và theo sau là 8 chữ số)
- In ra lỗi nếu có dòng sai định dạng
- Báo cáo số dòng hợp lệ và không hợp lệ

###  TASK 3 – Chấm điểm bài thi và phân tích
- Chấm điểm theo quy tắc:
  - Đúng: +4 điểm
  - Sai: -1 điểm
  - Bỏ qua: 0 điểm
- Tính thống kê:
  - Số học sinh điểm > 80
  - Trung bình, cao nhất, thấp nhất, miền giá trị, trung vị
  - Câu hỏi bị bỏ qua nhiều nhất và sai nhiều nhất

###  TASK 4 – Ghi file kết quả
- Xuất file mới tên `<tên_lớp>_grades.txt`
- Mỗi dòng bao gồm `ID,Score`

---
Hướng dẫn chạy
1. Mở file notebook `tran_thanhngan_grade_the_exams`
2. Chạy toàn bộ cell trong notebook
3. Khi được yêu cầu nhập, nhập tên lớp (VD: class1, không cần `.txt`)
4. Xem kết quả trên màn hình và trong file xuất ra.
**Lưu ý**: Đảm bảo file notebook và các file dữ liệu nằm cùng thư mục.
---
