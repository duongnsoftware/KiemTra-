# bai_lam

# BÀI LÀM – THI THỬ HACKATHON 02 (GAMEZONE)

- **Họ tên: Nguyễn Hải Dương**
- **Lớp:**
- **Link repository:**
- **Hệ điều hành (Windows/macOS):**

## 4.2. Thao tác CLI

### Các lệnh đã chạy

```bash
# Ghi lệnh vào đây
6.Hiển thị đường dẫn tuyệt đối thư mục hiện tại : pwd
7.Liệt kê nội dung, gồm cả file ẩn : ls -Force
8.Di chuyển cap_nhat.txt vào docs, file logo vào media : mv ./cap_nhat.txt./docs
                                                         mv./logo_game_zone.png./media
 9.Sao chép logo từ media vào backup: cp./media/logo_game_zone.png ./backup
 10.Xoá file .tmp ở gốc; không xoá file khác: rm .tmp
                                                      
```

### Kết quả liệt kê toàn bộ dự án

```
(Dán kết quả vào đây)
```

## 4.3. Lọc log thủ công

### Lệnh đã chạy

```bash
Get-Conten ./logs/game.log "ERROR" > logs/daily_report.txt

```

### 2 dòng lỗi đầu tiên trong daily_report.txt

```
2025-11-05 08:03:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:09:15 [ERROR] Mat ket noi may chu game
```

## 4.4. README.md

> Chấm trực tiếp trên `README.md` ở gốc dự án.
> 
- [x]  Heading 1
- [x]  Mô tả in đậm + in nghiêng
- [x]  Bảng `Thư mục | Nội dung` (≥3 dòng)
- [x]  Code block lệnh liệt kê
- [x]  Task list (≥2 việc, ≥1 đã xong)
- [x]  Blockquote nhắc không upload `.env`

## 4.5. Chạy script auto_report

### Lệnh chạy

```bash
Get-Content ./logs/game.log "ERROR" > logs/auto_report.txt

logs/auto_report.txt 

```

### Nội dung file logs/auto_report.txt

```
=== BAO CAO LOI GAMEZONE ===

2025-11-05 08:03:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:09:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:12:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:39:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:42:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:51:15 [ERROR] Loi luu tien trinh choi

```

## 4.6. Đếm số dòng lỗi

### Lệnh

```bash
( Get-Content ./logs/game.log | "ERROR" ) -Count
```

### Kết quả đếm

```
6 
```

## 4.7. Báo cáo tổng hợp

### Các lệnh đã chạy

```bash
=== TONG HOP LOG GAMEZONE === > tong_hop.txt 

Get-Content ./logs/game.log | WARNING 
```

### Nội dung file logs/tong_hop.txt

```
(Dán kết quả vào đây)
```

## 4.8. Excel

> Chấm trực tiếp trên file `data/giao_dich_thang_11.xlsx`.
>