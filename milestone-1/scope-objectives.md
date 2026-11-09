# Project Scope, Objectives & Measures of Effectiveness

**Project:** Student Dormitory Management System  
**Course:** CO3011 – Software Project Management  
**Document Version:** 0.1 (Draft)  
**Status:** Proposed Scope – Pending Client Confirmation

---

## 1. Purpose

Tài liệu này xác định phạm vi, mục tiêu, kết quả mong đợi và các tiêu chí đo lường hiệu quả của dự án Student Dormitory Management System.

Mục đích chính:

- Xác định những nghiệp vụ mà hệ thống dự kiến hỗ trợ.
- Phân biệt các chức năng thuộc và không thuộc phạm vi dự án.
- Thiết lập các mục tiêu có thể đo lường.
- Cung cấp cơ sở cho hoạt động lập kế hoạch, ước lượng và kiểm thử.
- Hạn chế việc mở rộng phạm vi không được kiểm soát (Scope Creep).

Đây là bản đề xuất ban đầu, được xây dựng từ mô tả đề tài của giảng viên và phân tích sơ bộ của nhóm.

## 2. Project Scope Statement

Dự án hướng đến việc phát triển một ứng dụng web quản lý ký túc xá dành cho sinh viên và nhân viên quản lý.

Hệ thống dự kiến hỗ trợ quy trình đăng ký chỗ ở, xét duyệt đăng ký, phân bổ phòng, quản lý thông tin lưu trú và xử lý các yêu cầu liên quan đến phòng ở.

Phạm vi phần mềm được giới hạn ở các nghiệp vụ cốt lõi nhằm tạo ra một sản phẩm có thể vận hành và trình diễn các quy trình hoàn chỉnh từ đầu đến cuối.

Sản phẩm được phát triển trong khuôn khổ bài tập lớn CO3011 và chưa đặt mục tiêu thay thế toàn bộ hệ thống quản lý ký túc xá thực tế của một trường đại học.

## 3. In-Scope Functional Requirements

Các chức năng dưới đây là phạm vi MVP được nhóm đề xuất, chưa phải yêu cầu đã được khách hàng phê duyệt.

### 3.1. User Authentication & Authorization

**FR01 – Quản lý truy cập hệ thống**

- Người dùng đăng nhập bằng tài khoản được cấp.
- Hệ thống phân biệt hai vai trò chính: Student và Dormitory Staff/Admin.
- Người dùng chỉ có thể thực hiện các thao tác phù hợp với quyền của mình.
- Người dùng có thể đăng xuất.

### 3.2. Dormitory Room Management

**FR02 – Quản lý thông tin phòng**

Nhân viên quản lý có thể:

- Xem danh sách phòng.
- Thêm và cập nhật thông tin phòng.
- Xem sức chứa tối đa của từng phòng.
- Theo dõi số lượng sinh viên đang được phân bổ.
- Xem tình trạng còn chỗ hoặc đã đủ chỗ.

Hệ thống cần kiểm soát việc phân bổ không vượt quá sức chứa quy định.

### 3.3. Dormitory Registration

**FR03 – Đăng ký chỗ ở**

Sinh viên có thể:

- Truy cập biểu mẫu đăng ký.
- Gửi yêu cầu đăng ký chỗ ở.
- Theo dõi trạng thái xử lý đơn.
- Xem kết quả đăng ký.

Các trạng thái đề xuất:

- Pending – Chờ xét duyệt.
- Approved – Đã duyệt.
- Rejected – Bị từ chối.

Quy tắc về việc sinh viên tự chọn phòng hoặc được nhân viên phân phòng cần được xác nhận thêm.

### 3.4. Application Review & Room Allocation

**FR04 – Xét duyệt và phân bổ phòng**

Nhân viên quản lý có thể:

- Xem danh sách đơn đăng ký.
- Xem thông tin của từng đơn.
- Phê duyệt hoặc từ chối đơn.
- Phân bổ sinh viên vào phòng còn sức chứa.
- Xem kết quả phân bổ.

Hệ thống dự kiến thực hiện kiểm tra dữ liệu để tránh phân phòng vượt sức chứa hoặc phân bổ trùng một sinh viên vào nhiều phòng tại cùng một thời điểm.

Quy trình xét duyệt và phân phòng chi tiết sẽ được làm rõ thông qua Requirement Discovery.

### 3.5. Student Residence Information

**FR05 – Tra cứu thông tin lưu trú**

Sinh viên có thể:

- Xem thông tin phòng được phân bổ.
- Xem trạng thái lưu trú hiện tại.

Nhân viên có thể:

- Xem danh sách sinh viên được phân bổ vào từng phòng.
- Tra cứu thông tin lưu trú của sinh viên.

### 3.6. Student Support Request Management

**FR06 – Quản lý yêu cầu hỗ trợ**

Sinh viên có thể:

- Tạo yêu cầu hỗ trợ liên quan đến phòng ở.
- Nhập nội dung và mô tả vấn đề.
- Theo dõi tình trạng xử lý yêu cầu.

Nhân viên có thể:

- Xem các yêu cầu được gửi đến.
- Cập nhật trạng thái xử lý.
- Ghi nhận kết quả xử lý.

Trạng thái đề xuất:

- Pending – Chờ tiếp nhận.
- In Progress – Đang xử lý.
- Resolved – Đã giải quyết.

## 4. Out-of-Scope Features

Để giới hạn độ phức tạp và tập trung vào các nghiệp vụ chính, nhóm đề xuất loại trừ những chức năng sau khỏi MVP.

| ID | Chức năng không thực hiện | Lý do |
|---|---|---|
| EX01 | Thanh toán trực tuyến | Tăng độ phức tạp, yêu cầu tích hợp dịch vụ bên ngoài |
| EX02 | Ứng dụng di động riêng | Ứng dụng web đáp ứng phạm vi đề xuất ban đầu |
| EX03 | Tích hợp hệ thống quản lý sinh viên của trường | Chưa có yêu cầu hoặc khả năng truy cập hệ thống bên ngoài |
| EX04 | Phân phòng tự động bằng thuật toán tối ưu | Chưa cần thiết cho quy trình MVP |
| EX05 | Thông báo thời gian thực | Có thể mở rộng sau |
| EX06 | Quản lý điện, nước và hóa đơn | Không thuộc các nghiệp vụ ưu tiên được đề xuất |
| EX07 | Quản lý nhiều cơ sở KTX với các quy trình khác nhau | Vượt khỏi phạm vi MVP dự kiến |

Các mục loại trừ cần được xác nhận với client trước khi chốt phạm vi chính thức.

## 5. Project Objectives

Mục tiêu dự án được xác định dựa trên kết quả sử dụng hệ thống, thay vì chỉ liệt kê các module phần mềm cần hoàn thành.

### O1 – Improve Registration Accessibility

Cải thiện khả năng thực hiện và theo dõi quy trình đăng ký chỗ ở thông qua một hệ thống tập trung.

**Kết quả mong đợi:**

Sinh viên có thể hoàn thành quy trình gửi đăng ký và xem trạng thái xử lý mà không phải sử dụng nhiều công cụ riêng biệt trong kịch bản thử nghiệm.

### O2 – Improve Room Allocation Accuracy

Nâng cao tính nhất quán và chính xác của quá trình phân bổ phòng.

**Kết quả mong đợi:**

Nhân viên có thể phân bổ chỗ ở dựa trên thông tin sức chứa được cập nhật, đồng thời hệ thống ngăn các thao tác phân bổ không hợp lệ.

### O3 – Improve Support Request Tracking

Cải thiện khả năng tiếp nhận, theo dõi và xử lý các yêu cầu liên quan đến phòng ở.

**Kết quả mong đợi:**

Sinh viên và nhân viên có thể theo dõi tiến trình xử lý yêu cầu trên cùng một hệ thống.

### O4 – Improve Information Consistency

Hỗ trợ quản lý thông tin sinh viên và phòng ở một cách thống nhất.

**Kết quả mong đợi:**

Thông tin đăng ký, phân phòng và lưu trú có thể được tra cứu nhất quán giữa các vai trò người dùng được cấp quyền.

## 6. Measures of Effectiveness

Nhóm đề xuất các chỉ số đo lường sau để đánh giá mức độ đạt được mục tiêu dự án.

Các giá trị mục tiêu hiện là **proposed targets**, chưa được client xác nhận và có thể cần điều chỉnh theo điều kiện thử nghiệm thực tế.

| Objective | Measure of Effectiveness | Proposed Target |
|---|---|---|
| O1 | Tỷ lệ người dùng thử hoàn thành đăng ký và tra cứu trạng thái mà không cần hỗ trợ | ≥ 80% |
| O2 | Tỷ lệ kịch bản kiểm thử phân phòng tuân thủ giới hạn sức chứa và quy tắc không phân trùng | 100% |
| O3 | Tỷ lệ yêu cầu hỗ trợ thử nghiệm có thể theo dõi được trạng thái và kết quả xử lý | 100% |
| O4 | Tỷ lệ trường hợp kiểm thử cho kết quả thông tin lưu trú nhất quán giữa các giao diện | 100% |

### Measurement Methods

**M1 – Registration Usability Test**

Cho một nhóm người dùng thử thực hiện quy trình đăng ký và theo dõi trạng thái bằng dữ liệu thử nghiệm.

Ghi nhận số lượng người dùng hoàn thành mà không cần trợ giúp.

**M2 – Room Allocation Validation Test**

Kiểm thử các trường hợp phòng còn chỗ, phòng đã đầy, phân bổ trùng và các dữ liệu không hợp lệ.

Ghi nhận tỷ lệ kiểm thử thành công.

**M3 – Support Request Tracking Test**

Tạo các yêu cầu hỗ trợ thử nghiệm và kiểm tra khả năng theo dõi trạng thái từ lúc gửi đến lúc hoàn thành.

**M4 – Data Consistency Test**

Đối chiếu thông tin đăng ký, phân phòng và lưu trú được hiển thị cho các vai trò khác nhau.

### Measurement Limitations

Do dự án mang tính học thuật, phần lớn kết quả sẽ được đo thông qua môi trường demo hoặc thử nghiệm.

Các chỉ số trên có thể chứng minh tính hiệu quả trong phạm vi thử nghiệm, nhưng chưa đủ để khẳng định hiệu quả khi triển khai thực tế ở quy mô lớn.

Nếu thu thập được dữ liệu quy trình hiện tại, nhóm có thể bổ sung các phép đo trước và sau khi áp dụng giải pháp.

## 7. Expected Project Outcomes

Sau khi hoàn thành, dự án kỳ vọng đạt được:

1. Một quy trình đăng ký và xét duyệt chỗ ở có thể vận hành từ đầu đến cuối.
2. Khả năng quản lý và kiểm tra tình trạng phân bổ phòng.
3. Khả năng theo dõi thông tin lưu trú trên hệ thống tập trung.
4. Một quy trình tiếp nhận và xử lý yêu cầu hỗ trợ có thể kiểm chứng.
5. Bằng chứng thử nghiệm để đánh giá mức độ đạt được các mục tiêu O1–O4.

Các kết quả này là kỳ vọng của dự án. Mức độ hoàn thành sẽ được đánh giá trong giai đoạn Final Review.

## 8. Major Project Deliverables

Các sản phẩm bàn giao chính dự kiến bao gồm:

| ID | Deliverable | Description |
|---|---|---|
| P01 | Requirements & Scope Documentation | Tài liệu xác định yêu cầu và phạm vi |
| P02 | Project Management Plan | Kế hoạch, ước lượng, lịch trình và nguồn lực |
| P03 | Student Portal | Giao diện và chức năng dành cho sinh viên |
| P04 | Management Portal | Giao diện và chức năng dành cho nhân viên |
| P05 | Backend & Database | API, quy tắc nghiệp vụ và lưu trữ dữ liệu |
| P06 | Testing Evidence | Test cases, kết quả kiểm thử và bằng chứng chất lượng |
| P07 | Final Report & Demonstration | Báo cáo tổng kết và demo sản phẩm |

Danh sách này là cơ sở tham khảo cho PBS trong Task 2.1, chưa phải PBS hoàn chỉnh.

## 9. Scope Constraints and Dependencies

### 9.1. Constraints

- Nhóm cần tuân thủ quy định 4–5 thành viên hoặc có sự chấp thuận ngoại lệ của giảng viên.
- Thời hạn dự án và milestone thực hiện theo thông báo trên LMS.
- Nguồn lực phát triển phụ thuộc vào lịch học và thời gian khả dụng của thành viên.
- Phần mềm phải được triển khai và kiểm thử trong phạm vi thời gian dự án.
- Phạm vi nên ưu tiên các nghiệp vụ cốt lõi thay vì những chức năng phức tạp không cần thiết.

### 9.2. Dependencies

- Quy trình phân phòng phụ thuộc vào các quy tắc nghiệp vụ được xác nhận.
- Ước lượng công sức phụ thuộc vào phạm vi chức năng và năng lực của nhóm.
- Kế hoạch triển khai phụ thuộc vào nguồn lực và lịch thực tế.
- Tiêu chí nghiệm thu phụ thuộc vào thỏa thuận với client/người có thẩm quyền.
- Việc chốt Baseline V1.0 phụ thuộc vào quá trình rà soát và thống nhất kế hoạch.

## 10. Scope Assumptions

| ID | Assumption | Status |
|---|---|---|
| A01 | Hệ thống được triển khai dưới dạng web application | Pending |
| A02 | Hai vai trò sử dụng chính là Student và Staff/Admin | Pending |
| A03 | Nhân viên thực hiện phân phòng thủ công thông qua hệ thống | Pending |
| A04 | Dự án sử dụng dữ liệu thử nghiệm phục vụ demo | Pending |
| A05 | Thanh toán trực tuyến không thuộc MVP | Pending |
| A06 | Phiên bản đầu tiên phục vụ một mô hình quản lý KTX thống nhất | Pending |

Các giả định cần được cập nhật khi có kết quả khảo sát hoặc phản hồi của client.

## 11. Initial Requirements Traceability

Bảng này thể hiện mối liên hệ ban đầu giữa mục tiêu và yêu cầu chức năng.

| Objective | Related Requirements | Verification |
|---|---|---|
| O1 | FR01, FR03 | M1 |
| O2 | FR02, FR04 | M2 |
| O3 | FR06 | M3 |
| O4 | FR03, FR04, FR05 | M4 |

Bảng sẽ được mở rộng ở những milestone tiếp theo nhằm liên kết mục tiêu, sản phẩm, hoạt động, nguồn lực, rủi ro, kiểm thử và checkpoint.

## 12. Scope Review and Approval

### Current Status

**Draft V0.1 – Not Approved**

Các bước tiếp theo:

1. Rà soát nội bộ các chức năng và mục tiêu đề xuất.
2. Khảo sát người dùng và làm rõ các yêu cầu chưa chắc chắn.
3. Xác định người có thẩm quyền phê duyệt phạm vi.
4. Điều chỉnh phạm vi và các chỉ số đo lường theo phản hồi thực tế.
5. Lưu phiên bản được thống nhất để phục vụ Project Baseline V1.0.

Các thay đổi phạm vi sau khi thiết lập baseline cần được phân tích, ghi nhận và xử lý theo quy trình quản lý thay đổi của dự án.

## 13. References

- CO3011 – Software Project Management, Project Assignment 2026–2027.
- Email giao đề tài Student Dormitory Management System.
- `project-context.md` – Draft V0.1.
- `business-case.md` – Draft V0.1.
- Client Interaction Log – Pending.