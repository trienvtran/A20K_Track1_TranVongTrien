
## Incident Playbook

**Tình huống:** 9h30 sáng, khách hàng tweet ảnh AI của GlucuCare tư vấn sai về thực phẩm cho người tiểu đường, bài đăng đạt 200 retweets trong 30 phút.

## Bước 1. Verify (3 phút)
* **Check log tại:** **Helicone** (để xem toàn bộ trace từ user prompt đến AI response) và **Database** (để đối chiếu với chỉ số thực tế của user đó).
* **Verify thật vs giả:** Copy `request_id` từ screenshot của khách (nếu có) tra vào Helicone. Nếu không có ID, đối soát timestamp và nội dung tin nhắn trong DB. Nếu không tìm thấy bản ghi trùng khớp -> Screenshot là giả (photoshop).

## Bước 2. Stop the bleeding (5 phút)
* **Option chọn:** **Hard Switch** (Ngắt kết nối AI ngay lập tức, chuyển sang chế độ "Bảo trì" hoặc chỉ cho phép dùng công cụ tra cứu tĩnh).
* **Lý do:** Đây là sản phẩm y tế. Một thông tin sai lệch có thể gây nguy hiểm tính mạng. Phải ưu tiên an toàn tuyệt đối trước khi tìm hiểu nguyên nhân gốc rễ (Root Cause).

## Bước 3. Customer comm (5 phút)
*Gửi DM trực tiếp cho người tweet bài:*

**Subject: Từ [Tên Founder] - Founder GlucuCare: Về sự cố tư vấn sáng nay**

Chào bạn,
Tôi là [Tên của bạn], Founder của GlucuCare. Tôi vừa trực tiếp kiểm tra hệ thống và xác nhận lỗi tư vấn sai mà bạn đã chia sẻ trên X.

**Chuyện gì đã xảy ra:** AI của chúng tôi đã nhầm lẫn dữ liệu giữa hai loại thực phẩm, dẫn đến lời khuyên không chính xác cho trường hợp của bạn. Đây là sai sót nghiêm trọng mà tôi chịu trách nhiệm cao nhất.
**Tôi đang làm gì:** Tôi đã tạm ngắt hệ thống AI để rà soát lại toàn bộ bộ lọc an toàn (Guardrails).
**Để bù đắp:** Tôi đã gửi tặng bạn 1 năm sử dụng gói Premium hoàn toàn miễn phí và một voucher kiểm tra sức khỏe tổng quát trị giá 2.000.000đ — không cần thủ tục gì thêm.
**Kết nối trực tiếp:** Nếu bạn cần trao đổi thêm, đây là số điện thoại cá nhân của tôi: [Số điện thoại của bạn].

-- [Tên ]
Email: [Email ]@glucucare.vn

## Bước 4. Public response (2 phút)
*Đăng tweet từ tài khoản Founder:*

> Chúng tôi đã ghi nhận sự cố tư vấn sai của GlucuCare sáng nay. Với tư cách Founder, tôi gửi lời xin lỗi chân thành đến cộng đồng. Chúng tôi đã tạm dừng tính năng AI để siết chặt bộ lọc an toàn y tế. An toàn của các bạn là ưu tiên số 1. Sẽ có báo cáo chi tiết trong 24h tới.
