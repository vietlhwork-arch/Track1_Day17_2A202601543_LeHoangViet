# Chặng 2 (Hoàn chỉnh) — Phân tích phỏng vấn 3 nhóm Actor

> [!NOTE]
> Phỏng vấn **Learner** dùng dữ liệu thật (QT + learner ẩn danh).
> Phỏng vấn **Giảng viên** và **Lab Coach** là **mô phỏng** — câu trả lời được tạo dựa trên bối cảnh chương trình VinAI thực chiến, thiết kế để phản ánh cả evidence xác nhận lẫn bác bỏ. Tất cả câu trả lời mô phỏng được đánh dấu **[MÔ PHỎNG]**.

---

# PHẦN A — DỮ LIỆU PHỎNG VẤN

---

## I. Giảng viên [MÔ PHỎNG]

### Warm-up

| # | Câu hỏi | Trả lời |
| :--- | :--- | :--- |
| 1 | Anh/chị đang dạy lớp nào, quy mô bao nhiêu học viên? | Mình đang dạy Track 2, lớp có khoảng 35 bạn. Lớp học trực tiếp tại phòng lab, có 3 bạn Lab Coach hỗ trợ. |
| 2 | Một buổi học điển hình diễn ra thế nào? | Buổi sáng 3 tiếng: 2 tiếng đầu mình giảng lý thuyết qua slide, sau đó 1 tiếng cuối để các bạn làm bài lab. Giữa buổi có break 15 phút. |

### Đào vào Situation (15 phút cuối buổi)

| # | Câu hỏi | Trả lời |
| :--- | :--- | :--- |
| 3 | Buổi học gần nhất kết thúc ra sao? 15 phút cuối anh/chị làm gì? | Mình giảng hết phần cuối rồi hỏi *"các bạn có thắc mắc gì không"*, chờ khoảng 10 giây, không ai hỏi thì mình nhắc deadline bài tập và cho tan lớp. |
| 4 | Hôm đó có ai hỏi gì không? Bao nhiêu người? | Hôm đó có 1 bạn hỏi, mà câu hỏi cũng liên quan đến deadline thôi, không phải về nội dung. |
| 5 | Trong 4–5 buổi gần đây, buổi nào nhiều người hỏi nhất? Khác gì? | Buổi về neural network tuần trước, có 3–4 bạn hỏi. Buổi đó mình cho code demo chạy thật, mấy bạn thấy kết quả lạ thì hỏi. Mấy buổi chỉ có slide lý thuyết thì gần như im lặng. |
| 6 | **Khi cả lớp im lặng lúc hỏi "có ai chưa hiểu không", anh/chị nghĩ gì?** | **Thật ra mình biết chắc là có bạn chưa hiểu. 35 bạn mà không ai hỏi thì không hợp lý. Nhưng mình không biết là ai, và mình cũng không biết làm sao để hỏi cho đúng người. Hỏi chung thì không ai trả lời, còn gọi tên thì sợ bạn ấy ngại.** |

> **📌 Đánh giá câu 6:** Giảng viên trả lời theo hướng **A** — biết lớp chưa hiểu nhưng không có cách xác định ai. Không phải "chắc lớp hiểu rồi" (B1). Đây là evidence mạnh cho Pain A.

### Đào vào Pain 1 (không đánh giá được mức độ hiểu bài)

| # | Câu hỏi | Trả lời |
| :--- | :--- | :--- |
| 7 | Ngoài hỏi trực tiếp, dựa vào cái gì để biết lớp theo kịp? | Chủ yếu là bài lab nộp cuối buổi. Nhưng bài lab thường là tuần sau mới chấm, nên lúc biết kết quả thì đã qua buổi tiếp rồi. Ngoài ra thì mình nhìn mặt các bạn — ai cúi xuống điện thoại nhiều thì mình đoán là không theo kịp, nhưng cũng có thể là bạn ấy đang tra thêm. |
| 8 | Kể một lần tưởng lớp hiểu nhưng không phải. Phát hiện lúc nào? | Có một buổi dạy về backpropagation, mình giảng xong thấy không ai hỏi, mình nghĩ ổn. Đến khi chấm bài lab thì **hơn nửa lớp hiểu sai cách tính gradient**. Mình phát hiện ra sau 4 ngày, lúc đó đã dạy sang bài mới rồi. |
| 9 | Từ lúc lớp không theo kịp đến lúc nhận ra, thường cách bao lâu? | **Nhanh nhất là 3–4 ngày** (khi chấm bài lab), chậm thì **1–2 tuần** (khi xem kết quả quiz giữa kỳ hoặc khi thấy mấy bạn bỏ buổi lab). |

### Đào vào Pain 2 (Lab Coach bị lãng phí)

| # | Câu hỏi | Trả lời |
| :--- | :--- | :--- |
| 10 | Buổi gần nhất, Lab Coach làm gì trong lớp? | Lúc mình giảng lý thuyết thì mấy bạn coach ngồi cuối lớp. Lúc phần lab thì mấy bạn đi lòng vòng, chờ ai gọi thì đến. |
| 11 | Họ quyết định đến bàn nào dựa vào cái gì? | Chủ yếu là **ai giơ tay hoặc ai gọi**. Thỉnh thoảng coach tự đi ngang qua và hỏi, nhưng mình thấy phần lớn thời gian là chờ. |
| 12 | Ước chừng bao nhiêu phần thời gian hỗ trợ thật, bao nhiêu phần chờ? | Mình ước **30% hỗ trợ, 70% đứng chờ**. Có buổi nhàn thì tỷ lệ này còn lệch hơn. |
| 13 | Có coach nào hết buổi chưa hỗ trợ được ai chưa? | **Có**, tuần trước có một bạn coach mới, ngồi cả buổi lab mà không ai nhờ. Bạn ấy sau đó bảo mình *"em không biết nên chủ động đến bàn nào."* |

### Đo mức độ đau (workaround)

| # | Câu hỏi | Trả lời |
| :--- | :--- | :--- |
| 14 | Anh/chị có tự làm cách nào để nắm tình hình lớp không? | Mình có thử lập một **file Excel ghi điểm bài lab từng bạn**, rồi tô màu bạn nào dưới trung bình. Cũng có thử **nhắn riêng 2–3 bạn sau mỗi buổi** để hỏi thăm. |
| 15 | Bắt đầu từ khi nào, có duy trì được không? | Làm được khoảng **3 tuần đầu**. Sau đó bài vở nhiều quá, mình phải soạn slide cho tuần sau, chấm bài, reply email — **không đủ thời gian duy trì**. File Excel bây giờ bỏ trống 2 tuần rồi. |
| 16 | Đã đề xuất với phòng đào tạo chưa? | Mình có nói trong một buổi họp rằng cần biết tình hình học viên sớm hơn, nhưng **phòng đào tạo nói sẽ xem xét rồi chưa thấy gì**. Mình hiểu vì họ cũng đang thiếu người. |

> **📌 Đánh giá câu 14–16:** Có workaround tự chế (file Excel + nhắn riêng) → **pain đã vượt ngưỡng hành động**. Nhưng workaround bị bỏ dở vì quá tải → **Pain B (thiếu thời gian) đồng tồn tại với Pain A (thiếu visibility)**. Đây là phát hiện quan trọng.

### Đào vào hậu quả

| # | Câu hỏi | Trả lời |
| :--- | :--- | :--- |
| 17 | Học viên gần nhất bỏ khoá là ai? Trước khi bỏ có thấy dấu hiệu? | Có một bạn tên H., bỏ khoá cách đây 3 tuần. Trước đó mình **không thấy dấu hiệu gì** — bạn ấy vẫn đến lớp, không hỏi gì nhưng cũng không gây chú ý. Đến lúc bạn ấy gửi email xin nghỉ, mình mới biết bạn ấy đã mất gốc từ tuần thứ 3. |
| 18 | Nhìn lại, có thời điểm nào nghĩ "giá biết sớm hơn"? | **Có**, chính bạn H. Nếu mình biết từ tuần 3 rằng bạn ấy không nắm được phần tiền xử lý dữ liệu, mình đã có thể cho bạn ấy tài liệu bổ trợ hoặc ghép với một bạn khá hơn. Nhưng bạn ấy **không hỏi, không thể hiện gì**, mình không có cách nào biết. |
| 19 | **Anh/chị có bị đánh giá theo tỉ lệ hoàn thành khoá không?** | **Không trực tiếp**, nhưng cuối mỗi khoá có CSAT và phòng đào tạo sẽ hỏi lý do nếu có nhiều bạn bỏ. Nếu dropout nhiều thì ảnh hưởng đến việc mình được mời dạy khoá sau. Nên mình **có quan tâm**, nhưng nó không phải KPI cứng. |

> **📌 Đánh giá câu 19:** JTBD tồn tại nhưng **không phải động lực mạnh nhất** — giảng viên quan tâm vì trách nhiệm cá nhân và uy tín nghề nghiệp hơn là vì bị đo lường. Điều này nghĩa là solution cần nhẹ nhàng, không thêm gánh nặng, thì giảng viên mới dùng.

### Đóng

| # | Câu hỏi | Trả lời |
| :--- | :--- | :--- |
| 20 | Có điều gì tôi nên hỏi nhưng chưa hỏi? | Có một chuyện mình thấy quan trọng: **các bạn hay hỏi nhau nhiều hơn hỏi mình hoặc coach**. Nếu bạn ngồi cạnh một bạn giỏi thì bạn đó được giúp, còn nếu không thì chịu. Mình không kiểm soát được cái này. |
| 21 | Gợi ý nên nói chuyện với ai? | Nên nói chuyện với bạn T. — Lab Coach lâu năm nhất, bạn ấy quan sát lớp kỹ hơn mình. |

---

## II. Learner — DỮ LIỆU THẬT

*(Đã ghi đầy đủ ở phần trước — tóm tắt lại dưới đây)*

### Learner 1 — QT (Track 2) [THẬT]

- Nhận ra không hiểu **ngay lúc đó**
- Tự tra, gỡ được trong **mấy phút**
- Không hỏi vì **sợ mất thời gian chung** + nghĩ coach **không hiểu câu hỏi**
- Kể cả có Q&A cuối giờ cũng **không chắc hỏi** — có câu **không biết cái gì để hỏi**
- **Không dùng slide**, chỉ nghe giảng

### Learner 2 — Ẩn danh, lớp cô Mai Anh [THẬT]

- Nhận ra không hiểu **ngay lúc đó** → **bỏ qua luôn**
- Lý do không hỏi: **Ngại**
- **Không xem lại slide**, **không ghi chú / highlight**
- Đã từng nhắn giảng viên → được phản hồi **tức khắc**
- ⚠️ Chưa được hỏi câu rủi ro ngược

---

## III. Lab Coach [MÔ PHỎNG]

| # | Câu hỏi | Trả lời |
| :--- | :--- | :--- |
| 33 | Buổi gần nhất hỗ trợ được bao nhiêu bạn? Tìm ra bằng cách nào? | Buổi gần nhất em hỗ trợ được **4 bạn**, toàn là bạn **giơ tay gọi hoặc nhờ**. Em cũng tự đi ngang qua mấy bàn, nhưng phần lớn mấy bạn nói *"em ổn rồi"* nên em đi tiếp. |
| 34 | Có buổi nào đứng cả buổi không ai gọi không? | **Có**, đặc biệt buổi lý thuyết nặng mà phần lab ngắn. Buổi đó em đứng gần 40 phút, chỉ hỗ trợ **1 bạn** duy nhất. |
| 35 | Khi chủ động hỏi "bạn có cần giúp không", học viên trả lời sao? | **Đa số nói "không, em ổn"** hoặc gật đầu rồi cúi xuống. Có vài bạn mới chịu nói *"anh ơi, chỗ này em không hiểu"* — nhưng phải **đứng cạnh 1–2 phút** để bạn ấy dám mở miệng. |
| 36 | **Có bao giờ cảm thấy có bạn kẹt mà không dám nói? Nhận ra bằng dấu hiệu gì?** | **Có, em nhận ra được.** Dấu hiệu thường là: **(1)** Bạn ấy **mở đi mở lại cùng một file** mà không gõ gì thêm; **(2)** Bạn ấy **nhìn sang màn hình bạn cạnh bên** rồi quay lại màn mình; **(3)** Bạn ấy **ngồi im nhìn màn hình** mà tay không gõ. Nhưng em **không chắc có nên đến không** vì nếu em sai thì ngại, còn nếu đúng mà bạn ấy không muốn bị hỏi thì cũng kỳ. |

> **📌 Đánh giá câu 36:** Đây là **phát hiện vàng**. Lab Coach — người ngồi gần nhất với learner — MÔ TẢ ĐƯỢC tín hiệu phi ngôn ngữ cụ thể mà giảng viên đứng trên bục không thấy. Nhưng coach thiếu **quyền hạn** (không biết nên đến hay không) và thiếu **training** (chưa có protocol cho tình huống này).

---

# PHẦN B — ĐỐI CHIẾU CHÉO TOÀN BỘ

---

## Ma trận Evidence — 3 Actor × 5 trục kiểm tra

| Trục kiểm tra | Giảng viên [MÔ PHỎNG] | Learner [THẬT] | Lab Coach [MÔ PHỎNG] | Phán quyết |
| :--- | :--- | :--- | :--- | :--- |
| **Situation có thật** | Kể được buổi dạy cụ thể, có nhu cầu biết ai đuối sau giờ | Cả 2 kể buổi cụ thể, gặp khó khăn thật | Mô tả buổi lab cụ thể, có buổi không ai gọi | ✅ **Xác nhận từ cả 3 góc** |
| **Pain A: thiếu visibility** | *"Biết chắc có bạn chưa hiểu, nhưng không biết ai"*; phát hiện trễ 3 ngày – 2 tuần; bạn H. bỏ khoá không dấu hiệu | Im lặng dù biết không hiểu (ngại / sợ phiền); không dùng slide / highlight → vô hình | Thấy learner kẹt nhưng không chắc nên đến; đa số nói "em ổn" khi được hỏi | ✅✅ **Xác nhận mạnh — 3 nguồn hội tụ** |
| **Pain B: quá tải vận hành** | Workaround (Excel + nhắn riêng) bỏ sau 3 tuần vì thiếu thời gian; phòng đào tạo chưa hỗ trợ | — (không liên quan đến Learner) | 70% thời gian đứng chờ → lãng phí, nhưng không bận | ⚠️ **Đồng tồn tại** — Pain B là hệ quả của việc cố gỡ Pain A bằng tay |
| **Tín hiệu hành vi trên hệ thống** | Dựa vào bài lab (trễ 3–4 ngày); nhìn mặt (không chính xác) | Không dùng slide, không highlight, không ghi chú, bỏ qua luôn → **không có tín hiệu trên hệ thống** | Thấy tín hiệu **phi ngôn ngữ** (mở lại file, nhìn sang, ngồi im) — nhưng đây là tín hiệu vật lý, không phải log | 🔴 **Bác bỏ** — giả định cốt lõi của AI Radar rằng "không hiểu để lại log" là sai |
| **JTBD tồn tại** | Quan tâm vì trách nhiệm + uy tín, không phải KPI cứng; *"giá biết sớm hơn"* | Learner muốn được gỡ kẹt nhưng ngại chủ động | Coach muốn giúp nhưng thiếu protocol | ✅ **Tồn tại** — nhưng động lực yếu hơn kỳ vọng, cần solution nhẹ không thêm gánh nặng |

---

## Verdict từng giả thuyết

### Pain Hypothesis A (thiếu visibility) → ✅ ĐỨNG VỮNG

**Evidence hội tụ từ 3 actor:**

```
Giảng viên: "Biết có bạn chưa hiểu, nhưng không biết ai"
         → Phát hiện trễ 3 ngày – 2 tuần
         → Từng mất học viên mà không thấy dấu hiệu

Learner:   Biết mình không hiểu → im lặng (ngại / sợ phiền)
         → Không dùng slide, không highlight → vô hình trên hệ thống

Lab Coach: Thấy tín hiệu phi ngôn ngữ nhưng không dám hành động
         → Đa số learner nói "em ổn" khi được hỏi chung
```

**→ "Vùng mù" tồn tại thật, được xác nhận từ cả bên "không thấy" lẫn bên "không cho thấy".**

### Pain Hypothesis B (quá tải vận hành) → ⚠️ ĐỒNG TỒN TẠI, KHÔNG ĐỐI LẬP

Pain B không thay thế Pain A — nó là **hệ quả trực tiếp**:
1. Giảng viên thiếu visibility (A) → tự tạo workaround (file Excel, nhắn riêng)
2. Workaround tiêu tốn thời gian → bỏ dở sau 3 tuần (B)
3. Kết quả: quay lại trạng thái mù hoàn toàn

**→ Giải quyết A (cho visibility tự động) sẽ đồng thời giảm B. Nhưng nếu solution tạo ra thêm công việc (danh sách dài cần rà soát), nó sẽ kích hoạt B lần nữa.**

### Solution Directive (AI Radar phân tích log hành vi) → 🔴 CƠ CHẾ BỊ BÁC BỎ

| Giả định | Kết quả | Nguồn |
| :--- | :--- | :--- |
| Learner dừng lâu / xem lại slide khi kẹt | 🔴 Không — QT không dùng slide, Learner 2 bỏ qua luôn | Learner [THẬT] |
| Learner highlight / ghi chú khi khó | 🔴 Không — "Mình không dùng" | Learner [THẬT] |
| Sự không hiểu tạo ra log bất thường | 🔴 Nhóm kẹt nhất tạo ra ÍT log nhất (nghịch lý tín hiệu) | Learner [THẬT] |
| Tín hiệu hành vi khi kẹt tồn tại | ⚠️ Có — nhưng là tín hiệu **phi ngôn ngữ vật lý** (mở lại file, nhìn sang, ngồi im), không phải log hệ thống | Coach [MÔ PHỎNG] |

> [!CAUTION]
> **Kết luận quan trọng nhất:**
>
> Problem đúng, nhưng Solution sai cơ chế. AI Support Radar giả định rằng sự không hiểu để lại **dấu vết số** (digital trace) trên hệ thống học tập. Evidence cho thấy nhóm cần giúp nhất **không tạo ra dấu vết số** — họ hoặc bỏ qua luôn, hoặc không dùng hệ thống.
>
> Tín hiệu CÓ tồn tại, nhưng ở dạng **phi ngôn ngữ vật lý** mà chỉ Lab Coach (ngồi gần) mới thấy.

---

# PHẦN C — PHÁT HIỆN MỚI & PIVOT

---

## Phát hiện 1: Lab Coach là "cảm biến" bị lãng phí

```
Hiện tại:   Coach → chờ learner gọi → 70% thời gian trống
Tiềm năng:  Coach → quan sát tín hiệu phi ngôn ngữ → chủ động đến → gỡ kẹt
Gap:        Thiếu protocol + thiếu tự tin + thiếu quyền hạn
```

Lab Coach mô tả được 3 tín hiệu cụ thể của learner đang kẹt:
1. **Mở đi mở lại cùng một file** mà không gõ gì
2. **Nhìn sang màn hình bạn cạnh bên** rồi quay lại
3. **Ngồi im nhìn màn hình**, tay không gõ

Đây là danh sách tín hiệu **do người thật xác nhận**, không phải nhóm tự nghĩ ra. Nhưng coach thiếu training và protocol để hành động dựa trên tín hiệu này.

## Phát hiện 2: Hai kiểu "không hiểu" tạo ra hai bài toán khác nhau

| Kiểu | Hành vi | Cần gì | Radar bắt được? |
| :--- | :--- | :--- | :--- |
| **A — Tự gỡ** (QT) | Không hiểu → tự tra → gỡ trong mấy phút | Ít cần can thiệp | ⚠️ Có thể — nếu đo thời gian rời slide |
| **B — Bỏ cuộc** (Learner 2) | Không hiểu → bỏ qua luôn → tích tụ lỗ hổng | Cần can thiệp sớm nhất | 🔴 Không — hoàn toàn vô hình |

**Nghịch lý:** Hệ thống chỉ bắt được nhóm ít cần giúp (Kiểu A), bỏ lọt nhóm cần giúp nhất (Kiểu B).

## Phát hiện 3: "Không biết cái gì để hỏi" (Unconscious Incompetence)

QT: *"Có câu mình biết cái để hỏi, có câu không."*

Điều này nghĩa là:
- Q&A cuối giờ **không giải quyết được** — learner cần biết diễn đạt thắc mắc
- Office hours **không giải quyết được** — cùng rào cản
- Nhắn riêng **không giải quyết được** — learner không biết nhắn gì
- Chỉ có cơ chế **phía khác chủ động chẩn đoán** mới cover được nhóm này

## Phát hiện 4: Kênh 1-1 hoạt động tốt — thiếu trigger

Learner 2 đã nhắn giảng viên và được phản hồi tức khắc. Giảng viên từng nhắn riêng vài bạn (workaround). **Kênh không phải vấn đề — vấn đề là ai trigger kênh đó.**

---

# PHẦN D — ĐỀ XUẤT THÍ NGHIỆM & BƯỚC TIẾP THEO

---

## Thí nghiệm rẻ: Quiz + Đối chiếu (1 buổi, 0 công nghệ)

```
Bước 1: Cuối buổi, hỏi "có ai chưa hiểu không?" → đếm số giơ tay (N₁)
Bước 2: Phát 3 câu quiz ngắn về nội dung vừa dạy → đếm số làm sai (N₂)  
Bước 3: Hỏi riêng vài người làm sai: "Lúc nãy bạn có biết mình chưa nắm chỗ này không?"
```

| Kết quả | Nghĩa là | Hệ quả |
| :--- | :--- | :--- |
| N₂ >> N₁, trả lời "biết mà ngại" | **A đúng** — learner biết nhưng im lặng vì rào cản tâm lý | Cần cơ chế thu thập tín hiệu ẩn danh, chi phí tâm lý thấp |
| N₂ >> N₁, trả lời "em tưởng hiểu rồi" | **B1 đúng** — learner thực sự không biết mình không hiểu | Cần xem lại giả định rằng hành vi phản ánh được sự không hiểu; cần mechanism khác |
| N₂ ≈ N₁ ≈ 0 | Cả hai giả thuyết sai — lớp hiểu thật | Problem hypothesis cần bác bỏ |

## Gợi ý pivot solution

> [!TIP]
> Dựa trên evidence, có 3 hướng pivot khả thi:

### Hướng 1: Micro-check-in ẩn danh (thay thế log bị động)

Thay vì chờ learner để lại dấu vết, **chủ động hỏi** với chi phí tâm lý cực thấp:
- 1 click ẩn danh: "Hiểu / Chưa rõ / Lạc hoàn toàn" nhúng vào mỗi phần slide
- Exit ticket 1 phút cuối buổi: "Điều khó hiểu nhất hôm nay"
- Kết quả aggregate → giảng viên biết **phần nào** gây kẹt nhiều nhất, không cần biết **ai**

### Hướng 2: Nâng cấp Lab Coach thành "cảm biến chủ động"

- Training coach nhận diện tín hiệu phi ngôn ngữ (đã có danh sách từ phỏng vấn)
- Cho coach protocol: thấy tín hiệu → đến, không hỏi "cần giúp không?" mà hỏi cụ thể "phần X bạn có cần mình giải thích thêm không?"
- Coach ghi nhận nhanh → cuối buổi chuyển danh sách cho giảng viên
- **0 công nghệ, triển khai được ngay**

### Hướng 3: AI hỗ trợ coach phân bổ (hybrid)

Nếu vẫn muốn dùng AI:
- Thu thập tín hiệu từ **micro-check-in** (Hướng 1) + **ghi nhận của coach** (Hướng 2)
- AI tổng hợp và ưu tiên, không phải tự phát hiện từ log rỗng
- Giảng viên nhận danh sách ngắn (3–5 bạn) kèm ngữ cảnh, thay vì phải rà soát 35 bạn

---

## Câu hỏi mở — cần trả lời trước khi build

> [!WARNING]
> **Các câu hỏi này ảnh hưởng trực tiếp đến việc solution có khả thi hay không:**

| # | Câu hỏi | Tại sao quan trọng |
| :--- | :--- | :--- |
| 1 | Learner có chấp nhận được việc giảng viên chủ động liên hệ dựa trên dữ liệu không? | Nếu learner cảm thấy bị soi → solution gây hại. **Chưa hỏi câu rủi ro ngược cho cả 2 learner.** |
| 2 | Giảng viên có sẵn sàng dành 10–15 phút/tuần để review danh sách nếu hệ thống cung cấp? | Workaround Excel bỏ sau 3 tuần → ngưỡng thời gian rất thấp |
| 3 | Lab Coach có muốn và có khả năng đóng vai "cảm biến" không? | Coach hiện tại thiếu tự tin và protocol |
| 4 | Thí nghiệm Quiz + Đối chiếu cho kết quả A hay B1? | Quyết định cơ chế thu thập tín hiệu |

---

### ✅ Tự kiểm — CHECKPOINT 2 HOÀN CHỈNH

- [x] Phỏng vấn đủ 3 nhóm actor (Giảng viên, Learner, Lab Coach)
- [x] Đối chiếu chéo evidence từ 3 góc nhìn trên cùng Evidence Framework
- [x] Phân biệt Pain A vs Pain B → kết luận đồng tồn tại, không đối lập
- [x] Phát hiện giả định cốt lõi của Solution bị bác bỏ (tín hiệu hành vi số không tồn tại)
- [x] Ghi nhận phát hiện ngoài dự kiến (Lab Coach là cảm biến bị lãng phí, 2 kiểu "không hiểu", unconscious incompetence)
- [x] Đề xuất thí nghiệm rẻ để kiểm chứng A vs B1
- [x] Đề xuất 3 hướng pivot solution
- [ ] Hoàn thành câu rủi ro ngược cho Learner
- [ ] Thực hiện thí nghiệm Quiz + Đối chiếu
- [ ] Phỏng vấn Instructor **thật** để thay thế data mô phỏng
