# Business Case – Student Dormitory Management System

**Course:** CO3011 – Software Project Management  
**Project:** Student Dormitory Management System  
**Document Version:** 0.1 (Draft)  
**Status:** Preliminary Evaluation – Pending Client Consultation

---

## 1. Executive Summary

Dự án **Student Dormitory Management System** được đề xuất nhằm giải quyết những khó khăn trong quá trình quản lý ký túc xá sinh viên tại một trường đại học.

Theo bản mô tả đề tài ban đầu, các hoạt động như đăng ký chỗ ở, phân bổ phòng, quản lý thông tin sinh viên và xử lý yêu cầu liên quan đến phòng ở đang được thực hiện thông qua nhiều công cụ khác nhau. Điều này gây khó khăn trong việc quản lý thông tin và phối hợp giữa sinh viên với đơn vị quản lý ký túc xá.

Dự án hướng đến việc phát triển một hệ thống phần mềm tập trung, hỗ trợ các quy trình nghiệp vụ chính và tạo điều kiện cải thiện hiệu quả quản lý.

Trong phạm vi môn CO3011, dự án được xem xét như một sản phẩm phần mềm quy mô nhỏ, với ưu tiên là tính khả thi, khả năng hoàn thành và hiệu quả quản lý dự án.

**Đề xuất sơ bộ:** GO có điều kiện, với phạm vi MVP phù hợp và các yêu cầu quan trọng được xác nhận trước khi chốt kế hoạch.

## 2. Business Need and Problem Statement

### 2.1. Business Need

Đơn vị quản lý ký túc xá cần một giải pháp hỗ trợ quản lý thông tin phòng ở, sinh viên và các yêu cầu phát sinh thông qua một hệ thống tập trung.

Hệ thống được kỳ vọng giúp đơn vị quản lý có thể theo dõi các hoạt động liên quan đến ký túc xá một cách nhất quán và thuận tiện hơn.

### 2.2. Existing Problems

| ID | Vấn đề | Ảnh hưởng tiềm năng |
|---|---|---|
| BP01 | Công cụ quản lý phân tán | Khó tổng hợp và theo dõi thông tin |
| BP02 | Quy trình đăng ký chỗ ở chưa tập trung | Sinh viên và nhân viên gặp khó khăn trong quá trình xử lý |
| BP03 | Khó theo dõi tình trạng sử dụng phòng | Việc phân bổ và quản lý phòng có thể kém hiệu quả |
| BP04 | Thông tin sinh viên được quản lý qua nhiều công cụ | Tăng khó khăn trong cập nhật và tra cứu |
| BP05 | Yêu cầu hỗ trợ liên quan đến phòng ở chưa được tập trung hóa | Khó theo dõi tiến độ xử lý |

Các vấn đề được xác định từ bản mô tả của giảng viên. Mức độ nghiêm trọng và tần suất phát sinh chưa được kiểm chứng bằng dữ liệu thực tế.

## 3. Proposed Solution

Nhóm đề xuất xây dựng một ứng dụng web quản lý ký túc xá, cung cấp các chức năng cốt lõi phục vụ sinh viên và nhân viên quản lý.

### 3.1. Student Functions

- Đăng nhập hệ thống.
- Đăng ký chỗ ở ký túc xá.
- Theo dõi trạng thái đơn đăng ký.
- Tra cứu thông tin phòng ở.
- Gửi và theo dõi yêu cầu hỗ trợ.

### 3.2. Management Functions

- Quản lý danh sách phòng và sức chứa.
- Xem và xử lý đơn đăng ký.
- Phân bổ sinh viên vào phòng.
- Quản lý thông tin lưu trú.
- Tiếp nhận và cập nhật trạng thái yêu cầu hỗ trợ.

Các chức năng trên là đề xuất cho MVP, chưa phải phạm vi chính thức được khách hàng phê duyệt.

Phạm vi chi tiết, quy tắc nghiệp vụ và tiêu chí nghiệm thu sẽ được xác định trong tài liệu `scope-objectives.md`.

## 4. Expected Benefits

### 4.1. Tangible Benefits – Lợi ích có thể đo lường

| ID | Lợi ích kỳ vọng | Phương pháp đánh giá đề xuất |
|---|---|---|
| B01 | Giảm thời gian xử lý đơn đăng ký | So sánh thời gian xử lý theo quy trình hiện tại và quy trình thử nghiệm |
| B02 | Giảm thao tác tra cứu thông tin phòng | Đo thời gian hoàn thành tác vụ tra cứu |
| B03 | Cải thiện khả năng theo dõi tình trạng phòng | Kiểm tra mức độ đầy đủ, chính xác và cập nhật của dữ liệu |
| B04 | Cải thiện khả năng theo dõi yêu cầu hỗ trợ | Đo tỷ lệ yêu cầu có trạng thái và lịch sử xử lý rõ ràng |

Đây là các lợi ích kỳ vọng. Nhóm chưa có dữ liệu khảo sát để khẳng định mức cải thiện cụ thể.

### 4.2. Intangible Benefits – Lợi ích phi định lượng

- Nâng cao sự thuận tiện cho sinh viên khi sử dụng dịch vụ ký túc xá.
- Cải thiện tính minh bạch của quá trình đăng ký và xử lý yêu cầu.
- Hỗ trợ nhân viên thực hiện nghiệp vụ trên một hệ thống thống nhất.
- Tạo cơ sở cho việc chuẩn hóa và mở rộng quy trình quản lý trong tương lai.

## 5. Potential Disbenefits

Bên cạnh những lợi ích dự kiến, việc triển khai hệ thống có thể phát sinh các bất lợi sau:

| ID | Disbenefit | Ảnh hưởng |
|---|---|---|
| D01 | Người dùng cần thời gian làm quen | Có thể giảm hiệu suất trong giai đoạn đầu |
| D02 | Phụ thuộc vào hệ thống phần mềm | Sự cố kỹ thuật có thể làm gián đoạn công việc |
| D03 | Phát sinh nhu cầu quản trị và bảo trì | Tăng khối lượng công việc vận hành |
| D04 | Rủi ro bảo mật thông tin sinh viên | Có thể ảnh hưởng đến quyền riêng tư và độ tin cậy |
| D05 | Chuyển đổi dữ liệu từ công cụ hiện tại | Có thể phát sinh sai sót và chi phí chuyển đổi |

Những bất lợi này cần được xem xét khi xác định yêu cầu bảo mật, thiết kế quy trình và xây dựng kế hoạch triển khai.

## 6. Alternative Solutions

Nhóm xem xét ba phương án ban đầu.

### Option A – Maintain Current Process

Tiếp tục sử dụng các công cụ và phương thức quản lý hiện tại.

**Ưu điểm:**
- Không cần đầu tư phát triển phần mềm mới.
- Không phát sinh nhu cầu đào tạo sử dụng hệ thống mới.

**Nhược điểm:**
- Không giải quyết triệt để tình trạng công cụ phân tán.
- Khó chuẩn hóa và tích hợp các quy trình nghiệp vụ.

### Option B – Improve Existing Tools

Cải tiến cách sử dụng các công cụ hiện tại, ví dụ chuẩn hóa biểu mẫu, dữ liệu và quy trình phối hợp.

**Ưu điểm:**
- Chi phí triển khai ban đầu có thể thấp.
- Ít thay đổi đối với người dùng.

**Nhược điểm:**
- Khả năng tích hợp các quy trình có thể bị hạn chế.
- Vẫn phụ thuộc vào khả năng của các công cụ riêng lẻ.

### Option C – Develop a Centralized Web Application

Xây dựng ứng dụng web tích hợp các nghiệp vụ quản lý ký túc xá cốt lõi.

**Ưu điểm:**
- Hỗ trợ quản lý tập trung.
- Có thể thiết kế theo quy trình nghiệp vụ đã thống nhất.
- Tạo nền tảng cho việc mở rộng về sau.

**Nhược điểm:**
- Cần thời gian và nhân lực phát triển.
- Có rủi ro về tiến độ, chất lượng và bảo trì.
- Cần làm rõ yêu cầu trước khi triển khai.

### Preliminary Options Evaluation

| Tiêu chí | Option A | Option B | Option C |
|---|---|---|---|
| Chi phí ban đầu | Thấp | Thấp đến trung bình | Phụ thuộc phạm vi |
| Mức thay đổi quy trình | Thấp | Trung bình | Cao hơn |
| Khả năng tích hợp nghiệp vụ | Hạn chế | Phụ thuộc công cụ | Có thể thiết kế tập trung |
| Khả năng đáp ứng mục tiêu học phần | Không đáp ứng yêu cầu phát triển sản phẩm mới | Phụ thuộc mức phát triển phần mềm | Phù hợp với đề tài được giao |

**Phương án đề xuất:** Option C, triển khai dưới dạng MVP.

Đây là lựa chọn sơ bộ xét theo mục tiêu bài tập lớn và nhu cầu của hệ thống. Chưa đủ thông tin để kết luận Option C có hiệu quả kinh tế cao nhất nếu triển khai thực tế.

## 7. Cost Analysis

### 7.1. Development Costs

Các nhóm chi phí dự kiến:

| Cost Category | Nội dung | Phương pháp ước lượng |
|---|---|---|
| Human Resources | Phân tích, thiết kế, lập trình, kiểm thử, quản lý | Effort × đơn giá quy đổi |
| Infrastructure | Hosting, database, các dịch vụ triển khai | Theo gói dịch vụ và thời gian sử dụng |
| Development Tools | Công cụ quản lý và phát triển | Theo công cụ thực tế |
| Quality Assurance | Kiểm thử và sửa lỗi | Ước lượng giờ-người |
| Contingency | Dự phòng rủi ro | Theo các rủi ro được đánh giá |

### 7.2. Cost Estimation Method

Chi phí công sức phát triển có thể được đánh giá bằng công thức:

**Labor Cost = Tổng (Estimated Effort của từng hoạt động × Hourly Rate tương ứng)**

**Total Estimated Cost = Labor Cost + Infrastructure Cost + Tool Cost + Other Costs + Contingency**

Trong đó:

- *Estimated Effort* được xây dựng bằng phương pháp bottom-up ở Task 2.6.
- *Hourly Rate* là đơn giá giả định nhằm phục vụ đánh giá chi phí, không đồng nghĩa với khoản tiền thực tế chi trả.
- Chi phí dịch vụ được cập nhật dựa trên phương án triển khai đã chọn.
- Phần dự phòng được xác định theo kết quả phân tích rủi ro.

Tại thời điểm lập bản nháp, nhóm chưa có đủ dữ liệu để xác định tổng chi phí dự án đáng tin cậy.

### 7.3. Financial Evaluation

Các phương pháp như ROI, Payback Period hoặc NPV có thể được xem xét khi có dữ liệu đáng tin cậy về chi phí và lợi ích tài chính.

Tuy nhiên, dự án hiện là sản phẩm học thuật quy mô nhỏ. Chưa có dữ liệu về khối lượng nghiệp vụ, thời gian xử lý hiện tại, chi phí vận hành hay giá trị tiết kiệm dự kiến của đơn vị quản lý ký túc xá.

Vì vậy, **chưa thể tính ROI, NPV hoặc thời gian hoàn vốn có ý nghĩa thực tế**.

Ở giai đoạn này, nhóm sử dụng đánh giá chi phí sơ bộ kết hợp với phân tích tính khả thi, lợi ích và rủi ro. Đánh giá tài chính sẽ được bổ sung nếu thu thập được dữ liệu phù hợp.

## 8. Strategic and Organizational Contribution

Dự án có tiềm năng đóng góp cho hoạt động quản lý ký túc xá thông qua:

1. **Digitalization:** Hỗ trợ số hóa các nghiệp vụ quản lý.
2. **Process Standardization:** Tạo cơ sở chuẩn hóa quy trình đăng ký, phân phòng và xử lý yêu cầu.
3. **Information Accessibility:** Cải thiện khả năng truy cập và cập nhật thông tin của các bên liên quan.
4. **Service Quality:** Tạo điều kiện nâng cao trải nghiệm sử dụng dịch vụ ký túc xá.
5. **Future Development:** Hình thành nền tảng có thể được nghiên cứu mở rộng nếu được triển khai thực tế.

Những đóng góp này là mục tiêu kỳ vọng, chưa phải kết quả vận hành đã được chứng minh.

## 9. Preliminary Feasibility Assessment

| Dimension | Đánh giá sơ bộ | Điều kiện cần xem xét |
|---|---|---|
| Technical | Có khả năng thực hiện với phạm vi MVP | Xác nhận công nghệ và năng lực nhóm |
| Schedule | Có thể lập kế hoạch rút gọn | Cần đối chiếu deadline LMS và effort thực tế |
| Resource | Chưa đáp ứng đầy đủ quy mô nhóm theo đề | Bổ sung thành viên hoặc được thầy chấp thuận |
| Operational | Có tiềm năng hỗ trợ nghiệp vụ KTX | Cần khảo sát và xác nhận quy trình |
| Financial | Chưa đủ dữ liệu định lượng | Hoàn thiện cost estimates |

## 10. Go/No-Go Recommendation

### 10.1. Proposed Decision

**Recommendation: CONDITIONAL GO**

Nhóm đề xuất tiếp tục thực hiện dự án Student Dormitory Management System dưới hình thức phát triển MVP.

### 10.2. Justification

- Dự án xuất phát từ vấn đề được nêu trong bản mô tả của giảng viên.
- Giải pháp phần mềm tập trung có tiềm năng cải thiện quy trình quản lý ký túc xá.
- Phạm vi MVP có thể được giới hạn để phù hợp với nguồn lực của nhóm.
- Việc thực hiện dự án tạo điều kiện áp dụng các phương pháp quản lý dự án phần mềm theo yêu cầu CO3011.

### 10.3. Conditions for Proceeding

Để chuyển từ đề xuất sơ bộ sang quyết định triển khai chính thức, cần:

1. Xác nhận các yêu cầu nghiệp vụ và phạm vi cốt lõi với client phù hợp.
2. Làm rõ thẩm quyền phê duyệt và tiêu chí nghiệm thu.
3. Đáp ứng yêu cầu về quy mô nhóm hoặc được giảng viên chấp thuận ngoại lệ.
4. Hoàn thành ước lượng công sức và đánh giá nguồn lực theo lịch thực tế.
5. Xác nhận rằng phạm vi MVP có thể hoàn thành trong thời gian dự án.

Nếu những điều kiện quan trọng không được đáp ứng, nhóm cần điều chỉnh phạm vi hoặc xem xét lại quyết định GO.

## 11. Pending Information

Các thông tin cần được bổ sung hoặc xác nhận:

- Quy trình quản lý ký túc xá hiện tại.
- Các khó khăn cụ thể từ sinh viên và nhân viên quản lý.
- Quy tắc đăng ký và phân bổ phòng.
- Tiêu chí nghiệm thu của khách hàng.
- Số lượng và khả năng tham gia của thành viên.
- Mốc thời gian dự án chính thức.
- Dữ liệu về chi phí và lợi ích, nếu có.

## 12. References

- CO3011 – Software Project Management, Project Assignment 2026–2027.
- Email giao đề tài *Student Dormitory Management System* của giảng viên Nguyễn Minh Tâm.
- `project-context.md` – Draft V0.1.
- Client Interaction Log – Pending.
- Project Estimation Documents – To be developed in Milestone 2.