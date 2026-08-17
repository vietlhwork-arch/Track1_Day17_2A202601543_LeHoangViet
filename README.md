# Track1_Day17_2A202601543_LeHoangViet

---

## 1. Thông tin cá nhân và nhóm

| Mục | Nội dung |
| :--- | :--- |
| **MHV** | 2A202601543 |
| **Họ tên** | Lê Hoàng Việt |
| **Tên nhóm** | JCungDuoc |
| **Thành viên** | Lê Hoàng Việt |
| **Case đã chọn** | Case C — AI Support Radar |

---

## 2. Problem Hypothesis Brief

### Solution Directive (gốc)

> Sau mỗi phiên học, hệ thống phân tích các tín hiệu như di chuyển giữa slide, dừng lâu hoặc xem lại, highlight và ghi chú, đánh dấu "Chưa hiểu", thay đổi câu trả lời, và nội dung trao đổi với AI Chat. AI tạo một Support Queue cho giảng viên, gồm: Những học viên có thể cần hỗ trợ; Phần nội dung mà họ có thể đang gặp khó khăn; Các tín hiệu dẫn đến nhận định đó; Một hành động hỗ trợ được đề xuất.

### Capability trung tính

> Nhận diện sớm những học viên đang gặp khó khăn trong việc hiểu bài sau một phiên học — kể cả khi họ không chủ động lên tiếng — và cung cấp đủ ngữ cảnh để người phụ trách giảng dạy quyết định có can thiệp hỗ trợ hay không.

### Chuỗi Change

```
Solution
  → Instructor nhìn thấy ai đang kẹt và kẹt ở đâu (Visibility)
  → Instructor chủ động liên hệ hỗ trợ đúng trọng tâm
  → Learner được gỡ kẹt kịp thời, giảm dropout (Outcome)
```

### Actor đã chọn điều tra

- **Instructor / Coach** — mắt xích yếu nhất trong chuỗi Change
- **Learner (đang kẹt)** — actor bị tác động, cần kiểm tra rủi ro ngược

### Pain Hypothesis

> **Pain A (chọn điều tra trước):** Sau mỗi phiên học, Instructor thiếu visibility hoàn toàn về nhóm học viên im lặng — họ không hỏi, không chat, không bấm nút gì — dẫn đến việc Instructor mặc định cả lớp đã hiểu và bỏ lỡ thời điểm can thiệp sớm.
>
> **Pain B (cạnh tranh):** Instructor biết có người đuối nhưng việc rà soát từng bài tập / tin nhắn để xác định ai kẹt ở đâu tốn quá nhiều thời gian → chỉ hỗ trợ ai chủ động tìm đến.

### Điều phải đúng để giả thuyết đứng vững

1. Instructor thực sự coi việc học viên tụt hậu / bỏ học là trách nhiệm và nỗi đau của mình
2. Tồn tại "vùng mù thông tin" thực sự — Instructor không có cách nhận biết nhóm im lặng đang đuối
3. Nếu có thông tin kịp thời, Instructor sẵn sàng chủ động can thiệp

*(Chi tiết đầy đủ: xem [checkpoint_1_problem_hypothesis.md](./checkpoint_1_problem_hypothesis.md))*

---

## 3. Conversation Guide — Phiên bản cuối (đã sửa sau luyện)

### Nguyên tắc chung

- Hỏi về **quá khứ cụ thể** ("buổi gần nhất", "lần gần nhất"), không hỏi tương lai hay ý kiến chung
- **Không làm lộ solution** — không nhắc đến AI, hệ thống, dashboard, hay radar
- **Không mớm** — dùng câu trung tính, để user tự chọn hướng trả lời
- Theo **câu chuyện thật** — khi user kể tình huống cụ thể, đào sâu bằng "rồi sao nữa?", "cụ thể là gì?"

---

### Bộ A — Giảng viên / Instructor

**Big 3 cần học:**
1. Instructor có thực sự thiếu visibility về nhóm im lặng không? (Pain A)
2. Instructor đã tự xoay xở bằng workaround nào chưa? (đo mức đau)
3. Hậu quả của việc phát hiện trễ là gì? (consequence)

#### Warm-up
1. Anh/chị đang dạy lớp nào, quy mô bao nhiêu học viên?
2. Một buổi học điển hình diễn ra thế nào, từ lúc bắt đầu đến kết thúc?

#### Situation (10–15 phút cuối buổi)
3. Buổi học gần nhất kết thúc ra sao? 15 phút cuối anh/chị làm gì?
4. Hôm đó có ai hỏi gì không? Bao nhiêu người?
5. Trong 4–5 buổi gần đây, buổi nào nhiều người hỏi nhất? Buổi đó khác gì?
6. **★ Khi cả lớp im lặng lúc hỏi "có ai chưa hiểu không", lúc đó anh/chị nghĩ gì?**

> *Ghi chú cho interviewer:* Câu 6 là câu đắt nhất. Nếu trả lời "chắc chúng nó ngại" → A. Nếu "chắc lớp hiểu rồi" → B1. **Không mớm**, chờ họ tự nói.

#### Pain 1 — Không đánh giá được mức hiểu bài
7. Ngoài hỏi trực tiếp, anh/chị dựa vào cái gì để biết lớp theo kịp?
8. Kể một lần tưởng lớp hiểu nhưng hoá ra không phải. Phát hiện lúc nào, bằng cách nào?
9. Từ lúc lớp không theo kịp đến lúc nhận ra, thường cách bao lâu?

#### Pain 2 — Lab Coach *(MỚI — thêm sau khi luyện)*
10. Buổi gần nhất, Lab Coach làm gì trong lớp?
11. Họ quyết định đến bàn nào dựa vào cái gì?
12. Ước chừng bao nhiêu phần thời gian hỗ trợ thật, bao nhiêu phần chờ?
13. Có coach nào hết buổi chưa hỗ trợ được ai chưa?

#### Workaround (đo mức đau)
14. Anh/chị có tự làm cách nào nắm tình hình lớp không — ghi chú, file riêng, hỏi riêng vài bạn?
15. *(Nếu có)* Bắt đầu từ khi nào, có duy trì được không? Nếu bỏ giữa chừng thì vì sao?
16. Đã đề xuất với phòng đào tạo về chuyện này chưa?

> *Ghi chú cho interviewer:* Câu 14–16 đo pain thật. Workaround tự chế = bằng chứng mạnh nhất. Không có workaround → dù than nhiều, mức đau vẫn dưới ngưỡng hành động.

#### Hậu quả
17. Học viên gần nhất bỏ khoá là ai? Trước khi bỏ, có thấy dấu hiệu gì không?
18. Nhìn lại, có thời điểm nào nghĩ "giá biết sớm hơn thì đã can thiệp được"?
19. **★ Anh/chị có bị đánh giá theo tỉ lệ hoàn thành khoá không?**

> *Ghi chú cho interviewer:* Câu 19 kiểm tra JTBD có tồn tại thật không. Nếu "không" → toàn bộ động lực hành động yếu đi rất nhiều.

#### Đóng
20. Có điều gì tôi nên hỏi nhưng chưa hỏi không?
21. Anh/chị gợi ý tôi nên nói chuyện tiếp với ai?

---

### Bộ B — Learner

**Big 3 cần học:**
1. Learner có nhận ra mình không hiểu ngay lúc đó không? (tách "ngại" khỏi "tưởng đã hiểu")
2. Khi kẹt, learner làm gì — và hành vi đó có để lại tín hiệu đo được không?
3. Learner có chấp nhận được việc bị chủ động tiếp cận không? (rủi ro ngược)

#### Bối cảnh
1. Kể lại buổi học gần nhất — bạn ngồi đâu, làm gì trong buổi?
2. Bạn thường ngồi học liền một mạch hay dừng lại nhiều lần?

#### Then chốt — tách "ngại" khỏi "tưởng đã hiểu"
3. Lần gần nhất bạn nghe giảng mà không hiểu là khi nào? Chuyện gì xảy ra sau đó?
4. **★ Lúc còn đang trong buổi học, bạn có nhận ra là mình chưa nắm phần đó không — hay về nhà mới biết?**
5. *(Nếu về nhà mới biết)* Lúc ngồi trong lớp bạn cảm thấy thế nào về phần đó?
6. *(Nếu biết ngay lúc đó mà không hỏi)* Điều gì làm bạn không hỏi?

> *Ghi chú cho interviewer:* Câu 4 là câu đắt nhất. Đặt ở dạng lựa chọn trung tính, không nghiêng bên nào. "Em tưởng em hiểu rồi" → B1 (tín hiệu hành vi không tồn tại để mà bắt). "Em biết mà ngại" → A.

#### Hành vi thật khi kẹt
7. Lần gần nhất bạn không hiểu bài, sau đó bạn làm gì? Tra ở đâu, hỏi ai?
8. Mất bao lâu bạn mới gỡ được? Có gỡ được không?
9. Bài tập gần nhất làm mất bao lâu? Có phần nào phải bỏ trống không?
10. *(Sửa sau luyện)* Khi gặp chỗ khó, bạn **thường làm gì tiếp theo** — đọc tiếp, quay lại slide, tra ngoài, hay bỏ qua?

> *Ghi chú cho interviewer — ĐÃ SỬA:* Câu 10 ban đầu hỏi "bạn có xem lại slide nhiều lần không?" → mớm hành vi cụ thể. Sửa thành câu mở để learner tự mô tả hành vi thật.

#### Kiểm tra tín hiệu *(SỬA — gộp lại, bỏ câu dẫn dắt)*
11. *(Sửa sau luyện)* Bạn có dùng ghi chú, highlight, hay bất kỳ cách nào đánh dấu trong lúc học không? Nếu có, dùng lúc nào?

> *Ghi chú cho interviewer — ĐÃ SỬA:* Ban đầu hỏi tách "có ghi chú không?" rồi "ghi lúc hiểu hay lúc không hiểu?" → dẫn dắt quá nhiều, gợi ý rằng người phỏng vấn đang quan tâm đến hành vi ghi chú cụ thể. Gộp thành 1 câu mở.

#### Kênh hỗ trợ hiện tại
12. Bạn có bao giờ nhắn hỏi giảng viên chưa? Lần gần nhất là khi nào, bao lâu thì được trả lời?
13. *(Nếu chưa bao giờ nhắn)* Điều gì khiến bạn không nhắn?
14. Bạn có nhờ Lab Coach bao giờ chưa? Kể lần gần nhất.
15. *(Nếu chưa nhờ)* Điều gì khiến bạn không nhờ?

#### Rủi ro ngược (BẮT BUỘC hỏi)
16. **★ Nếu giảng viên tự nhiên nhắn cho bạn "thầy thấy em có vẻ đang vướng phần X", bạn thấy thế nào?**
17. **★ Bạn có muốn biết hệ thống ghi nhận gì về việc học của mình không?**

> *Ghi chú cho interviewer:* Hai câu này kiểm tra liệu solution có gây hại nhóm nó định giúp. Learner bị tác động nhưng không có quyền quyết định. Phải hỏi trước khi build.

---

### Bộ C — Lab Coach *(MỚI — thêm sau khi luyện)*

**Big 3 cần học:**
1. Coach có thực sự nhàn rỗi không? Bao nhiêu thời gian hỗ trợ thật?
2. Coach có nhận ra learner kẹt bằng tín hiệu gì? (kiểm tra tín hiệu phi ngôn ngữ)
3. Khi chủ động đến hỏi, learner phản ứng sao?

1. Buổi gần nhất bạn hỗ trợ được bao nhiêu bạn? Tìm ra họ bằng cách nào?
2. Có buổi nào bạn đứng cả buổi mà không ai gọi không?
3. Khi bạn chủ động đến hỏi "bạn có cần giúp không", học viên thường trả lời sao?
4. **★ Có bao giờ bạn cảm thấy có bạn đang kẹt nhưng không dám nói không? Bạn nhận ra bằng dấu hiệu gì?**

> *Ghi chú cho interviewer:* Câu 4 rất giá trị — coach ở gần learner hơn giảng viên, họ quan sát được tín hiệu phi ngôn ngữ. Nếu mô tả được dấu hiệu cụ thể → danh sách tín hiệu do người thật xác nhận.

---

### Câu TUYỆT ĐỐI KHÔNG hỏi

| Câu | Lý do |
| :--- | :--- |
| "Nếu có hệ thống tự phát hiện học viên đang kẹt thì anh/chị thấy sao?" | Hỏi về tương lai + mớm solution → ai cũng gật |
| "Anh/chị có muốn một danh sách học viên cần hỗ trợ không?" | Câu hỏi mà không ai trả lời "không" |
| "Bạn có ngại hỏi trong lớp không?" | Mớm sẵn A, khoá luôn khả năng phát hiện B1 |
| "Việc không biết ai đang kẹt có phải vấn đề lớn không?" | Đặt sẵn kết luận vào câu hỏi |

---

### Thay đổi so với bản trước luyện

| # | Thay đổi | Lý do (dựa trên trải nghiệm luyện) |
| :--- | :--- | :--- |
| 1 | **Thêm Bộ C — Lab Coach** | Khi luyện phỏng vấn Learner, phát hiện learner nhắc đến coach ("không thật sự hiểu câu hỏi của mình") → cần kiểm chứng từ góc coach. Coach cũng là người gần learner nhất, có thể thấy tín hiệu mà giảng viên bỏ lỡ. |
| 2 | **Sửa câu hỏi slide** (Bộ B, câu 10) | Ban đầu: "Khi gặp chỗ khó, bạn có xem lại slide đó nhiều lần không?" → mớm một hành vi cụ thể, learner chỉ cần trả lời có/không. Sửa thành câu mở: "bạn thường làm gì tiếp theo?" để learner tự mô tả hành vi thật. |
| 3 | **Gộp 2 câu ghi chú/highlight** thành 1 (Bộ B, câu 11) | Ban đầu hỏi tách: "có ghi chú không?" rồi "ghi lúc hiểu hay lúc không hiểu?" → dẫn dắt quá nhiều, gợi ý interviewer đang quan tâm đến hành vi ghi chú. Gộp lại và để mở. |
| 4 | **Thêm ghi chú "★" cho câu đắt nhất** mỗi bộ | Khi luyện, interviewer dễ bị cuốn theo mạch hỏi mà quên câu then chốt. Đánh dấu ★ để nhắc dừng lại, chờ, và đào sâu. |
| 5 | **Thêm Big 3 đầu mỗi bộ** | Khi luyện, interviewer đôi khi hỏi hết bảng mà quên mục đích. Big 3 giúp quay lại "mình đang cần học gì từ người này". |

---

## 4. Practice Reflection

### Câu hỏi nào đã giúp user kể một tình huống cụ thể?

> **"Lần gần nhất bạn nghe giảng mà không hiểu là khi nào? Chuyện gì xảy ra sau đó?"** — Câu này buộc learner quay lại một sự kiện cụ thể thay vì nói chung chung. Cả QT và Learner 2 đều kể được tình huống thật: QT tự tra trong mấy phút, Learner 2 bỏ qua luôn. Từ câu trả lời cụ thể này mới đào tiếp được lý do (sợ phiền / ngại) và hành vi (tự tra / bỏ qua) — thay vì chỉ nhận được "ừ thì cũng có lúc không hiểu".

### Chỗ nào mình cần làm tốt hơn ở lần phỏng vấn thật?

> **Quên hỏi câu rủi ro ngược cho cả 2 learner.** Đây là câu bắt buộc trong bộ hỏi (câu 16–17 Bộ B) nhưng khi luyện, mình bị cuốn theo mạch câu chuyện về hành vi khi kẹt mà quên đóng phần rủi ro ngược. Nếu không hỏi câu này, mình sẽ build solution mà không biết learner có cảm thấy bị soi hay không — gây hại đúng nhóm mình định giúp.
>
> Ngoài ra, khi Learner 2 nói "bỏ qua luôn", mình đã không đào tiếp: "Rồi sau đó sao? Bài tập có bỏ trống không? Có bao giờ quay lại không?" — bỏ lỡ cơ hội hiểu hậu quả thật của việc bỏ qua.

### Sau khi luyện, nhóm đã sửa Conversation Guide ở đâu và vì sao?

> **5 thay đổi cụ thể** (chi tiết ở bảng trên):
>
> 1. **Thêm Bộ C cho Lab Coach** — vì phỏng vấn learner bất ngờ cho thấy coach là actor quan trọng (QT nói coach "không hiểu câu hỏi", Learner 2 vừa nghe vừa làm việc riêng mà coach không phát hiện).
> 2. **Sửa câu slide** từ câu đóng (có/không) thành câu mở — vì câu cũ mớm hành vi "xem lại slide" mà thực tế learner không làm.
> 3. **Gộp câu ghi chú/highlight** — vì hỏi tách ra dẫn dắt quá rõ rằng interviewer quan tâm đến hành vi này.
> 4. **Thêm đánh dấu ★ cho câu đắt nhất** — vì khi luyện dễ cuốn theo mạch mà quên câu then chốt.
> 5. **Thêm Big 3 đầu mỗi bộ** — vì khi luyện đôi khi hỏi hết danh sách mà quên mục đích.

---

## 5. AI Support Log

### AI đã giúp gì?

| Bước | AI hỗ trợ |
| :--- | :--- |
| Checkpoint 1 — Problem Framing | Hỗ trợ cấu trúc chuỗi Solution → Change → Actor → Situation & Job → Pain → Evidence. AI giúp viết 2 Pain Hypothesis cạnh tranh (A: thiếu visibility, B: quá tải vận hành) và xác định điều gì có thể bác bỏ giả thuyết. |
| Checkpoint 2 — Interview Analysis | Tổng hợp evidence từ 2 bài phỏng vấn Learner thật, đối chiếu với Evidence Framework. AI phát hiện "nghịch lý tín hiệu" — learner càng đuối càng ít dấu vết. |
| Mô phỏng phỏng vấn Instructor & Coach | Tạo câu trả lời mô phỏng cho Giảng viên (21 câu) và Lab Coach (4 câu) dựa trên bối cảnh VinAI thực chiến, để có đủ data đối chiếu chéo 3 actor. |
| Conversation Guide revision | Hỗ trợ đề xuất 5 thay đổi cho Guide dựa trên evidence từ phỏng vấn luyện. |

### Điểm AI sai / hời hợt và đã tự sửa

| Vấn đề | Cách đã sửa |
| :--- | :--- |
| **Phỏng vấn Instructor & Lab Coach là mô phỏng, không phải data thật.** Điều này nghĩa là evidence từ 2 nhóm actor này chưa được kiểm chứng và có thể sai hoàn toàn. | Đánh dấu rõ **[MÔ PHỎNG]** ở tất cả câu trả lời giả lập. Tách biệt kết luận dựa trên data thật (Learner) và data mô phỏng (Instructor, Coach). Ghi nhận rằng phỏng vấn Instructor thật vẫn cần thực hiện. |
| **AI ban đầu chưa nhấn mạnh việc thiếu câu rủi ro ngược** — phân tích xong mới bổ sung vào phần câu hỏi mở. | Trong bản sửa Conversation Guide, đánh dấu câu rủi ro ngược là **BẮT BUỘC** với ★, đặt ở cuối mỗi bộ để interviewer không bỏ sót. |
| **AI đề xuất pivot quá sớm** (micro-check-in, nâng cấp coach) khi evidence mới chỉ từ 2 learner + data mô phỏng. | Nhận thức rằng pivot chỉ nên là "gợi ý tiềm năng" chứ không phải kết luận. Cần thêm phỏng vấn thật và thí nghiệm Quiz + Đối chiếu để có đủ cơ sở. |

---

## Tham chiếu

- [checkpoint_1_problem_hypothesis.md](./checkpoint_1_problem_hypothesis.md) — Chặng 1: Đặt giả thuyết
- [checkpoint_2_interview_analysis.md](./checkpoint_2_interview_analysis.md) — Chặng 2: Phân tích phỏng vấn
- [interview/notes.md](./interview/notes.md) — Ghi chú phỏng vấn lượt interviewer
- [interview/recording.m4a](./interview/recording.m4a) — File bản ghi âm phỏng vấn
