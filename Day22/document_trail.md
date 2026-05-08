# Document Trail - GlucuCare Legal & Safety Checklist
## 1. Đối chiếu 5 loại hồ sơ thẩm định
| Tuần | Deadline | Loại hồ sơ | Nội dung cần hoàn thành |
| --- | --- | --- | --- |
| **Tuần 1** | **12/05/2026** | **Phê duyệt Marketing** | Rà soát lại Landing Page, Slide Deck. Thay các từ "điều trị", "100%", "thay thế bác sĩ" bằng bản "Honest Version". |
| **Tuần 2** | **15/05/2026** | **Hồ sơ DPIA (NĐ 13)** | Lập báo cáo đánh giá tác động dữ liệu (mô tả luồng dữ liệu mâm cơm đi qua server quốc tế và cách bảo mật). |
| **Tuần 3** | **22/05/2026** | **Hồ sơ CTIA (NĐ 13)** | Hoàn thiện và nộp hồ sơ đánh giá tác động chuyển dữ liệu ra nước ngoài cho Cục An ninh mạng (A05). |
| **Tuần 4** | **01/06/2026** | **Consent & Privacy** | Cập nhật luồng đồng ý trên App: Tách riêng nút "Đồng ý xử lý dữ liệu sức khỏe nhạy cảm" thay vì gộp chung vào điều khoản sử dụng. |

---
## 2. TOP 1 

* **Lựa chọn:** **Hồ sơ DPIA / CTIA (Đánh giá tác động xử lý & chuyển dữ liệu cá nhân).**
* **Lý do:** Đây là bằng chứng vật chứng duy nhất để chứng minh GlucuCare không cố tình vi phạm Nghị định 13 khi gửi dữ liệu sức khỏe người Việt sang OpenAI/Gemini; thiếu hồ sơ này đồng nghĩa với việc mất quyền bảo vệ khi có thanh tra dữ liệu.

---

## 3. Hành động 1 tuần cho hồ sơ DPIA/CTIA

### Template tài liệu :

1. **Luồng dữ liệu (Data Flow):** Mô tả chi tiết hành trình từ mâm cơm (ảnh) -> Cloud (Vietnam) -> API LLM (Overseas) -> Kết quả (Dashboard).
2. **Ma trận rủi ro:** Định danh rủi ro lộ lọt tại các điểm chạm vendor và biện pháp mã hóa/ẩn danh đã áp dụng.
3. **Cơ chế Consent:** Minh chứng về nút bấm "Đồng ý xử lý dữ liệu nhạy cảm" riêng biệt đã triển khai trên app.
4. **Báo cáo tác động:** Phân tích lợi ích mang lại cho bệnh nhân tiểu đường so với rủi ro bảo mật tiềm ẩn.
5. **Cam kết Vendor:** Phụ lục các chứng chỉ bảo mật (SOC2, HIPAA) của OpenAI/Microsoft Azure để chứng minh đã chọn vendor uy tín.

### Vận hành:

* **Người chịu trách nhiệm:** Founder (Trực tiếp phê duyệt nội dung và nộp hồ sơ).
* **Tần suất cập nhật:** 01 lần ngay bây giờ + Cập nhật ngay khi thay đổi luồng dữ liệu hoặc đổi Vendor AI chính.

