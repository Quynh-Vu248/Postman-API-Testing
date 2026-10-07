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
- Kiểm tra Response Time


## 3. Công cụ sử dụng

- Postman Web
- Google Chrome
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

![GET Request](images/01-get-single-post.png)


## 5.2 GET - Test Response

Các test đã thực hiện:

- Status code = 200
- Response là JSON
- Response có id
- Response có title

### Kết quả

![GET Test](images/02-get-test-results.png)

## 5.3 GET - Lấy danh sách

Request:

GET /posts

Expected:

HTTP 200 OK và trả về danh sách JSON.

![GET All](images/03-get-all-posts.png)

---

## 5.4 POST - Tạo bài viết

Request:

POST /posts
Expected:

HTTP 201 Created.

Kết quả
<img width="1048" height="559" alt="image" src="https://github.com/user-attachments/assets/ca1b1fa4-4f95-41b3-80bb-9ac149e82f94" />


