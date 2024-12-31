# 2. Mô tả kiến trúc

## 2.1. Mô hình phân rã thành phần
- Phân rã chi tiết các module trong từng phân hệ (Client/Server)
- Mô tả chức năng và trách nhiệm của từng module
- Biểu đồ package thể hiện cấu trúc tổ chức code

## 2.2. Mô hình đối tượng
### 2.2.1. Các đối tượng chính
- User/Account: Thông tin người dùng và tài khoản
- Department: Thông tin phòng ban/trung tâm
- Project: Thông tin dự án
- Milestone: Các mốc quan trọng của dự án
- Release: Các phiên bản release
- Issue: Các vấn đề/công việc trong dự án

### 2.2.2. Sơ đồ lớp
- Class diagram thể hiện cấu trúc các đối tượng
- Các thuộc tính và phương thức của từng lớp
- Mối quan hệ kế thừa, liên kết giữa các lớp

## 2.3. Mô hình quan hệ
### 2.3.1. Quan hệ thừa kế (Generalization)
- Phân cấp các đối tượng User (Admin, Manager, Member)
- Phân cấp các loại Issue (Task, Bug, Feature)

### 2.3.2. Quan hệ liên kết (Association)
- Mối quan hệ giữa User-Department
- Mối quan hệ giữa Project-Department
- Mối quan hệ giữa Issue-Project

### 2.3.3. Quan hệ hợp thành (Aggregation/Composition)
- Project chứa nhiều Milestone
- Project chứa nhiều Release
- Project chứa nhiều Issue

## 2.4. Đặc tả giao diện
### 2.4.1. API Interface
- REST API endpoints cho từng service
- Request/Response format
- Authentication/Authorization

### 2.4.2. Component Interface  
- React components interface
- Service layer interface
- Repository interface

## 2.5. Mô hình tương tác
### 2.5.1. Sequence Diagrams
- Luồng xử lý đăng nhập/xác thực
- Luồng tạo/cập nhật Project
- Luồng quản lý Issue
- Luồng phân quyền truy cập

### 2.5.2. Activity Diagrams
- Quy trình tạo dự án mới
- Quy trình quản lý issue
- Quy trình release

## 2.6. Đặc tả chi tiết các lớp
### 2.6.1. Domain Models
- Các thuộc tính
- Các phương thức
- Validation rules
- Business constraints

### 2.6.2. Service Layer
- Business logic
- Transaction management
- Integration points

### 2.6.3. Data Access Layer
- Repository interfaces
- Query methods
- Data mapping

Mỗi phần trên sẽ được chi tiết hóa bằng các biểu đồ UML tương ứng sử dụng PlantUML và các đặc tả chi tiết về thuộc tính, phương thức của từng lớp. 