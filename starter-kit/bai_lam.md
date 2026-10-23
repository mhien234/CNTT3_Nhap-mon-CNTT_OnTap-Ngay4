# BÀI LÀM – THI THỬ HACKATHON 01

- **Mã đề:** Thi thử
- **Họ tên:Tran Minh Hien** 
- **Lớp:cCNTT3** 
- **Link repository:** 
- **Hệ điều hành (Windows/macOS):**

## 4.2. Thao tác máy tính cơ bản bằng CLI

### Các lệnh đã chạy

```shell
# Ghi lần lượt các lệnh đã chạy, mỗi lệnh một dòng
PS D:\rikkei-app\Thực Hành MarkDown.Minh Hiển\starter-kit\starter-kit\van-phong-pham-website> pwd
PS D:\rikkei-app\Thực Hành MarkDown.Minh Hiển\starter-kit\starter-kit\van-phong-pham-website> ls -Force
PS D:\rikkei-app\Thực Hành MarkDown.Minh Hiển\starter-kit\starter-kit\van-phong-pham-website> mv .\logo_van_phong_pham.PNG .\media\
PS D:\rikkei-app\Thực Hành MarkDown.Minh Hiển\starter-kit\starter-kit\van-phong-pham-website> mv .\nhap_hang.txt .\docs\
PS D:\rikkei-app\Thực Hành PS D:\rikkei-app\Thực Hành MarkDown.Minh Hiển\starter-kit\starter-kit\van-phong-pham-website> rm .\temp_131.tmp
PS D:\rikkei-app\Thực Hành MarkDown.Minh Hiển\starter-kit\starter-kit\van-phong-pham-website> cd .\logs\
PS D:\rikkei-app\Thực Hành MarkDown.Minh Hiển\starter-kit\starter-kit\van-phong-pham-website\logs> ls
```

### Kết quả liệt kê toàn bộ dự án (Windows: Get-ChildItem -Recurse -Force; macOS: ls -aR)

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.3. Lọc log thủ công

### Lệnh đã chạy

```shell
# Ghi lệnh vào đây
PS D:\rikkei-app\Thực Hành MarkDown.Minh Hiển\starter-kit\starter-kit\van-phong-pham-website> Get-Content .\logs\shop.log | Select-String "ERROR"

PS D:\rikkei-app\Thực Hành MarkDown.Minh Hiển\starter-kit\starter-kit\van-phong-pham-website> Get-Content .\logs\shop.log | Select-String "ERROR" > .\logs\daily_report.txt

```

### 2 dòng lỗi đầu tiên trong daily_report.txt

```text
logs\shop.log:3:2025-10-28 08:24:28 [ERROR] Thanh toan bi tu choi
logs\shop.log:5:2025-10-28 08:30:28 [ERROR] Thanh toan bi tu choi

```

## 4.4. Thao tác với tài liệu Markdown (README.md)

> README.md được chấm trực tiếp trên file `README.md` ở gốc dự án. Đánh dấu `[x]` vào các mục đã làm để tự kiểm tra.

- [x] Heading 1: tên dự án
- [x] Mô tả ngắn có cả **in đậm** và *in nghiêng*
- [x] Bảng `Thư mục | Nội dung`, ít nhất 3 dòng dữ liệu
- [x] Code block chứa lệnh PowerShell/Terminal liệt kê nội dung dự án
- [x] Task list ít nhất 2 công việc, có ít nhất 1 mục đã hoàn thành
- [x] Blockquote nhắc không upload `.env`

## 4.5. Chạy script auto_report (.ps1 hoặc .sh)

### Lệnh chạy (Windows: nếu dùng Phụ lục 2 thì ghi cả 2 lệnh)

```shell
# ghi lệnh vào đây 
PS D:\rikkei-app\Thực Hành MarkDown.Minh Hiển\starter-kit\starter-kit\van-phong-pham-website> .\auto_report.ps1

```

### Nội dung file logs/auto_report.txt

```text "=== BAO CAO LOI ===" > .\logs\auto_report.txt
=== BAO CAO LOI ===

2025-10-28 08:24:28 [ERROR] Thanh toan bi tu choi
2025-10-28 08:30:28 [ERROR] Thanh toan bi tu choi
2025-10-28 08:33:28 [ERROR] Ket noi kho du lieu that bai
2025-10-28 08:39:28 [ERROR] Ket noi kho du lieu that bai
2025-10-28 08:42:28 [ERROR] Ket noi kho du lieu that bai
2025-10-28 09:12:28 [ERROR] Thanh toan bi tu choi


```

## 4.6. Đếm số dòng lỗi

### Lệnh

```shell
# Ghi lệnh vào đây 
PS D:\rikkei-app\Thực Hành MarkDown.Minh Hiển\starter-kit\starter-kit\van-phong-pham-website> Get-Content .\logs\shop.log | Select-String "ERROR" | Measure-Object -Line

```

### Kết quả đếm (Windows: giá trị Count; macOS: con số in ra)

```text
Lines Words Characters Property
----- ----- ---------- --------
    6

```

## 4.7. Báo cáo tổng hợp

### Các lệnh đã chạy

```shell
# Ghi lần lượt các lệnh đã chạy, mỗi lệnh một dòng (xoá dòng này)

```

### Nội dung file logs/tong_hop.txt

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.8. Excel

> Phần Excel được chấm trực tiếp trên file `data/don_ban_thang_10.xlsx`, không cần ghi vào đây.
