# TOP 10 RỦI RO SỐNG CÒN — GLUCUCARE AI

**Tổng vốn:** 1.700.000.000 VNĐ | **Runway:** 24 tháng | **Burn rate:** ~71 triệu VNĐ/tháng

---

### RISK 1: Bị xếp loại là "Tư vấn y tế" (Medical Classification)
* **Loại:** Regulatory
* **Nếu:** Dùng từ ngữ khẳng định (an toàn/nguy hiểm) dẫn đến bị cơ quan chức năng hoặc App Store tuýt còi / **Thì:** Phải dừng hoạt động để sửa toàn bộ nội dung và cấu trúc pháp lý.
* **Dẫn đến:** Chi phí luật sư + 4 tháng vận hành không doanh thu = **Mất 5 tháng runway (~355 triệu VNĐ)**.
* **Likelihood:** 4/5 | **Impact:** 5/5
* **Giảm thiểu:** 1. Chỉ dùng từ mô tả (ví dụ: "vượt ngưỡng"). 2. Đặt Disclaimer tại mọi màn hình. 3. Tách lớp AI gợi ý ra khỏi bản MVP.

### RISK 2: Người cao tuổi bỏ dùng sau 7 ngày (User Churn)
* **Loại:** Customer-facing
* **Nếu:** Chụp ảnh mâm cơm quá phiền phức / **Thì:** Người già ngừng dùng, Caregiver thấy app vô dụng và hủy trả phí.
* **Dẫn đến:** Pilot thất bại, phải pivot toàn bộ sản phẩm = **Mất 4 tháng runway (~284 triệu VNĐ)**.
* **Likelihood:** 5/5 | **Impact:** 5/5
* **Giảm thiểu:** 1. Build luồng "ghi nhanh 3 chạm" không cần ảnh. 2. Cho con cái nhập hộ dữ liệu. 3. Đo metric "số ngày có dữ liệu" thay vì "số ảnh".

### RISK 3: OpenAI/Anthropic tăng giá hoặc siết chính sách (API Fragility)
* **Loại:** Vendor
* **Nếu:** Giá API Vision tăng hoặc OpenAI cấm mảng Y tế / **Thì:** Unit Economics vỡ (chi phí server vượt ARPU), tính năng cốt lõi bị ngắt.
* **Dẫn đến:** 2 tháng code lại hạ tầng + 1 tháng vận hành trễ = **Mất 3 tháng runway (~213 triệu VNĐ)**.
* **Likelihood:** 4/5 | **Impact:** 4/5
* **Giảm thiểu:** 1. Chốt lớp trung gian (Abstraction) để đổi model trong 24h. 2. Caching kết quả nhận diện món phổ biến. 3. Có chế độ fallback không AI.

### RISK 4: Vi phạm dữ liệu cá nhân 
* **Loại:** Regulatory
* **Nếu:** Lộ dữ liệu sức khỏe hoặc lưu trữ server ngoại không đúng quy định / **Thì:** Bị phạt hành chính và yêu cầu đóng cửa hạ tầng để khắc phục.
* **Dẫn đến:** Án phí + Chi phí migration dữ liệu cấp tốc = **Mất 6 tháng runway (~426 triệu VNĐ)**.
* **Likelihood:** 2/5 | **Impact:** 5/5
* **Giảm thiểu:** 1. Tách biệt PII và Health data trong DB. 2. Lưu dữ liệu nhạy cảm tại server nội địa. 3. Lưu log Consent rõ ràng.

### RISK 5: Founder "nghẽn cổ chai" (Founder Bottleneck)
* **Loại:** Founder-bandwidth
* **Nếu:** Founder ôm hết từ code đến sale nhà thuốc / **Thì:** Critical bug không được fix kịp, mất uy tín với đối tác chuỗi.
* **Dẫn đến:** Chậm tiến độ học hỏi, đốt tiền vô ích = **Mất 2 tháng runway (~142 triệu VNĐ)**.
* **Likelihood:** 5/5 | **Impact:** 3/5
* **Giảm thiểu:** 1. Chỉ tập trung 1 metric sống còn/tháng. 2. Từ chối mọi yêu cầu "custom" ngoài roadmap. 3. Outsource thủ tục giấy tờ.

### RISK 6: "Ảo giác" AI gây cảnh báo sai (AI Hallucination)
* **Loại:** Customer-facing
* **Nếu:** AI nhận diện sai (ví dụ: nhầm món ngọt thành món kiêng) / **Thì:** Cảnh báo sai liên tục khiến Caregiver mất niềm tin và tắt thông báo.
* **Dẫn đến:** Tính năng quan trọng nhất bị vô hiệu hóa = **Mất 3 tháng runway (~213 triệu VNĐ)**.
* **Likelihood:** 4/5 | **Impact:** 4/5
* **Giảm thiểu:** 1. Thiết lập ngưỡng tin cậy (Confidence score). 2. Cơ chế Human-in-the-loop (con cái duyệt lại). 3. Chỉ alert khi có xu hướng nguy hiểm thực sự.

### RISK 7: Kênh nhà thuốc không ra số (Distribution Failure)
* **Loại:** Partner
* **Nếu:** Nhân viên nhà thuốc không mặn mà giới thiệu app / **Thì:** CAC (chi phí có khách) tăng vọt, không đạt mốc user để gọi vốn vòng sau.
* **Dẫn đến:** Gãy kênh phân phối chính, phải tìm kênh mới từ đầu = **Mất 4 tháng runway (~284 triệu VNĐ)**.
* **Likelihood:** 4/5 | **Impact:** 4/5
* **Giảm thiểu:** 1. Onboarding cho dược sĩ trong dưới 60 giây. 2. Đo conversion từng cửa hàng. 3. Có kênh dự phòng (Referral từ con cái).

### RISK 8: Không đủ dữ liệu để AI "học" (Data Starvation)
* **Loại:** Customer-facing
* **Nếu:** User nhập liệu rời rạc / **Thì:** Không tạo được vòng lặp dữ liệu đóng.
* **Dẫn đến:** Không chứng minh được lợi thế công nghệ khi gọi vốn tiếp = **Mất 3 tháng runway (~213 triệu VNĐ)**.
* **Likelihood:** 4/5 | **Impact:** 4/5
* **Giảm thiểu:** 1. Nhắc nhở thông minh dựa trên giờ ăn. 2. Game hóa (Streak). 3. Dùng Rule-based làm lõi trước khi dùng AI.

### RISK 9: Lỗi hạ tầng thông báo (Communication Failure)
* **Loại:** Vendor
* **Nếu:** Provider SMS/Push lỗi hoặc tăng giá / **Thì:** Con cái không nhận được cảnh báo kịp thời.
* **Dẫn đến:** Giảm Retention rõ rệt = **Mất 1 tháng runway (~71 triệu VNĐ)**.
* **Likelihood:** 3/5 | **Impact:** 2/5
* **Giảm thiểu:** 1. Đa dạng kênh: Zalo, In-app, Email. 2. Dùng Local Notification cho các nhắc nhở định kỳ.

### RISK 10: App Store chặn Launch (Platform Risk)
* **Loại:** Vendor
* **Nếu:** Apple/Google giữ app vì lý do "Medical Advice" / **Thì:** Trễ tiến độ Pilot với nhà thuốc.
* **Dẫn đến:** Mất đà thị trường = **Mất 2 tháng runway (~142 triệu VNĐ)**.
* **Likelihood:** 3/5 | **Impact:** 3/5
* **Giảm thiểu:** 1. Đăng ký category "Health & Fitness", tránh "Medical". 2. Chuẩn bị sẵn bản PWA (Web App) để chạy Pilot.

