# [SECURITY PAYLOAD LIBRARY]
## Allowed
### SQL Injection
'

''

' OR 1=1 --

admin'--

<script>alert(1)</script>

../../etc/passwd

%00

; ls -la

&& whoami

### XSS

<script>alert(1)</script>

<img src=x onerror=alert(1)>

"><script>alert(1)</script>

### Path Traversal

../../etc/passwd

..\..\windows\system32

### Null Byte

%00

### Command Injection

; ls -la

&& cat /etc/passwd

### Permission Scope Restriction
- View
- Search
- Read

## AI MUST NOT
### Non-Destructive Generation
- DROP, TRUNCATE, DELETE, ALTER, GRANT, REVOKE
- Data Purge, Database Cleanup
- System Shutdown, System Restart
- File Deletion
- Destructive Script

### SQL Injection
'; DROP TABLE customer;--

'; TRUNCATE TABLE customer;--

'; DELETE FROM customer;--

rm -rf /

shutdown now

### Permission Scope Restriction
- Create
- Update
- Delete
- Admin
- Permission Management

### CRITICAL SAFETY REQUIREMENT

AI tuyệt đối không được tạo bất kỳ testcase, payload, request hoặc dữ liệu nào có khả năng:

- Xoá dữ liệu
- Sửa dữ liệu
- Thay đổi cấu trúc dữ liệu
- Thay đổi quyền
- Gây gián đoạn hệ thống
