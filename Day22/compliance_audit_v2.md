# BÁO CÁO TUÂN THỦ PHÁP LÝ 

## I. DANH SÁCH VI PHẠM PHÁP LÝ TIỀM NĂNG

### VI PHẠM 1: Quảng cáo thổi phồng công năng nhận diện

* **Luật áp dụng:** Bộ luật Hình sự 2015 (sửa đổi 2017)
* **Điều:** Điều 198 (Tội lừa dối khách hàng) - Hành vi quảng cáo sai sự thật về chất lượng hàng hóa, dịch vụ.
* **Bằng chứng trong sản phẩm:** "AI nhận diện chính xác 100% mọi món ăn Việt Nam."
* **Pattern khớp với:** Vụ Kera 
* **Hành động sửa:** Sửa thành "AI hỗ trợ nhận diện các món ăn phổ biến trong cơ sở dữ liệu."
* **Deadline:** 12/05/2026 (Trước khi Launch chiến dịch Marketing tiếp theo).

### VI PHẠM 2: Sử dụng thuật ngữ gây hiểu lầm là cơ sở khám chữa bệnh

* **Luật áp dụng:** Luật AI Việt Nam 134/2025/QH15
* **Điều:** Điều 15 (Minh bạch thông tin hệ thống AI) - Không được gây nhầm lẫn AI với tư vấn chuyên gia y tế.
* **Bằng chứng trong sản phẩm:** "Giải pháp thay thế hoàn toàn bác sĩ dinh dưỡng."
* **Pattern khớp với:** Vụ Kera 
* **Hành động sửa:** Xóa bỏ cụm "thay thế hoàn toàn", bổ sung disclaimer: "Sản phẩm không thay thế chẩn đoán y khoa."
* **Deadline:** 12/05/2026.

### VI PHẠM 3: Cam kết kết quả sức khỏe không có bằng chứng

* **Luật áp dụng:** Luật AI Việt Nam 134/2025/QH15
* **Điều:** Điều 42 (Hành vi bị cấm) - Thổi phồng năng lực AI để trục lợi.
* **Bằng chứng trong sản phẩm:** "Dự báo chính xác 95% biến động đường huyết sau ăn."
* **Pattern khớp với:** Vụ Kera 
* **Hành động sửa:** Chuyển sang mô tả xu hướng: "Cung cấp dự báo xu hướng dựa trên lịch sử dữ liệu người dùng."
* **Deadline:** 12/05/2026.

### VI PHẠM 4: Chuyển dữ liệu sức khỏe ra nước ngoài trái quy định

* **Luật áp dụng:** Luật BVDLCN 91/2025/QH15 (PDPL)
* **Điều:** Điều 30 (Xử lý dữ liệu cá nhân nhạy cảm) và Điều 31 (Chuyển dữ liệu ra nước ngoài).
* **Bằng chứng trong sản phẩm:** Gửi dữ liệu cá nhân trực tiếp qua API OpenAI/Gemini (server ngoại) mà chưa lập hồ sơ CTIA.
* **Pattern khớp với:** Vụ rò rỉ CIC 
* **Hành động sửa:** Thiết lập lớp Anonymization để ẩn danh hóa dữ liệu định danh trước khi gửi API.
* **Deadline:** 22/05/2026 (Theo thời hạn nộp hồ sơ A05).

### VI PHẠM 5: Thiếu quy trình Consent cho dữ liệu nhạy cảm

* **Luật áp dụng:** Luật BVDLCN 91/2025/QH15 (PDPL)
* **Điều:** Điều 8 (Quyền của chủ thể dữ liệu) và Điều 11 (Sự đồng ý).
* **Bằng chứng trong sản phẩm:** Gộp chung sự đồng ý xử lý dữ liệu định danh (Tên, SĐT) và dữ liệu sức khỏe (đường huyết) vào 1 nút "Đồng ý" duy nhất.
* **Pattern khớp với:** Vụ rò rỉ CIC
* **Hành động sửa:** Tách riêng nút đồng ý (Checkbox) cho việc xử lý dữ liệu sức khỏe nhạy cảm.
* **Deadline:** 01/06/2026.

### VI PHẠM 6: Sai lệch phân loại rủi ro hệ thống AI

* **Luật áp dụng:** Luật AI Việt Nam 134/2025/QH15
* **Điều:** Điều 9 (Phân loại hệ thống AI rủi ro cao).
* **Bằng chứng trong sản phẩm:** Tự phân loại là rủi ro "Trung bình" trong hồ sơ nội bộ, mặc dù can thiệp trực tiếp vào dinh dưỡng bệnh nhân.
* **Pattern khớp với:** Đối chiếu theo danh mục của Điều 9: Hệ thống AI hỗ trợ ra quyết định trong Y tế là **Rủi ro cao**.
* **Hành động sửa:** Cập nhật lại hồ sơ rà soát nội bộ và chuẩn bị bộ dữ liệu kiểm soát (Auditable logs).
* **Deadline:** 15/06/2026.

### VI PHẠM 7: Rủi ro nguồn tiền và kiểm soát dòng tiền Vendor

* **Luật áp dụng:** Bộ luật Hình sự 2015 - Điều 324 (Tội rửa tiền)
* **Điều:** Điều 324 (Hành vi không kiểm soát nguồn gốc tiền trong giao dịch công nghệ).
* **Bằng chứng trong sản phẩm:** Sử dụng cổng thanh toán bên thứ ba chưa được cấp phép hoặc thiếu cơ chế KYC cho Caregiver khi nạp số tiền lớn.
* **Pattern khớp với:** Vụ Mr Pips 
* **Hành động sửa:** Tích hợp SDK của các cổng thanh toán chính quy (Napvas/Momo) và lưu vết giao dịch.
* **Deadline:** 22/05/2026.

---

## II. ƯU TIÊN TOP 5 HÀNH ĐỘNG KHẨN CẤP

| Thứ tự | Vi phạm nghiêm trọng nhất | 3 Hành động sửa cụ thể |
| --- | --- | --- |
| **1** | **Marketing thổi phồng (Kera)** | 1. Rà soát lại toàn bộ Content Marketing trên tất cả nền tảng.2. Thay các từ khẳng định tuyệt đối bằng từ hỗ trợ. 3. Founder ký biên bản phê duyệt nội dung "Honest Version". |
| **2** | **Chuyển dữ liệu ngoại (PDPL)** | 1. Xây dựng Data Gateway để ẩn danh hóa dữ liệu. 2. Soạn thảo Hồ sơ CTIA gửi Cục An ninh mạng. 3. Chỉ gửi dữ liệu tối thiểu cần thiết cho AI xử lý. |
| **3** | **Phân loại Rủi ro AI Cao** | 1. Lưu nhật ký (Logging) mọi câu trả lời của AI. 2. Thiết lập cơ chế con người duyệt lại (Human-in-the-loop). 3. Xây dựng quy trình ngắt hệ thống (Kill-switch) khi AI sai lệch. |
| **4** | **Consent nhạy cảm (PDPL)** | 1. Tách riêng các loại Consent trên App. 2. Cho phép người dùng rút lại Consent dễ dàng. 3. Lưu log lịch sử Consent của từng user vào Database. |
| **5** | **Rủi ro dòng tiền (Pips-style)** | 1. Rà soát pháp lý của cổng thanh toán đang dùng. 2. Thiết lập ngưỡng báo động giao dịch bất thường. 3. Lưu vết KYC (định danh) tối thiểu đối với người trả tiền. |

---
