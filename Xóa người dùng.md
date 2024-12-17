Để xóa người dùng `snipeit` mà bạn đã tạo trước đó, bạn cần thực hiện các bước sau trong MySQL:
-----------------------

Step 1: Đăng nhập vào MySQL với quyền root hoặc người dùng có quyền quản trị:
```
sudo mysql
```

Step 2: Xóa quyền của người dùng (nếu có) trước khi xóa người dùng:

Bạn cần xóa tất cả quyền mà người dùng `snipeit` có. Câu lệnh này sẽ loại bỏ quyền truy cập của người dùng `snipeit`:

```
REVOKE ALL PRIVILEGES ON *.* FROM 'snipeit'@'localhost';
```

Step 3: Xóa người dùng:

Sau khi đã thu hồi các quyền, bạn có thể xóa người dùng bằng câu lệnh sau:

```
DROP USER 'snipeit'@'localhost';
```

Step 4: Làm mới quyền để áp dụng thay đổi:

```
FLUSH PRIVILEGES;
```
















