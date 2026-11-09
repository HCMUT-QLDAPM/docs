# Project Context

**Project:** Student Dormitory Management System  
**Course:** CO3011 – Software Project Management  
**Document Version:** 0.1 (Draft)  
**Status:** Initial draft – Pending requirement clarification

## 1. Project Background

Ký túc xá sinh viên là một bộ phận quan trọng trong hệ thống dịch vụ hỗ trợ sinh viên tại các trường đại học. Hoạt động quản lý ký túc xá bao gồm đăng ký chỗ ở, phân bổ phòng, quản lý thông tin sinh viên, theo dõi tình trạng sử dụng phòng và tiếp nhận các yêu cầu phát sinh trong thời gian lưu trú.

Theo bản mô tả đề tài do giảng viên cung cấp, các hoạt động trên hiện được thực hiện thông qua nhiều công cụ khác nhau, gây khó khăn cho cả sinh viên và đơn vị quản lý.

Vì vậy, dự án **Student Dormitory Management System** được đề xuất nhằm xây dựng một hệ thống phần mềm tập trung, hỗ trợ quản lý thông tin và các quy trình nghiệp vụ chính của ký túc xá.

## 2. Organizational and Business Context

### 2.1. Organizational Context

Dự án được đặt trong bối cảnh một trường đại học có nhu cầu cải thiện hoạt động quản lý ký túc xá dành cho sinh viên.

Các nhóm đối tượng liên quan dự kiến bao gồm:

- **Sinh viên:** Người đăng ký và sử dụng dịch vụ ký túc xá.
- **Nhân viên quản lý:** Người thực hiện nghiệp vụ quản lý phòng, phân bổ chỗ ở và xử lý yêu cầu.
- **Đơn vị quản lý ký túc xá:** Bộ phận chịu trách nhiệm quản lý hoạt động lưu trú.
- **Nhóm phát triển:** Đơn vị phân tích, thiết kế và xây dựng phần mềm.

Vai trò và thẩm quyền cụ thể của từng đối tượng cần được xác nhận trong quá trình khảo sát yêu cầu.

### 2.2. Business Processes

Dựa trên mô tả ban đầu, các quy trình nghiệp vụ chính cần xem xét bao gồm:

1. Tiếp nhận đăng ký chỗ ở từ sinh viên.
2. Phân bổ phòng cho sinh viên.
3. Quản lý thông tin sinh viên lưu trú.
4. Theo dõi phòng và tình trạng sử dụng.
5. Tiếp nhận và xử lý yêu cầu liên quan đến phòng ở.

Quy trình chi tiết, thứ tự xử lý và các quy tắc nghiệp vụ chưa được xác định đầy đủ.

## 3. Current Problems

Từ bản mô tả đề tài, có thể xác định các vấn đề ban đầu:

### P1. Fragmented Management Tools

Các hoạt động quản lý đang được thực hiện thông qua nhiều công cụ khác nhau, thiếu một hệ thống tập trung.

### P2. Difficulties in Room Allocation

Việc phân bổ phòng và theo dõi tình trạng sử dụng phòng gặp khó khăn khi thông tin và quy trình quản lý bị phân tán.

### P3. Student Information Management

Thông tin sinh viên và quá trình lưu trú cần được quản lý thống nhất để hỗ trợ nhân viên thực hiện công việc.

### P4. Handling Student Requests

Việc tiếp nhận và giải quyết các yêu cầu liên quan đến phòng ở chưa được hỗ trợ bởi một quy trình phần mềm tập trung.

Các vấn đề trên được xác định từ đề bài ban đầu. Mức độ ảnh hưởng thực tế cần được kiểm chứng qua khảo sát.

## 4. Proposed Software Product

Dự án đề xuất phát triển một hệ thống quản lý ký túc xá tập trung, hỗ trợ hai nhóm người dùng chính:

**Student Portal**

- Đăng nhập hệ thống.
- Đăng ký chỗ ở ký túc xá.
- Theo dõi tình trạng đăng ký và thông tin phòng.
- Gửi và theo dõi các yêu cầu hỗ trợ.

**Management Portal**

- Quản lý thông tin phòng và tình trạng sử dụng.
- Xem và xử lý các đơn đăng ký.
- Phân bổ sinh viên vào phòng.
- Quản lý thông tin lưu trú.
- Tiếp nhận và xử lý yêu cầu của sinh viên.

Đây là các chức năng đề xuất ban đầu, **chưa phải phạm vi đã được khách hàng phê duyệt**.

## 5. Project Opportunities

Việc xây dựng hệ thống có thể tạo ra các cơ hội cải thiện sau:

- Tập trung hóa thông tin và nghiệp vụ quản lý ký túc xá.
- Giảm sự phụ thuộc vào nhiều công cụ riêng biệt.
- Hỗ trợ tra cứu tình trạng phòng và thông tin lưu trú.
- Cải thiện khả năng theo dõi và xử lý yêu cầu sinh viên.
- Tạo cơ sở để chuẩn hóa quy trình quản lý.

Những lợi ích này là kỳ vọng của dự án, chưa phải kết quả đã được đo lường.

## 6. Major Assumptions

Các giả định ban đầu cần kiểm chứng:

| ID | Assumption | Status |
|---|---|---|
| A01 | Hệ thống sẽ được triển khai dưới dạng ứng dụng web | Pending |
| A02 | Sinh viên và nhân viên quản lý sử dụng tài khoản riêng | Pending |
| A03 | Việc phân phòng do nhân viên quản lý thực hiện | Pending |
| A04 | Dữ liệu mẫu có thể được sử dụng để demo | Pending |
| A05 | Thanh toán trực tuyến không nằm trong phạm vi MVP | Pending |

Không xem các giả định này là yêu cầu chính thức cho đến khi được xác nhận phù hợp.

## 7. Project Constraints

### 7.1. Team and Resource Constraints

- Đề bài quy định nhóm gồm 4–5 sinh viên.
- Nhóm hiện có 3 thành viên và cần bổ sung nhân sự hoặc xin phép giảng viên.
- Các thành viên phải cân đối công việc dự án với lịch học và các hoạt động khác.

### 7.2. Schedule Constraints

- Dự án phải tuân theo các milestone của môn CO3011.
- Thời hạn chính thức được công bố trên LMS.
- Nhóm cần lập lịch dự án dựa trên thời gian khả dụng thực tế của các thành viên.

### 7.3. Technical Constraints

- Công nghệ phát triển chưa được thống nhất.
- Hệ thống cần hỗ trợ các luồng nghiệp vụ cốt lõi và có khả năng kiểm thử.
- Việc triển khai phải phù hợp với thời gian, kỹ năng và tài nguyên của nhóm.

### 7.4. Scope Constraints

- Ưu tiên các nghiệp vụ chính của hệ thống quản lý ký túc xá.
- Hạn chế bổ sung các chức năng phức tạp không cần thiết.
- Phạm vi chính thức cần được thống nhất trước khi thiết lập Project Baseline V1.0.

## 8. Open Questions

Các vấn đề chưa rõ cần tiếp tục tìm hiểu:

- Sinh viên có được lựa chọn phòng trực tiếp không?
- Quy trình phê duyệt đăng ký diễn ra như thế nào?
- Có những loại phòng và quy định phân bổ nào?
- Hệ thống có cần quản lý thanh toán không?
- Ai chịu trách nhiệm phê duyệt yêu cầu và nghiệm thu sản phẩm?
- Dữ liệu demo cần đáp ứng những điều kiện gì?

Các câu trả lời sẽ được cập nhật sau hoạt động Client Consultation và Requirement Discovery.

## 9. References

- CO3011 – Project Assignment 2026–2027.
- Email giao đề tài *Student Dormitory Management System* của giảng viên Nguyễn Minh Tâm.
- Client Interaction Log (sẽ bổ sung khi thực hiện khảo sát).