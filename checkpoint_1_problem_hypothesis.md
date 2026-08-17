# Chặng 1 — Đặt giả thuyết

---

## 1. Solution — Gỡ solution khỏi hình thức cụ thể

**Case đã chọn:** Case C — AI Support Radar

**Solution directive:**

> Sau mỗi phiên học, hệ thống phân tích các tín hiệu như di chuyển giữa slide, dừng lâu hoặc xem lại, highlight và ghi chú, đánh dấu "Chưa hiểu", thay đổi câu trả lời, và nội dung trao đổi với AI Chat. AI tạo một Support Queue cho giảng viên, gồm: Những học viên có thể cần hỗ trợ; Phần nội dung mà họ có thể đang gặp khó khăn; Các tín hiệu dẫn đến nhận định đó; Một hành động hỗ trợ được đề xuất. Giảng viên xem lại và quyết định có liên hệ với học viên hay không.

**Capability trung tính:**

> Nhận diện sớm những học viên đang gặp khó khăn trong việc hiểu bài sau một phiên học — kể cả khi họ không chủ động lên tiếng — và cung cấp đủ ngữ cảnh để người phụ trách giảng dạy quyết định có can thiệp hỗ trợ hay không.

---

## 2. Change — Làm lộ chuỗi thay đổi được kỳ vọng

```
Solution → Instructor nhìn thấy ai đang kẹt và kẹt ở đâu (Visibility) → Instructor chủ động liên hệ hỗ trợ đúng trọng tâm → Learner được gỡ kẹt kịp thời, giảm dropout (Outcome)
```

**Các thay đổi được kỳ vọng:**

1. **Instructor biết được điều trước đây không biết:** Sau phiên học, Instructor nhìn thấy danh sách học viên có dấu hiệu nghẽn kiến thức kèm ngữ cảnh cụ thể (kẹt ở slide nào, tín hiệu hành vi gì), thay vì chỉ thấy nhóm học viên chủ động hỏi.
2. **Instructor thay đổi hành vi:** Từ bị động (chờ học viên tìm đến) sang chủ động (mở danh sách, chọn học viên ưu tiên và liên hệ trước buổi học tiếp theo).
3. **Learner nhận được hỗ trợ mà không cần tự giơ tay:** Learner đang im lặng được Instructor tiếp cận, gỡ đúng điểm nghẽn mà không phải vượt qua rào cản tâm lý khi tự đi hỏi.

> **Lưu ý:** Nếu Instructor không mở danh sách hoặc không dành thời gian liên hệ, solution không tạo được outcome — dù AI phân tích chính xác 100%.

---

## 3. Actor — Xác định các nhóm người có liên quan

| Actor | Họ đang làm gì? | Pain hoặc hậu quả có thể có | Họ hưởng lợi thế nào? |
| :--- | :--- | :--- | :--- |
| **Instructor / Coach** | Dạy học, theo dõi tiến độ lớp, trả lời khi có người hỏi. | Không biết ai đang đuối trong nhóm học viên im lặng; chỉ phát hiện khi học viên nộp bài kém hoặc bỏ học. | Có visibility về tình trạng hiểu bài thực tế của cả lớp, biết nên ưu tiên hỗ trợ ai. |
| **Learner (đang kẹt)** | Tự học qua slide, gặp chỗ khó thì tự loay hoay hoặc bỏ qua. | Ngại hỏi, không biết diễn đạt thắc mắc; tích tụ lỗ hổng dẫn đến tụt hậu hoặc bỏ khóa. | Được gỡ kẹt đúng lúc mà không phải tự thừa nhận mình không hiểu. |
| **Learner (không kẹt)** | Học bình thường theo tiến độ. | Rủi ro bị hệ thống nhận diện nhầm (false positive) do thói quen đọc chậm. | Gần như không hưởng lợi trực tiếp. |

**Actor nhóm chọn để điều tra trước:** Instructor / Coach

**Vì sao chọn nhánh này thay vì actor khác:** Instructor là mắt xích yếu nhất trong chuỗi Change — nếu Instructor không có nhu cầu phát hiện học viên đuối sau buổi học, hoặc đã có đủ công cụ để làm việc này, thì toàn bộ solution mất lý do tồn tại. Cần kiểm chứng phía cung cấp hỗ trợ trước khi kiểm chứng phía nhận hỗ trợ.

---

## 4. Situation & Job — User đang cố làm gì trong tình huống nào?

```
Tình huống bắt đầu: Một phiên học trực tuyến vừa kết thúc
→ User muốn hoàn thành việc gì: Xác định xem có học viên nào cần được hỗ trợ thêm trước buổi học tiếp theo
→ Hiện tại họ làm như thế nào: Dựa vào quiz cuối giờ, hỏi chung "Ai có thắc mắc gì không?", chờ học viên tự inbox
→ Điểm bắt đầu gặp vướng mắc: Nhóm học viên im lặng không tạo ra bất kỳ tín hiệu nào → Instructor không có cơ sở để hành động
```

**Mô tả Situation & Job:**

> Khi một phiên học trực tuyến kết thúc, Instructor đang cố xác định những học viên cần hỗ trợ thêm bằng cách dựa vào quiz cuối giờ, câu hỏi trên lớp và tin nhắn trực tiếp từ học viên.

**JTBD Hypothesis:**

> Khi phiên học kết thúc và tôi cần đảm bảo không ai bị tụt lại, tôi muốn nhanh chóng biết được học viên nào đang gặp khó khăn và họ kẹt ở đâu, để có thể can thiệp hỗ trợ đúng trọng tâm trước buổi học tiếp theo.

---

## 5. Pain — Viết các cách giải thích cạnh tranh

**Pain Hypothesis A:**

> Khi phiên học kết thúc, Instructor gặp khó khăn trong việc xác định học viên cần hỗ trợ vì **hoàn toàn thiếu tín hiệu từ nhóm học viên im lặng** (họ không hỏi, không chat, không bấm nút gì), dẫn đến việc Instructor mặc định cả lớp đã hiểu và bỏ lỡ thời điểm can thiệp sớm.

**Pain Hypothesis B — cách giải thích cạnh tranh:**

> Khi phiên học kết thúc, Instructor gặp khó khăn trong việc xác định học viên cần hỗ trợ vì **dù nhận thức được có người đuối, việc rà soát từng bài tập và tin nhắn để xác định ai kẹt ở đâu tốn quá nhiều thời gian**, dẫn đến việc Instructor chỉ hỗ trợ những ai chủ động tìm đến và phó mặc phần còn lại.

**Giả thuyết nhóm chọn để điều tra trước:** A

**Lý do chọn:** Hypothesis A là tiền đề sống còn của Solution Directive — hệ thống AI thu thập log hành vi vì giả định Instructor đang "mù thông tin". Nếu thực tế Instructor đã biết ai đuối (qua quiz, qua kinh nghiệm) nhưng chỉ thiếu thời gian (Hypothesis B), thì ném thêm một danh sách dài chỉ làm tăng gánh nặng vận hành chứ không giải quyết gốc rễ.

---

## 6. Evidence — Xác định điều cần tìm trước khi viết câu hỏi

| Cần kiểm tra | Evidence làm nhóm tin hơn | Evidence làm nhóm nghi ngờ hoặc bác bỏ |
| :--- | :--- | :--- |
| **Situation có thật** | Instructor kể được một buổi dạy gần đây mà họ muốn biết tình hình lớp sau giờ học; có bước rà soát học viên trong quy trình thực tế. | Instructor dạy xong là tắt máy; hoàn toàn không có thói quen hay nhu cầu ngó lại tình hình học viên. |
| **Pain có ý nghĩa** | Instructor bày tỏ bất lực vì không biết nhóm im lặng hiểu bài hay không; từng bị bất ngờ khi học viên nộp bài điểm liệt mà trên lớp không hề hỏi gì. | Instructor coi việc không hiểu là trách nhiệm của học viên; *"Ai không hiểu tự đi hỏi, lớn rồi."* |
| **Workaround tồn tại** | Instructor đã tự làm cách thủ công: soi bài quiz cuối giờ, nhắn tin hỏi ngẫu nhiên vài bạn, mở form ẩn danh, nhờ trợ giảng quan sát. | Instructor không làm bất cứ hành động nào ngoài việc chờ ai inbox thì trả lời. |
| **Consequence tồn tại** | Tỷ lệ dropout cao; học viên đánh giá khóa học thấp; Instructor phải dạy phụ đạo cuối kỳ để cứu vãn. | Lớp vẫn đạt 100% chỉ tiêu; không có hậu quả đáng kể về completion rate hay satisfaction. |
| **Pattern có lặp** | Tình trạng "học viên im lặng rồi tụt hậu" lặp đi lặp lại ở hầu hết các buổi học có kiến thức nặng. | Chỉ xảy ra ở 1–2 cá nhân cá biệt do lười, không phải vấn đề phổ quát. |

---

## Chốt Problem Hypothesis và park solution

**Problem Hypothesis nhóm mang sang Chặng 2:**

> Sau mỗi phiên học trực tuyến có kiến thức phức tạp, Instructor gặp khó khăn trong việc xác định và hỗ trợ kịp thời những học viên đang nghẽn kiến thức vì hoàn toàn thiếu tín hiệu từ nhóm học viên im lặng, dẫn đến việc bỏ lỡ thời điểm can thiệp sớm và khiến học viên có nguy cơ tụt hậu hoặc bỏ học.

**Điều gì phải đúng để giả thuyết đứng vững:**

1. Instructor thực sự coi việc học viên tụt hậu/bỏ học là trách nhiệm và nỗi đau của mình (Job tồn tại).
2. Tồn tại một "vùng mù thông tin" thực sự — Instructor không có cách nào nhận biết nhóm im lặng đang đuối (Pain tồn tại).
3. Nếu có thông tin kịp thời, Instructor sẵn sàng dành thời gian chủ động can thiệp (Hành vi thay đổi khả thi).

**Điều gì có thể khiến nhóm sửa hoặc bác bỏ giả thuyết:**

1. *"Tôi biết thừa ai đuối qua bài quiz 5 phút cuối giờ rồi."* → Bác bỏ Pain thiếu thông tin; dịch chuyển sang Hypothesis B.
2. *"Biết ai đuối nhưng không có thời gian nhắn tin cho từng người."* → Pain không phải thiếu visibility mà là quá tải vận hành.
3. *"Học viên lớn rồi phải tự chịu trách nhiệm, tôi chỉ dạy đúng giáo án."* → Bác bỏ toàn bộ Job.

---

**Solution Parking Lot**

| # | Hướng giải quyết có thể có | AI / Không sử dụng AI |
| :--- | :--- | :--- |
| 1 | AI Support Radar — phân tích log hành vi học tập để tạo danh sách ưu tiên hỗ trợ cho Instructor | AI |
| 2 | AI Tutor nhúng trực tiếp trên slide — gợi ý giải thích khi phát hiện Learner dừng đọc bất thường | AI |
| 3 | Bức tường ẩn danh (Padlet/Slido) — Learner vote khái niệm chưa rõ cuối buổi mà không lộ danh tính | Không sử dụng AI |
| 4 | Exit Ticket 1 phút — mỗi Learner ghi 1 câu "Điều khó hiểu nhất hôm nay" trước khi rời lớp | Không sử dụng AI |
| 5 | Lịch Office Hours cố định với TA — biến việc gặp trợ giảng thành thủ tục mặc định hàng tuần | Không sử dụng AI |

---

### ✅ Tự kiểm — CHECKPOINT 1

- [x] Lần theo đủ chuỗi: Solution → Change → Actor → Situation & Job → Pain → Evidence
- [x] Có hai cách giải thích cạnh tranh (Pain A: thiếu visibility / Pain B: quá tải vận hành)
- [x] Nói rõ điều gì có thể làm giả thuyết trở nên sai (3 câu nói cụ thể từ Instructor)
