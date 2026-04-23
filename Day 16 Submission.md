## 8. Final submission — Day 16 Package

```markdown
# Day 16 Submission 

## Members
- Nguyễn Phạm Trà My - 2A202600482

---

## 1. Idea reframed

Original idea:
> Xây dựng một website cho phép người sinh viên dùng tranh luận/luyện tập với AI, lưu lại transcript và cung cấp report đánh giá sau mỗi phiên.

Reframed as a product opportunity:
> Người học muốn cải thiện kỹ năng tranh luận nhưng thiếu môi trường luyện tập thực tế và phản biện liên tục. Hiện tại họ thường phải tự luyện (viết luận, suy nghĩ một chiều) hoặc phụ thuộc vào người khác để tranh luận, dẫn đến việc luyện tập không đều và khó đánh giá chất lượng lập luận. Các công cụ hiện có (chatbot thông thường) chỉ trả lời câu hỏi chứ không đóng vai trò là đối thủ tranh luận có cấu trúc, cũng không cung cấp feedback rõ ràng về logic, evidence hay cách lập luận. Điều này tạo ra cơ hội cho một sản phẩm nơi AI không chỉ “trả lời”, mà đóng vai trò như một đối thủ tranh luận + người đánh giá, giúp người dùng luyện tập theo flow hoàn chỉnh: debate → phản biện → phân tích → cải thiện.

---

## 2. Customer / Segment Card

- **Segment name:** Sinh viên / người học muốn cải thiện kỹ năng tranh luận và tư duy phản biện
- **Operational context:** Họ học trong môi trường có yêu cầu trình bày quan điểm (thuyết trình, viết luận, phỏng vấn, debate), nhưng không có môi trường luyện tập thường xuyên với phản hồi chất lượng
- **Recurring workflow:** Chọn một chủ đề → tự suy nghĩ hoặc viết lập luận → (hiếm khi) tranh luận với người khác → không có đánh giá rõ ràng về đúng/sai hoặc mạnh/yếu
- **Pain moment:** Không biết lập luận của mình có đủ logic hay không, thiếu người phản biện, không có feedback cụ thể sau khi luyện tập
- **Why now:** AI đã đủ khả năng tham gia hội thoại và phân tích nội dung, nhưng các công cụ hiện tại chưa được thiết kế theo workflow luyện tập tranh luận hoàn chỉnh
- **Access path:** Sinh viên công nghệ, người học online, người luyện IELTS/critical thinking — dễ tiếp cận qua web app

One-sentence description:
> Một sinh viên muốn luyện kỹ năng tranh luận nhưng không có đối thủ, không có coach và không nhận được feedback rõ ràng về chất lượng lập luận của mình.

---

## 3. Need Map (2–3 needs)

### Need #1 (priority)
- **Statement (JTBD):** When [I want to practice debating regularly], I want [an always-available system], so I can [train anytime without depending on others].
- **Current workaround:** Không luyện tập hoặc chỉ luyện tập khi có người phù hợp
- **Pain signal:** thời gian luyện tập không đều và không biết bản thân có tiến bộ hay không
- **Evidence / proxy evidence:** Debate cần ít nhất 2 người → friction cao để bắt đầu luyện tập
- **Why underserved:** Không có hệ thống nào đóng vai trò vừa là opponent vừa là environment luyện tập liên tục

### Need #2
- **Statement (JTBD):** When I finish a discussion or debate, I want structured feedback on my argument quality, so I can improve in the next attempt.
- **Current workaround:** Tự đánh giá hoặc nhận feedback rời rạc từ người khác
- **Pain signal:** Không biết sai ở logic, evidence hay cách trình bày → cải thiện chậm
- **Evidence / proxy evidence:** Feedback từ người thật không có format chuẩn, không repeatable
- **Why underserved:** Không có tool nào generate report phân tích sau khi tranh luận

### Need #3 (optional)
- **Statement (JTBD):** When I prepare arguments for a topic (e.g. essay, interview, debate), I want someone to challenge my reasoning, so I can identify weaknesses before presenting.
- **Current workaround:** Tự phản biện hoặc hỏi bạn bè (không consistent)
- **Pain signal:** Mất cơ hội thể hiện tốt (điểm thấp, fail interview, thuyết trình kém)
- **Evidence / proxy evidence:** Sinh viên thường chỉ luyện bằng viết luận → không có phản biện real-time
- **Why underserved:** Chatbot chỉ trả lời → không đóng vai trò “opponent” → thiếu phản biện hai chiều

---

## 4. Strategy Statement

For [sinh viên và người học cần cải thiện kỹ năng lập luận]
who struggle with [thiếu môi trường phản biện và feedback có cấu trúc],
our product helps them [luyện tập và cải thiện chất lượng lập luận một cách có hệ thống]
through [một AI đóng vai trò đối thủ tranh luận + hệ thống report phân tích sau mỗi phiên],
unlike [chatbot thông thường hoặc việc tự luyện,],
because we can leverage [chúng tôi xây dựng full workflow debate → transcript → evaluation thay vì chỉ trả lời câu hỏi].

---

## 5. Moat Hypothesis

**Moat mechanism:** [Domain-learning flywheel + data compounding]

If we deploy [N] times in [vertical/context], the following improve:
1. AI hiểu pattern lập luận phổ biến (logical fallacies, weak reasoning)
2. Report đánh giá ngày càng chính xác và hữu ích
3. Dataset transcript giúp refine cả opponent behavior và evaluation

Why competitors cannot easily replicate this:
> Vì moat nằm ở dữ liệu tranh luận thực tế + feedback loop giữa debate và evaluation. Model chung ai cũng có, nhưng dữ liệu workflow-specific (debate + scoring) tích lũy theo thời gian thì khó replicate nhanh.

---

## 6. Initial TAM / SAM / SOM view

| Layer | Estimate | Key assumptions | Confidence |
|---|---|---|---|
| TAM | Large (global learners market) | Bao gồm tất cả người học cần cải thiện kỹ năng lập luận: sinh viên, người đi làm, người luyện thi (IELTS, GMAT, phỏng vấn) | low |
| SAM | Medium (education & self-learning segment) | Tập trung vào sinh viên đại học, người học online và người luyện kỹ năng communication/critical thinking | medium |
| SOM | Small (early adopters trong 12–24 tháng) | Target ban đầu là sinh viên tech-savvy, người quen dùng AI tools và tự học | medium |

**Top 3 unknowns requiring further research:**
1. Mức độ willingness to pay cho sản phẩm luyện kỹ năng tranh luận  
2. Tần suất sử dụng thực tế (user có quay lại luyện thường xuyên không)  
3. Giá trị perceived của report (có đủ để giữ chân user không)

**Judgment:**
- [x] Worth pursuing now  
- [ ] Worth pursuing but not now (need to validate willingness to pay)
- [ ] Not worth pursuing as currently framed
---

## 7. Positioning Note (2 sentences)

**What we are:**
> Một nền tảng giúp người học luyện tập tranh luận với AI và nhận feedback có cấu trúc sau mỗi phiên.

**What we are not / not yet:**
> Không phải chatbot hỏi đáp thông thường, và chưa phải một chương trình đào tạo kỹ năng hoàn chỉnh.

---

## 8. Self-assessment before Day 17

Trong 6 mắt xích (Idea → Customer → Need → Strategy → Moat → Market Size), mắt xích yếu nhất:

> Market Size và willingness to pay (chưa có dữ liệu thực tế, mới dừng ở assumptions)

Open questions chúng tôi muốn khám phá thêm ở Day 17:
1. Người dùng sẵn sàng trả tiền cho phần nào: trải nghiệm debate hay report phân tích?
2. MVP nên tập trung vào challenge mode (đối thủ tranh luận) hay coach mode (feedback)?
3. Yếu tố nào quyết định retention: chất lượng phản biện của AI hay giá trị của report?

---
