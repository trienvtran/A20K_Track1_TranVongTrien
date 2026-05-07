**Risk lớn nhất:** AI đưa ra lời khuyên dinh dưỡng sai lệch dẫn đến tăng/hạ đường huyết cấp tính.

## R1 — RULES (3 phút)
* **Cấm cụ thể:** Nghiêm cấm sử dụng dữ liệu thô từ OpenAI/Gemini để đưa ra liều lượng thuốc hoặc chẩn đoán bệnh mà không qua bộ lọc y tế (Medical Guardrails).
* **Allowed alternative:** Sử dụng dữ liệu từ nguồn tin cậy (Bộ Y tế, Hiệp hội Đái tháo đường) làm Ground Truth. Chi phí: ~$100/tháng cho API dữ liệu chuyên ngành hoặc nhân sự kiểm định.
* **Hậu quả vi phạm:** Nhân sự tự ý thay đổi Logic Guardrail mà không có sự đồng ý của CTO sẽ bị đình chỉ công tác và xem xét chấm dứt hợp đồng ngay lập tức.
* **Update mechanism:** Toàn bộ quy tắc về lời khuyên y tế được cập nhật ngày 1 hàng tháng, có sự tham gia của chuyên gia dinh dưỡng và pháp lý để đảm bảo tuân thủ quy định mới nhất.

## R2 — RAILS (5 phút)
* **Tool 1: NeMo Guardrails (NVIDIA):** Dùng để chặn các câu hỏi ngoài phạm vi dinh dưỡng và lọc các câu trả lời mang tính chất "chẩn đoán y khoa" nguy hiểm. Cost: Open-source (Self-hosted trên AWS ~$50/tháng).
* **Tool 2: Lakera Guard:** Tích hợp trực tiếp vào API để chặn các cuộc tấn công Prompt Injection có thể khiến AI "quên" các quy tắc an toàn y tế. Cost: ~$200/tháng cho gói startup.

## R3 — RITUAL (5 phút)
* **Ritual hàng tuần:** "Medical Safety Review" vào 14h chiều Thứ Sáu hàng tuần. Toàn bộ team Engineering và Chuyên gia dinh dưỡng sẽ ngồi lại để review 5 trường hợp AI đưa ra lời khuyên bị người dùng đánh dấu là "nghi ngờ".
* **Question của Founder:** "Trong tuần qua, có trường hợp nào AI đưa ra lời khuyên mà nếu người dùng làm theo 100% sẽ dẫn đến nguy cơ phải nhập viện không?"

