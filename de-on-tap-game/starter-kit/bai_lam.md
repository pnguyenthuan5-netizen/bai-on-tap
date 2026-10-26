# BÀI LÀM – THI THỬ HACKATHON 02 (GAMEZONE)

- **Họ tên:*Nguyễn Thuận Phát* 
- **Lớp:*CNTT3* 
- **Link repository:** 
- **Hệ điều hành (Windows/macOS):*Windows* 

## 4.2. Thao tác CLI

### Các lệnh đã chạy

```shell
# Ghi lệnh vào đây
 cd..
 pwd
 ls
 mv '.\cap nhat.txt.txt' .\docs\
 mv '.\logo gamezone.png.PNG' .\media\
 rm .\temp_207.tmp
 cd logs
 Get-ChildItem
 cd ..
\

### Kết quả liệt kê toàn bộ dự án
PS C:\Users\admin\Downloads\de-on-tap-game\starter-kit\gamezone-website\logs> cd..
PS C:\Users\admin\Downloads\de-on-tap-game\starter-kit\gamezone-website> pwd

Path
----
C:\Users\admin\Downloads\de-on-tap-game\starter-kit\gamezone-website


PS C:\Users\admin\Downloads\de-on-tap-game\starter-kit\gamezone-website> ls


    Directory: C:\Users\admin\Downloads\de-on-tap-game\starter-kit\gamezone-website


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        10/26/2026   1:15 PM                backup
d-----        10/26/2026   1:19 PM                data
d-----        10/26/2026   1:14 PM                docs
d-----        10/26/2026   1:19 PM                logs
d-----        10/26/2026   1:15 PM                media
-a----        10/26/2026   1:10 PM             70 .env
-a----        10/26/2026   1:10 PM           1437 bai_lam.md
-a----        10/26/2026   1:10 PM             61 cap nhat.txt.txt
-a----        10/26/2026   1:10 PM           8542 logo gamezone.png.PNG
-a----        10/26/2026   1:10 PM             22 temp_207.tmp


PS C:\Users\admin\Downloads\de-on-tap-game\starter-kit\gamezone-website> mv '.\cap nhat.txt.txt' .\docs\
PS C:\Users\admin\Downloads\de-on-tap-game\starter-kit\gamezone-website> mv '.\logo gamezone.png.PNG' .\media\
PS C:\Users\admin\Downloads\de-on-tap-game\starter-kit\gamezone-website> rm .\temp_207.tmp
PS C:\Users\admin\Downloads\de-on-tap-game\starter-kit\gamezone-website> cd logs
PS C:\Users\admin\Downloads\de-on-tap-game\starter-kit\gamezone-website\logs> Get-ChildItem


    Directory: C:\Users\admin\Downloads\de-on-tap-game\starter-kit\gamezone-website\logs


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/26/2026   1:10 PM            986 game.log.log


PS C:\Users\admin\Downloads\de-on-tap-game\starter-kit\gamezone-website\logs> cd ..
PS C:\Users\admin\Downloads\de-on-tap-game\starter-kit\gamezone-website>
```text
(Dán kết quả vào đây)

```

## 4.3. Lọc log thủ công

### Lệnh đã chạy
cat .\logs\game.log | Select-String "ERROR" > .\logs\daily_report.txt
```shell
# Ghi lệnh vào đây

```

### 2 dòng lỗi đầu tiên trong daily_report.txt

```text
(Dán kết quả vào đây)

```2025-11-05 08:03:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:09:15 [ERROR] Mat ket noi may chu game

## 4.4. README.md

> Chấm trực tiếp trên `README.md` ở gốc dự án.

- [ ] Heading 1
- [ ] Mô tả in đậm + in nghiêng
- [ ] Bảng `Thư mục | Nội dung` (≥3 dòng)
- [ ] Code block lệnh liệt kê
- [ ] Task list (≥2 việc, ≥1 đã xong)
- [ ] Blockquote nhắc không upload `.env`

## 4.5. Chạy script auto_report

### Lệnh chạy

```shell
# Ghi lệnh vào đây
New-Item auto_report.ps1
```

### Nội dung file logs/auto_report.txt

```text
(Dán kết quả vào đây)

```

    Directory: C:\Users\admin\Downloads\de-on-tap-game\starter-kit\gamezone-website


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/26/2026   2:14 PM              0 auto_report.ps1


## 4.6. Đếm số dòng lỗi

### Lệnh

```shell
# Ghi lệnh vào đây
(cat .\logs\game.log | select-string "ERROR").count
```

### Kết quả đếm

```text
(Dán kết quả vào đây)

```6

## 4.7. Báo cáo tổng hợp

### Các lệnh đã chạy

```shell
# Ghi lệnh vào đây
"=== TONG HOP LOG GAMEZONE" > .\logs\tong_hop.txt
cat .\logs\game.log | select-string "WARNING" >> .\logs\tong_hop.txt
(cat .\logs\game.log | Select-String "ERROR" >> .\logs\tong_hop.txt).count
```

### Nội dung file logs/tong_hop.txt

```text
(Dán kết quả vào đây)

```02025-11-05 08:03:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:09:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:12:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:39:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:42:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:51:15 [ERROR] Loi luu tien trinh choi
## 4.8. Excel

> Chấm trực tiếp trên file `data/giao_dich_thang_11.xlsx`.
