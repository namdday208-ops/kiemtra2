## 4.3. Lọc log truy cập website
### a) Lọc ERROR
```bash
grep "ERROR" logs/server.log > logs/loi_error.txt
```
Hai dòng đầu tiên của file loi_error.txt:
```
### a) Lọc ERROR
```bash
grep "ERROR" logs/server.log > logs/loi_error.txt
```
Hai dòng đầu tiên của file loi_error.txt:
```
`cmd
findstr
ERROR
logs\server.log
^>
logs\loi_error.txt
Hai
dong
dau
tien
cua
file
loi_error.txt:
Invalid parameter - /e:2
`powershell
Get-Content logs\server.log | Select-String "WARNING" | Measure-Object | Select-Object -ExpandProperty Count
0
