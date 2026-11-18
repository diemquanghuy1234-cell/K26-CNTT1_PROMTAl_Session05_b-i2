# Quy trình Prompt Chaining 3 Bước Viết Bài PR Sản Phẩm Công Nghệ (AI Chatbot)

## Bước 1: Nghiên cứu khách hàng & Khai thác nỗi đau (Persona & Pain Points)
Mục tiêu của bước này là tạo ra "nguyên liệu thô" đắt giá và định hình giọng điệu xuyên suốt. Kết quả được ép xuất ra dưới dạng cấu trúc dữ liệu (XML/Markdown chuẩn) để Prompt 2 đọc hiểu chính xác 100%.

* **Câu lệnh (Prompt 1):**
```text
# VAI TRÒ
Bạn là Chuyên gia Nghiên cứu Thị trường và Chiến lược Nội dung B2B (B2B Content Strategist) với 10 năm kinh nghiệm trong lĩnh vực SaaS và Trí tuệ nhân tạo.

# NHIỆM VỤ
Phân tích chân dung khách hàng mục tiêu và xác định các "nỗi đau" (pain points) cốt lõi cho sản phẩm mới: [Tên sản phẩm AI Chatbot - VD: NexaBot AI], một giải pháp AI Chatbot tự động hóa chăm sóc khách hàng và chốt đơn đa kênh dành cho doanh nghiệp vừa và nhỏ (SMEs).

# YÊU CẦU ĐẦU RA (BẮT BUỘC TUÂN THỦ CẤU TRÚC)
Hãy trình bày kết quả chính xác theo định dạng thẻ dữ liệu dưới đây để làm đầu vào cho bước tiếp theo. Không viết thêm lời chào hay giải thích thừa:

<CONTEXT_DATA>
  <TONE_OF_VOICE>Chuyên nghiệp, tin cậy, sắc bén, mang tính chuyên gia tư vấn giải pháp, tránh ngôn từ sáo rỗng hoặc quảng cáo quá lố.</TONE_OF_VOICE>
  <TARGET_AUDIENCE>
    - Chức danh: [Liệt kê 2-3 chức danh ra quyết định, VD: CEO, Giám đốc Vận hành, Trưởng phòng CSKH]
    - Đặc điểm doanh nghiệp: [Quy mô, ngành nghề]
  </TARGET_AUDIENCE>
  <PAIN_POINTS>
    1. [Tên nỗi đau 1]: [Mô tả chi tiết hậu quả về chi phí/thời gian/doanh thu] -> [Giải pháp của AI Chatbot]
    2. [Tên nỗi đau 2]: [Mô tả chi tiết hậu quả] -> [Giải pháp của AI Chatbot]
    3. [Tên nỗi đau 3]: [Mô tả chi tiết hậu quả] -> [Giải pháp của AI Chatbot]
    4. [Tên nỗi đau 4]: [Mô tả chi tiết hậu quả] -> [Giải pháp của AI Chatbot]
  </PAIN_POINTS>
  <SEO_KEYWORDS>
    - Từ khóa chính: [1 từ khóa]
    - Từ khóa phụ: [4-5 từ khóa liên quan]
  </SEO_KEYWORDS>
</CONTEXT_DATA>
```

---

## Bước 2: Thiết lập dàn ý chi tiết chuẩn SEO (Structured Outline)
Prompt 2 nhận toàn bộ khối `<CONTEXT_DATA>` từ Bước 1 làm đầu vào bắt buộc. Nó sẽ phân bổ dung lượng từ cho từng phần để đảm bảo tổng bài viết đạt 1000 - 1500 từ.

* **Câu lệnh (Prompt 2):**
```text
# VAI TRÒ
Bạn là Biên tập viên Trưởng (Managing Editor) chuyên phụ trách các bài viết PR công nghệ chuyên sâu trên các tạp chí kinh doanh uy tín.

# DỮ LIỆU ĐẦU VÀO (BẮT BUỘC SỬ DỤNG)
Dưới đây là dữ liệu nghiên cứu từ bước trước:
[DÁN TOÀN BỘ KẾT QUẢ <CONTEXT_DATA> TỪ PROMPT 1 VÀO ĐÂY]

# NHIỆM VỤ
Dựa trên dữ liệu trên, hãy lập một Dàn ý chi tiết (Outline) cho bài viết PR dài khoảng 1200 - 1500 từ. 

# YÊU CẦU CẤU TRÚC DÀN Ý
1. Giữ nguyên giọng điệu được quy định trong thẻ <TONE_OF_VOICE>.
2. Phân bổ số lượng từ dự kiến cho từng phần để đảm bảo tổng độ dài đạt 1200 - 1500 từ.
3. Trình bày đầu ra theo định dạng chuẩn dưới đây để chuyển sang bước viết bài:

<OUTLINE_DATA>
  <HEADLINE> [Đề xuất 1 tiêu đề chính giật tít, chứa từ khóa chính, đánh trúng nỗi đau lớn nhất] </HEADLINE>
  <LEAD> [Mục tiêu đoạn mở đầu: Khoảng 150 từ, đi thẳng vào nỗi đau của <TARGET_AUDIENCE> và hé lộ giải pháp] </LEAD>
  <BODY_SECTIONS>
    - H2: [Tiêu đề H2 số 1 - Tập trung phân tích bối cảnh & nỗi đau] (Dự kiến: 300 từ)
      + H3: [Ý nhỏ 1.1]
      + H3: [Ý nhỏ 1.2]
    - H2: [Tiêu đề H2 số 2 - Giới thiệu AI Chatbot như một bước ngoặt giải quyết vấn đề] (Dự kiến: 350 từ)
      + H3: [Tính năng 1 giải quyết Pain point 1]
      + H3: [Tính năng 2 giải quyết Pain point 2]
    - H2: [Tiêu đề H2 số 3 - Hiệu quả thực tế & Lợi ích định lượng cho doanh nghiệp] (Dự kiến: 300 từ)
      + H3: [Bài toán tối ưu chi phí/nhân sự]
      + H3: [Tăng trưởng tỷ lệ chuyển đổi]
  </BODY_SECTIONS>
  <CTA> [Mục tiêu đoạn kết & Kêu gọi hành động: Khoảng 150 từ, tạo sự khan hiếm hoặc ưu đãi dùng thử, thúc đẩy hành động ngay] </CTA>
</OUTLINE_DATA>
```

---

## Bước 3: Triển khai viết chi tiết & Tối ưu SEO (Content Generation)
Để tránh việc AI viết lướt qua cho xong, Prompt 3 yêu cầu AI phải viết sâu, sử dụng số liệu giả định hợp lý (hoặc số liệu thật nếu bạn cung cấp) và tuân thủ nghiêm ngặt dàn ý.

* **Câu lệnh (Prompt 3):**
```text
# VAI TRÒ
Bạn là Cây bút PR Công nghệ cấp cao (Senior Tech PR Copywriter).

# DỮ LIỆU ĐẦU VÀO
1. Ngữ cảnh & Giọng điệu:
[DÁN LẠI THẺ <TONE_OF_VOICE> VÀ <SEO_KEYWORDS> TỪ PROMPT 1]

2. Dàn ý chi tiết:
[DÁN TOÀN BỘ KẾT QUẢ <OUTLINE_DATA> TỪ PROMPT 2]

# NHIỆM VỤ
Hãy viết hoàn chỉnh bài PR dựa trên dàn ý và dữ liệu trên. 

# QUY TẮC VIẾT BÀI (BẮT BUỘC)
- Độ dài: Đạt từ 1000 đến 1500 từ. Viết sâu sắc, phân tích kỹ lưỡng từng luận điểm, tuyệt đối không viết tóm tắt hay gạch đầu dòng sơ sài.
- Định dạng: Sử dụng chuẩn Markdown (# cho Tiêu đề chính, ## cho H2, ### cho H3).
- SEO: Chèn tự nhiên từ khóa chính và từ khóa phụ vào Tiêu đề, đoạn Lead, các thẻ H2/H3 và rải đều trong bài. In đậm các từ khóa hoặc thông điệp quan trọng.
- Giọng điệu: Duy trì xuyên suốt sự chuyên nghiệp, tin cậy, khách quan như một bài báo phân tích chuyên ngành.
- Kết thúc bài bằng thẻ `[HẾT BÀI VIẾT]` để xác nhận đã hoàn thành toàn bộ dàn ý.
```

---

## Quy tắc xử lý đứt gãy ngữ cảnh (Anti-Truncation Protocol)
Khi viết bài dài 1500 từ, AI thường gặp giới hạn *max output tokens* và bị dừng đột ngột giữa câu. Nếu không thấy thẻ `[HẾT BÀI VIẾT]` ở cuối, bạn tuyệt đối **không** gõ lệnh chung chung như *"Viết tiếp đi"* (vì AI sẽ dễ bị đổi giọng văn hoặc viết lặp lại đoạn trước).

Hãy sử dụng **Prompt điều khiển tiếp tục** dưới đây:

```text
# LỆNH ĐIỀU KHIỂN TIẾP TỤC (CONTINUATION PROMPT)
Hệ thống đã ngắt quãng do giới hạn độ dài. Hãy viết tiếp phần còn lại của bài PR dựa trên <OUTLINE_DATA> đã cung cấp.

# QUY TẮC NỐI MẠCH VĂN (BẮT BUỘC)
1. Điểm bắt đầu: Nối tiếp NGAY LẬP TỨC từ cụm từ cuối cùng bị ngắt sau đây: "[DÁN 10 - 15 TỪ CUỐI CÙNG MÀ AI VỪA VIẾT DỞ]"
2. Không lặp lại tiêu đề hay các đoạn đã viết trước đó. Không thêm lời dẫn nhập kiểu "Dưới đây là phần tiếp theo...".
3. Giữ nguyên 100% giọng điệu chuyên nghiệp, tin cậy và văn phong của phần trước.
4. Tiếp tục hoàn thành các thẻ H2, H3 và phần CTA còn lại trong dàn ý cho đến khi kết thúc bằng thẻ `[HẾT BÀI VIẾT]`.
```

---

## Tóm tắt cơ chế bảo toàn tính nhất quán của chuỗi
* **Đóng gói dữ liệu bằng thẻ XML (`<CONTEXT_DATA>`, `<OUTLINE_DATA>`):** Giúp mô hình ngôn ngữ phân tách rạch ròi đâu là chỉ thị (instruction) và đâu là dữ liệu (data), ngăn chặn tình trạng "trôi ngữ cảnh" (context drift).
* **Truyền biến số `<TONE_OF_VOICE>` xuyên suốt:** Thẻ giọng điệu được định nghĩa ở Bước 1 và được gọi lại ở cả Bước 2 và Bước 3, đảm bảo văn phong không bị biến đổi từ đầu đến cuối bài.
* **Cơ chế neo từ khóa (Anchor Words) khi đứt gãy:** Việc bắt AI nối tiếp từ 10-15 từ cuối cùng bị ngắt giúp thuật toán dự đoán từ tiếp theo (next-token prediction) khớp nối hoàn hảo về mặt ngữ pháp lẫn mạch tư duy.

