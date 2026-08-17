# Track 1 — Day 17 Lab Assignment: Finding and Validating Pain Points

**Học viên:** Lê Hoàng Việt  
**Mã học viên:** 2A202601543  
**Case Study:** Case C — AI Support Radar  
**Repo:** `Track1_Day17_2A202601543_LeHoangViet`  
**Ngày thực hiện:** 17/08/2026  

---

## Cấu Trúc Thư Mục Nộp Bài

```
Track1_Day17_2A202601543_LeHoangViet/
├── README.md                              # Báo cáo tổng hợp đầy đủ 5 phần
├── checkpoint_1_problem_hypothesis.md     # Báo cáo Chặng 1 — Đặt giả thuyết
├── checkpoint_2_interview_analysis.md     # Báo cáo Chặng 2 — Phân tích & Đối chiếu chéo
└── interview/
    ├── notes.md                           # Ghi chép chi tiết 4 cuộc phỏng vấn (3 Thật + 1 Mô phỏng)
    └── recording.m4a                      # File ghi âm phỏng vấn thực tế
```

---

## 1. Thông Tin Chung & Bối Cảnh Case Study

- **Case Study C:** AI Support Radar — Hệ thống AI phân tích hành vi học tập (thời gian dừng trên slide, ghi chú, xem lại bài) để tự động phát hiện học viên đang gặp khó khăn và thông báo cho giảng viên.
- **Mục tiêu Lab:** 
  1. Đặt giả thuyết vấn đề (Problem Hypothesis) đa chiều, nhận diện Actor, Situation, Pain, JTBD và các mắt xích yếu nhất.
  2. Xây dựng Conversation Guide không mớm lời để xác thực vấn đề.
  3. Thực hiện phỏng vấn thực tế (Learner, Lab Coach) kết hợp mô phỏng (Instructor) để đối chiếu chéo (Cross-Interview Synthesis).
  4. Đúc kết bài học, nhận diện sự sụp đổ của giải pháp công nghệ ban đầu và đề xuất các hướng Pivot chiến lược.

---

## 2. Problem Hypothesis Brief (Tóm Tắt Chặng 1)

Chuỗi lập luận ban đầu của Case C:

```
Solution: AI Support Radar (phân tích log slide/LMS)
   │
   ▼
Change: Giảng viên nhận danh sách học viên đang gặp khó khăn sau mỗi buổi học
   │
   ▼
Actor: Giảng viên (người nhận thông tin) + Lab Coach (người hỗ trợ) + Học viên (người gặp khó)
   │
   ▼
Situation & Job: 10–15 phút cuối buổi học lý thuyết / trong giờ lab thực hành
   │
   ▼
Pain 1 (A): Giảng viên KHÔNG BIẾT ai đang kẹt và kẹt phần nào để hỗ trợ kịp thời
Pain 2 (B): Giảng viên & Coach QUÁ TẢI, không có thời gian rà soát từng học viên
   │
   ▼
Mắt xích yếu nhất: Giả định rằng "sự không hiểu sẽ để lại dấu vết số (digital traces) trên slide/LMS"
```

- **Pain Hypothesis A (Thiếu Visibility):** Giảng viên không có visibility về mức độ hiểu bài của học viên trong và ngay sau buổi học → Dẫn đến phát hiện muộn sau 3–14 ngày, tỷ lệ dropout âm thầm tăng.
- **Pain Hypothesis B (Quá tải vận hành):** Giảng viên và Coach bị quá tải, không thể chủ động hỏi thăm từng học viên theo cách thủ công.
- **Chi tiết đầy đủ:** Xem tại [checkpoint_1_problem_hypothesis.md](./checkpoint_1_problem_hypothesis.md).

---

## 3. Conversation Guide (Bản Cuối — Sau Khi Luyện & Hiệu Chỉnh)

### Bộ A — Giảng Viên / Instructor (21 câu)
- **Big 3 cần học:**
  1. Giảng viên đánh giá mức độ hiểu bài của lớp bằng cách nào? (Visibility thật vs ảo)
  2. Khi lớp im lặng, giảng viên nghĩ gì? (Tách A khỏi B1 mà không mớm lời)
  3. Từng có ai bỏ khóa/đuối mà không nhận ra kịp không? (Đo mức độ đau và chi phí bỏ lỡ)
- **Câu then chốt ★:** *"Khi cả lớp im lặng lúc anh/chị hỏi 'có ai chưa hiểu không', lúc đó anh/chị nghĩ gì?"*

### Bộ B — Học Viên / Learner (17 câu)
- **Big 3 cần học:**
  1. Khi không hiểu, học viên có biết ngay lúc đó không? (Tách "ngại hỏi" khỏi "tưởng đã hiểu")
  2. Hành vi thực tế khi kẹt là gì? Có để lại dấu vết trên slide/LMS không?
  3. Rủi ro ngược: Học viên có cảm thấy bị giám sát tiêu cực nếu hệ thống tự cảnh báo không?
- **Câu then chốt ★:** *"Lúc còn đang trong buổi học, bạn có nhận ra mình chưa nắm phần đó không — hay về nhà mới biết?"*
- **Câu rủi ro ngược ★:** *"Nếu giảng viên/hệ thống tự nhiên nhắn 'thấy em đang vướng phần X', bạn cảm thấy thế nào?"*

### Bộ C — Lab Coach (Mở rộng sau thực tế)
- **Big 3 cần học:**
  1. Coach phân bổ thời gian ra sao (chủ động hỗ trợ vs đứng chờ)?
  2. Coach phát hiện học viên gặp khó bằng những tín hiệu nào?
  3. Luồng thông tin phản hồi sau giờ lab được chuyển giao cho ai?
- **Câu then chốt ★:** *"Sau các buổi lab, anh/chị có thường cập nhật tình hình khó khăn của lớp cho giảng viên không?"*

---

## 4. Practice Reflection (Đúc Kết Thực Hành Phỏng Vấn)

### 1. Câu hỏi nào đã giúp mở được câu chuyện thật của User?
> **"Lần gần nhất bạn nghe giảng mà không hiểu là khi nào? Chuyện gì xảy ra sau đó?"**  
> Câu hỏi này hướng thẳng vào một sự kiện quá khứ cụ thể, tránh được câu trả lời chung chung. Cả 2 học viên phỏng vấn thật đều kể lại chi tiết: QT tự tra cứu trong vài phút, còn bạn học viên thứ 2 thì buông xuôi bỏ qua luôn vì "ngại".

### 2. Chỗ cần làm tốt hơn ở các lần phỏng vấn tiếp theo
> **Bắt buộc phải thực hiện đầy đủ câu hỏi về Rủi ro ngược (Negative Risk / Privacy).**  
> Trong buổi luyện ban đầu, interviewer dễ bị cuốn theo câu chuyện về hành vi kỹ thuật mà quên mất việc kiểm tra xem học viên có cảm thấy bị "xâm phạm riêng tư / soi mói" khi bị theo dõi hành vi hay không.

### 3. Những thay đổi cốt lõi của Conversation Guide sau thực chiến
1. **Thêm Bộ câu hỏi cho Lab Coach:** Phát hiện Coach là "cảm biến hiện trường" nắm 90% dữ liệu thực tế tại phòng lab.
2. **Loại bỏ hoàn toàn các câu hỏi dẫn dắt:** Sửa *"Bạn có xem lại slide nhiều lần không?"* thành câu hỏi mở *"Khi gặp chỗ khó, bạn thường làm gì tiếp theo?"*.
3. **Thêm quy tắc Big 3 & đánh dấu ngôi sao (★):** Giúp interviewer luôn bám sát mục tiêu cốt lõi của buổi phỏng vấn.

---

## 5. AI Support Log (Nhật Ký Tương Tác AI & Bài Học Bias)

### AI Đã Hỗ Trợ Những Gì?
1. **Xây dựng Problem Framing:** Hỗ trợ mô hình hóa chuỗi giá trị và viết 2 giả thuyết đối nghịch (Pain A vs Pain B).
2. **Thiết kế & Hoàn thiện Conversation Guide:** Tinh chỉnh các câu hỏi phỏng vấn theo phương pháp Mom Test, loại bỏ các bẫy hỏi tương lai và mớm lời.
3. **Tổng hợp dữ liệu đa nguồn:** Hỗ trợ xây dựng ma trận đối chiếu chéo 3 chiều (Giảng viên, Học viên, Lab Coach).

### Điểm AI Sai Lầm / Hời Hợt Và Cách Đã Khắc Phục Thực Tế

| Vấn đề / Sai lầm ban đầu của AI | Bài học thực tế & Cách khắc phục |
| :--- | :--- |
| **Confirmation Bias trong dữ liệu mô phỏng Coach:** AI ban đầu tạo kịch bản mô phỏng rằng Lab Coach "ngồi chờ lãng phí 70% thời gian, thiếu tự tin không dám tiếp cận học viên". | **Phỏng vấn Lab Coach THỰC TẾ lật ngược hoàn toàn:** Coach hoạt động 90%+ công suất, chủ động can thiệp bằng quan sát sắc thái và màn hình code, không ngồi chờ. |
| **Bỏ sót cấu trúc tổ chức:** AI giả định Coach báo cáo trực tiếp cho Giảng viên. | **Phát hiện đứt gãy luồng tin thật:** Coach báo cáo cho **Bên Vận hành (Operations)**, khiến Giảng viên hoàn toàn bị cô lập thông tin. |
| **Đề xuất Pivot công nghệ quá vội vã:** AI ban đầu muốn xây dựng AI Radar phức tạp hơn. | **Nhận diện nguyên nhân phi công nghệ:** Vấn đề gốc rễ là **thiếu kênh đồng bộ thông tin nội bộ (Coach ➔ Giảng viên)** chứ không phải thiếu thuật toán AI. |

---

## Tham Chiếu Chi Tiết

- [checkpoint_1_problem_hypothesis.md](./checkpoint_1_problem_hypothesis.md) — Chi tiết Chặng 1
- [checkpoint_2_interview_analysis.md](./checkpoint_2_interview_analysis.md) — Chi tiết Chặng 2 & Ma trận Evidence
- [interview/notes.md](./interview/notes.md) — Transcript chi tiết 4 cuộc phỏng vấn