
### Dependency 1: Vision AI API (Image recognition + reasoning)

**Worst-case:**  
API bị khóa hoặc tăng giá đột ngột khiến chi phí mỗi user không khả thi.

**Plan B:**  
- Xây abstraction layer cho model (LiteLLM hoặc tương đương)  
- Fallback sang model rẻ hơn (Gemini Flash) với scope hạn chế (chỉ nhận diện basic, không phân tích sâu)  
- Giảm tần suất gọi API bằng caching + yêu cầu user chọn từ preset khi confidence thấp  

**Cost:**  
~1–2 tuần dev + trade-off giảm độ chính xác trong ngắn hạn  

---

### Dependency 2: App Store / Google Play Review

**Worst-case:**  
App bị reject nhiều lần do bị classify là “medical advice app”, delay launch > 2–4 tuần.

**Plan B:**  
- Reframe sản phẩm thành “health logging tool”, không claim medical advice  
- Tách feature nhạy cảm (prediction) ra khỏi bản đầu  
- Chuẩn bị Web App (PWA) để pilot user mà không phụ thuộc Store  

**Cost:**  
~1–2 tuần chỉnh copy + 1 tuần deploy PWA  

---

### Dependency 3: User Adoption (Elderly usage)

**Worst-case:**  
Người cao tuổi không sử dụng app đủ đều → không có dữ liệu → toàn bộ hệ thống mất giá trị.

**Plan B:**  
- Thiết kế fallback input: chọn nhanh (preset) thay vì phụ thuộc vào ảnh  
- Cho phép caregiver nhập hộ trong giai đoạn đầu  
- Thử nghiệm onboarding trực tiếp tại nhà thuốc (assisted onboarding)  

**Cost:**  
~1 tuần UX adjustment + chi phí training tại điểm bán  

---

### Dependency 4: Pháp lý & Dữ liệu 

**Worst-case:**  
Bị yêu cầu dừng hoạt động do xử lý dữ liệu sức khỏe không compliant.

**Plan B:**  
- Tách PII và health data  
- Lưu trữ dữ liệu nhạy cảm tại server nội địa (Viettel/FPT)  
- Chỉ gửi dữ liệu đã anonymized ra ngoài cho AI xử lý  

**Cost:**  
~3–5 tuần infra + tăng chi phí vận hành ~20–30%  

---

## 2. Critical Path (NOW - 60–90 ngày)

### Tasks

T1: Thiết kế & triển khai Structured Logging UX (Blocking T2, T4)  
T2: Xây dựng pipeline lưu trữ dữ liệu (meal + glucose) (Blocking T4)  
T3: Thiết lập dashboard caregiver (Blocking T5)  
T4: Pilot onboarding tại nhà thuốc (Blocking T5)  
T5: Đo lường habit formation & retention (>= 14 ngày cohort)  

---

### Critical Path

T1 → T2 → T4 → T5  

---
