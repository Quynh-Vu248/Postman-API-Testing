# BÁO CÁO THỰC HÀNH POSTMAN

## 1. Thông tin sinh viên

- Họ và tên: Vũ Mai Quỳnh 
- Mã sinh viên: 23010223
- Môn học: Đánh giá kiểm định chất lượng phần mềm

## 2. Mục tiêu

Bài thực hành nhằm tìm hiểu và sử dụng công cụ Postman
trong kiểm thử API.

Các nội dung thực hiện:

- Tạo HTTP Request
- Sử dụng GET, POST, PUT, DELETE
- Kiểm tra HTTP Status Code
- Kiểm tra Response JSON
- Viết Test Script bằng JavaScript

## 3. Công cụ sử dụng

- Postman Web
- GitHub

## 4. API sử dụng

Base URL:

https://jsonplaceholder.typicode.com

| Method | Endpoint | Chức năng |
|---|---|---|
| GET | /posts/1 | Lấy một bài viết |
| GET | /posts | Lấy danh sách |
| POST | /posts | Tạo bài viết |
| PUT | /posts/1 | Cập nhật |
| DELETE | /posts/1 | Xóa |

---

# 5. Thực hiện kiểm thử

## 5.1 GET - Lấy một bài viết

### Request

GET /posts/1

### Expected Result

HTTP 200 OK.

Response có các trường:
- userId
- id
- title
- body

### Kết quả
<img width="549" height="549" alt="image" src="https://github.com/user-attachments/assets/63d0a0aa-5360-453f-a25d-862e20a97df3" />



## 5.2 GET - Test Response

Các test đã thực hiện:

- Status code = 200
- Response là JSON
- Response có id
- Response có title

### Kết quả

<img width="736" height="598" alt="image" src="https://github.com/user-attachments/assets/aeaf277c-792d-4ae2-a579-19a8846457b5" />


## 5.3 GET - Lấy danh sách

Request:

GET /posts

Expected:

HTTP 200 OK và trả về danh sách JSON.

<img width="738" height="587" alt="image" src="https://github.com/user-attachments/assets/a9188cad-0e20-4dce-a3db-372273ff65ea" />


## 5.4 POST - Tạo bài viết

Request:

POST /posts
Expected:

HTTP 201 Created.

Kết quả
<img width="1048" height="559" alt="image" src="https://github.com/user-attachments/assets/ca1b1fa4-4f95-41b3-80bb-9ac149e82f94" />
## 5.5 PUT - Cập nhật bài viết

Request:

PUT /posts/1

Expected:

HTTP 200 OK.

### Test Results
<img width="561" height="536" alt="image" src="https://github.com/user-attachments/assets/6976a2bb-c49e-44a0-9a4e-d613f233cb3b" />
## 5.6 DELETE - Xóa bài viết

Request:

DELETE /posts/1

Expected:

Request được xử lý thành công.
<img width="733" height="450" alt="image" src="https://github.com/user-attachments/assets/c07f6628-de61-479e-a870-a1af8cbe53f5" />
## 6. Bảng kết quả kiểm thử
Test Case	Method	Expected	Actual	Result
TC01	GET	200	200	PASS
TC02	GET	JSON	JSON	PASS
TC03	POST	201	201	PASS
TC04	PUT	200	200	PASS
TC05	DELETE	Success	Success	PASS
## 7.Chạy toàn bộ collection
<img width="740" height="582" alt="image" src="https://github.com/user-attachments/assets/82fc0c82-62fa-4682-83ef-389f488bf46c" />
## 8. Kết luận

Các kỹ năng đã thực hiện:

Tạo HTTP Request
Gửi GET, POST, PUT, DELETE
Kiểm tra Status Code
Kiểm tra Response
Viết Test Script
Chạy Collection
Phân tích kết quả kiểm thử
