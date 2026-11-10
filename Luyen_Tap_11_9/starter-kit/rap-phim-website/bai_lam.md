# BÀI LÀM – (ĐỀ LUYỆN TẬP SỐ 02)

- **Mã đề:** 02
- **Họ tên:Hoàng Xuân Nam**
- **Lớp:CNTT3**
- **Link repository:**
- **Hệ điều hành (Windows/macOS):**

## 4.2. Thao tác máy tính cơ bản bằng CLI

### Các lệnh đã chạy

```shell
# Ghi lần lượt các lệnh đã chạy, mỗi lệnh một dòng

``` pwd 
 ls 
 mkdir -p backup
mv bien_ban_ban_giao.txt docs/
cp data/ban_ve_thang_11.xlsx backup/


### Kết quả liệt kê toàn bộ dự án (Windows: Get-ChildItem -Recurse -Force; macOS: ls -aR)

```text
PS C:\Users\ADMIN\OneDrive\Ảnh\Screenshots\Luyen_Tap_11_9\starter-kit\rap-phim-website> pwd                             
                                                                                                                        
Path                                                                                                                    
----                                                                                                                    
C:\Users\ADMIN\OneDrive\Ảnh\Screenshots\Luyen_Tap_11_9\starter-kit\rap-phim-website                                     
                                                                                                                        
PS C:\Users\ADMIN\OneDrive\Ảnh\Screenshots\Luyen_Tap_11_9\starter-kit\rap-phim-website> ls                              
                                                                                                                        
    Directory: C:\Users\ADMIN\OneDrive\Ảnh\Screenshots\Luyen_Tap_11_9\starter-kit\rap-phim-website                      
                                                                                                                        
Mode                 LastWriteTime         Length Name                                                                  
----                 -------------         ------ ----                                                                  
d----          11/10/2026 12:22 PM                data                                                                  
d----          11/10/2026 12:20 PM                docs                                                                  
d----          11/10/2026 12:20 PM                evidence                                                              
d----          11/10/2026 12:22 PM                logs                                                                  
d----           11/9/2026  3:42 PM                web                                                                   
-a---           11/9/2026  3:42 PM             82 .env                                                                  
-a---           11/9/2026  3:42 PM           2611 bai_lam.md                                                            
-a---           11/9/2026  3:42 PM            172 bien_ban_ban_giao.txt                                                 
-a---           11/9/2026  3:42 PM             33 cache_991.tmp                                                         
                                                                                                                        
PS C:\Users\ADMIN\OneDrive\Ảnh\Screenshots\Luyen_Tap_11_9\starter-kit\rap-phim-website> mkdir -p backup                 
                                                                                                                        
    Directory: C:\Users\ADMIN\OneDrive\Ảnh\Screenshots\Luyen_Tap_11_9\starter-kit\rap-phim-website                      
                                                                                                                        
Mode                 LastWriteTime         Length Name                                                                  
----                 -------------         ------ ----                                                                  
d----          11/10/2026 12:26 PM                backup                                                                
                                                                                                                        
PS C:\Users\ADMIN\OneDrive\Ảnh\Screenshots\Luyen_Tap_11_9\starter-kit\rap-phim-website> mv bien_ban_ban_giao.txt docs/  
PS C:\Users\ADMIN\OneDrive\Ảnh\Screenshots\Luyen_Tap_11_9\starter-kit\rap-phim-website> cp data/ban_ve_thang_11.xlsx backup/
```

## 4.3. Lọc log truy cập website

### a) Lệnh lọc các dòng ERROR

```shell
Select-String "ERROR" server.log | Select-Object -ExpandProperty Line > loi_error.txt
```

### 2 dòng đầu tiên trong logs/loi_error.txt

```text
echo ## 4.3. Lọc log truy cập website >> bai_lam.md
echo ### a) Lọc ERROR >> bai_lam.md
echo ```cmd >> bai_lam.md
echo findstr "ERROR" logs\server.log ^> logs\loi_error.txt >> bai_lam.md
echo ``` >> bai_lam.md
echo Hai dong dau tien cua file loi_error.txt: >> bai_lam.md
echo ``` >> bai_lam.md
more +1 /e:2 logs\loi_error.txt >> bai_lam.md
echo ``` >> bai_lam.md
```

### b) Lệnh đếm số dòng WARNING và kết quả

```shell
# Get-Content logs\server.log | Select-String "WARNING" | Measure-Object | Select-Object -ExpandProperty Count

```

```text
(Dán kết quả đếm vào đây – xoá dòng này)

```

## 4.4. Chạy script tong_hop (.ps1 hoặc .sh)

### Lệnh chạy (Windows: nếu dùng Phụ lục 2 thì ghi cả 2 lệnh)

```shell
# Ghi lệnh vào đây (xoá dòng này)

```

### Nội dung file logs/tong_hop.txt

```text
(Dán nội dung file vào đây – xoá dòng này)

```

## 4.5. README.md và bảo vệ thông tin bí mật

> README.md, .gitignore và .env.example được chấm trực tiếp trên file ở gốc dự án. Đánh dấu `[x]` vào các mục đã làm để tự kiểm tra.

- [X] README.md: Heading 1, mô tả có **in đậm** và _in nghiêng_, bảng, code block, task list, blockquote
- [X] .gitignore có dòng `.env` (tên file đúng, không có đuôi .txt)
- [X] .env.example có đủ tên biến, giá trị để trống (tên file đúng, không có đuôi .txt)

## 4.6. Kiểm tra trang web bằng DevTools (F12) và báo cáo lỗi

### Bảng lỗi

| STT | Tab DevTools phát hiện lỗi | Tên file hoặc thông báo lỗi | Cách khắc phục |
| --- | -------------------------- | --------------------------- | -------------- |
| 1   |                            |                             |                |
| 2   |                            |                             |                |

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

> Phần Excel được chấm trực tiếp trên file `data/ban_ve_thang_11.xlsx`, không cần ghi vào đây.
