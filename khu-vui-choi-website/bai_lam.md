# BÀI LÀM – HACKATHON 02

- **Mã đề:** 04
- **Họ tên:Tran Thien Thuat
- **Lớp:CNTT1
- **Link repository:https://github.com/pocket1409-stack/Kiem-tra-cuoi-ky
- **Hệ điều hành (Windows/macOS):Windows

## 4.2. Thao tác máy tính cơ bản bằng CLI

### Các lệnh đã chạy

```shell
# pwd
mv noi_quy_khu_choi.txt docs/
 mkdir backup/
 rm temp_404.tmp
 cd logs/


```

### Kết quả liệt kê toàn bộ dự án (Windows: Get-ChildItem -Recurse -Force; macOS: ls -aR)
ls -Force
```Get-ChildItem -Recurse



```

## 4.3. Lọc log truy cập website

### a) Lệnh lọc các dòng status=500

```shell
#  Get-Content logs/entry.log|Select-String "status=500">logs/loi_500.txt

```

### 2 dòng đầu tiên trong logs/loi_500.txt

```
2026-04-28 08:11:50 POST /api/thanh-toan status=500
2026-04-28 08:21:23 POST /api/dat-tiec status=500


```

### b) Lệnh đếm số dòng status=404 và kết quả

```shell
#  Get-Content logs/entry.log|Select-String "status=404"|Measure-object

```

```text
4

```

## 4.4. Chạy script tong_hop (.ps1 hoặc .sh)

### Lệnh chạy (Windows: nếu dùng Phụ lục 2 thì ghi cả 2 lệnh)
 Get-content logs/entry.log|Select-string "status=404">>logs/tong_hop.txt
 Get-content logs/entry.log|Select-string "status=500"|Measure-Object >>logs/tong_hop.txt
```shell
# 

```

### Nội dung file logs/tong_hop.txt

```text
=== BAO CAO SU CO WEBSITE ===

2026-04-28 08:23:34 GET /ve-tet-2025 status=404
2026-04-28 08:29:56 GET /images/nha-bong-2.jpg status=404
2026-04-28 08:49:51 GET /images/nha-bong-2.jpg status=404
2026-04-28 09:00:35 GET /tin-tuc status=404




Count    : 6
Average  : 
Sum      : 
Maximum  : 
Minimum  : 
Property : 


```

## 4.5. README.md và bảo vệ thông tin bí mật

> README.md, .gitignore và .env.example được chấm trực tiếp trên file ở gốc dự án. Đánh dấu `[x]` vào các mục đã làm để tự kiểm tra.

- [x] README.md: Heading 1, mô tả có **in đậm** và *in nghiêng*, bảng, code block, task list, blockquote
- [x] .gitignore có dòng `.env` (tên file đúng, không có đuôi .txt)
- [x] .env.example có đủ tên biến, giá trị để trống (tên file đúng, không có đuôi .txt)

## 4.6. Kiểm tra trang web bằng DevTools (F12) và báo cáo lỗi

### Bảng lỗi

| STT | Tab DevTools phát hiện lỗi | Tên file hoặc thông báo lỗi | Cách khắc phục |
| --- | --- | --- | --- |
| 1 |  |  |  |
| 2 |  |  |  |

> Ảnh chụp màn hình lưu trong thư mục `evidence/` (network.png, console.png).

### Báo cáo lỗi gửi trưởng nhóm

- **Context:** 
- **Expected:** 
- **Actual:** 
- **Log:** 

### Câu tìm kiếm Google

```text
(Ghi câu tìm kiếm vào đây – xoá dòng này)

```

## 4.7. Excel

> Phần Excel được chấm trực tiếp trên file `data/ve_vao_cong_thang_4.xlsx`, không cần ghi vào đây.
