# Trung tâm gia sư

## Công nghệ sử dụng
- web FontEnd:    HTML5, CSS, JavaScript.
- web BackEnd:    Php.
- Cơ sở dữ liệu:  MySQL.

## Đối tượng sử dụng:
- Gia sư
- Người dùng

## Phân tích chức năng từng đối tượng
### Người dùng
- Đăng kí ,Đăng nhập, đăng xuất, Chỉnh sửa thông tin tài khoản
- Quản lý lớp học
  - Tạo lớp học
  - Nhận Người vào làm
- Đăng blog 
### Gia sư
- Đăng kí ,Đăng nhập, đăng xuất, Chỉnh sửa thông tin tài khoản
- Tìm, ứng tuyển vào lớp dạy
- Viết blog

## Cơ sở dữ liệu
- Gia sư

| Stt | Tên | Loại dữ liệu | Mô tả |
| :----: | :----: | :----: | :---- |
| 1 | id | bigint | mã tự động tăng | 
| 2 | name | varchar(50) | Tên người dùng | 
| 3 | email | varchar(100) | Địa chỉ email duy nhất | 
| 4 | phone_number | varchar(20) | Số điện thoại | 
| 5 | gender | tinyint | Giới tính: 0->nam, 1->nữ | 
| 6 | avatar | varchar(50) | Tên ảnh |
| 7 | address | varchar(250) | Địa chỉ nơi ở | 
| 8 | description | text | mô tả các nhân | 
| 9 | password | varchar(100) | Mật khẩu mã hóa | 

- Người dùng

| Stt | Tên | Loại dữ liệu | Mô tả |
| :----: | :----: | :----: | :---- |
| 1 | id | bigint | mã tự động tăng | 
| 2 | name | varchar(50) | Tên người dùng | 
| 3 | email | varchar(100) | Địa chỉ email duy nhất | 
| 4 | phone_number | varchar(20) | Số điện thoại | 
| 5 | gender | tinyint | Giới tính: 0->nam, 1->nữ | 
| 6 | avatar | varchar(50) | Tên ảnh |
| 7 | address | varchar(250) | Địa chỉ nơi ở | 
| 8 | password | varchar(100) | Mật khẩu mã hóa | 

- Môn học

| Stt | Tên | Loại dữ liệu | Mô tả |
| :----: | :----: | :----: | :---- |
| 1 | id | tinyint | mã tự động tăng | 
| 2 | name | varchar(50) | Tên môn học | 

- Lớp học

| Stt | Tên | Loại dữ liệu | Mô tả |
| :----: | :----: | :----: | :---- |
| 1 | id | bigint | mã lớp tự động tăng | 
| 2 | user_id | bigint | Mã người dùng |
| 3 | subject_id | tinyint | Mã môn học | 
| 4 | lever | tinyint | Mã môn học | 
| 5 | location | varchar(50) | Địa điểm | 
| 6 | gender | boolean | Giới tính gia sư | 
| 7 | description | text | mô công việc | 
| 8 | price | int | Tiền công(VND) |
| 9 | Created_at | time | Thời gian đăng |
| 10 | status | int | Tiền công(VND) |

- Blog gia sư 

| Stt | Tên | Loại dữ liệu | Mô tả |
| :----: | :----: | :----: | :---- |
| 1 | id | bigint | mã lớp tự động tăng | 
| 2 | user_id | bigint | Mã người dùng |
| 3 | type | boolean | loại Blog |
| 4 | title | varchar(250) | tiêu đề Blog |
| 5 | preview | varchar(250) | đoạn mô tả nhanh |
| 6 | description | text | nội dung |
| 7 | created_at | time | Thời gian đăng |
