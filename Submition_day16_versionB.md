## 8. Final submission — Day 16 Package

```markdown
# Day 16 Submission 

## Members
- Nguyễn Phạm Trà My - 2A202600482

---

## 1. Idea reframed

Original idea:
> Xây dựng một website cho phép sinh viên dùng tranh luận/luyện tập với AI, lưu lại transcript và cung cấp report đánh giá sau mỗi phiên.

Reframed as a product opportunity:
> Sinh viên tham gia các cuộc thi debate cần luyện tập thường xuyên theo format chuẩn (motion, prep, round, feedback), nhưng thực tế họ bị giới hạn bởi số lượng buổi sparring, thiếu opponent phù hợp và feedback từ judge thường không đủ chi tiết hoặc không kịp thời. Việc luyện tập hiện tại phụ thuộc vào lịch CLB hoặc team, dẫn đến tần suất không ổn định và khó cải thiện nhanh trước các giải đấu. Các công cụ AI hiện tại chỉ hỗ trợ trả lời hoặc brainstorm ý tưởng, nhưng không mô phỏng được một round debate hoàn chỉnh cũng như không cung cấp feedback theo tiêu chí chấm điểm thực tế. Điều này tạo ra một khoảng trống rõ ràng cho một sản phẩm có thể tái hiện toàn bộ workflow debate (debate round → transcript → judge-style feedback). Chúng tôi tin rằng một AI được thiết kế như một opponent + judge, bám sát format thi đấu, có thể trở thành môi trường luyện tập on-demand giúp sinh viên luyện nhiều round hơn, nhận feedback rõ ràng hơn và cải thiện hiệu suất thi đấu.
---

## 2. Customer / Segment Card

- **Segment name:** Sinh viên tham gia các câu lạc bộ debate hoặc chuẩn bị đi thi debate competition (BP,WSDC, parliamentary...)
- **Operational context:** Họ luyện tập theo format debate (có motion, role, timing), thường sinh hoạt trong CLB hoặc team nhỏ, chuẩn bị cho các cuộc thi trong trường hoặc liên trường
- **Recurring workflow:** Nhận motion → chuẩn bị argument (prep time) → tham gia debate → nhận feedback từ judge/teammate → cải thiện cho round sau
- **Pain moment:** Không biết lập luận của mình có đủ logic hay không, thiếu người phản biện, không có feedback cụ thể sau khi luyện tập
- **Why now:** AI đã đủ khả năng tham gia hội thoại và phân tích nội dung, nhưng các công cụ hiện tại chưa được thiết kế theo workflow luyện tập tranh luận hoàn chỉnh
- **Access path:** CLB debate trong trường, cộng đồng debate (Facebook group, Discord), workshop/competition nội bộ

One-sentence description:
> Một sinh viên trong CLB debate cần luyện tập thường xuyên cho các giải đấu nhưng thiếu opponent phù hợp và không nhận được feedback đủ sâu sau mỗi round.

---

## 3. Need Map (2–3 needs)

### Need #1 (priority)
- **Statement (JTBD):** When I prepare for an upcoming debate competition round, I want to practice with a strong opponent in a realistic format, so I can identify weaknesses in my arguments before competing.
- **Current workaround:** Luyện sparring với bạn trong CLB hoặc tự nghĩ phản biện
- **Pain signal:** Debate competition yêu cầu luyện nhiều round thực tế, nhưng số buổi sparring bị giới hạn bởi lịch CLB
- **Evidence / proxy evidence:** Debate cần ít nhất 2 người → friction cao để bắt đầu luyện tập
- **Why underserved:** Không có hệ thống nào có thể mô phỏng opponent theo format debate competition (BP/WSDC) một cách on-demand

### Need #2
- **Statement (JTBD):** When I finish a debate round, I want detailed and structured feedback similar to a judge, so I can understand exactly what to improve.
- **Current workaround:** Nhận feedback từ judge hoặc teammate (không consistent, phụ thuộc người) hoặc phải tự đánh giá nếu không có người hỗ trợ
- **Pain signal:** Không rõ mình sai ở logic, structure hay delivery → cải thiện chậm 
- **Evidence / proxy evidence:** Feedback trong CLB hoặc competition thường ngắn, không đủ chi tiết để cải thiện sâu
- **Why underserved:** Không có tool nào đóng vai trò “judge + coach” để phân tích lập luận theo tiêu chí chấm điểm

### Need #3 (optional)
- **Statement (JTBD):** When I train over multiple debate sessions, I want my performance and feedback to be tracked over time, so I can see my progress and focus on recurring weaknesses.
- **Current workaround:** Ghi nhớ thủ công hoặc không theo dõi
- **Pain signal:** Không biết mình có tiến bộ hay không, lặp lại lỗi cũ qua nhiều round
- **Evidence / proxy evidence:** Feedback từ mỗi buổi luyện bị rời rạc, không có hệ thống lưu trữ hoặc tổng hợp
- **Why underserved:** Không có hệ thống nào kết nối feedback qua nhiều session thành một lịch sử tiến bộ rõ ràng

---

## 4. Strategy Statement

For [sinh viên tham gia các cuộc thi debate (CLB, competition như BP/WSDC)]
who struggle with [thiếu môi trường sparring đủ tốt, feedback không đủ sâu và không theo dõi được tiến bộ],
our product helps them [luyện tập và cải thiện chất lượng lập luận một cách có hệ thống]
through [hai mode chính:
- **Challenge mode:** mô phỏng debate round thực tế với AI opponent theo format thi đấu  
- **Coach mode:** phân tích transcript và đưa ra feedback chi tiết + gợi ý cải thiện theo tiêu chí judge],
unlike [việc luyện tập trong CLB hoặc chatbot thông thường],
because we can leverage [chúng tôi tái hiện toàn bộ workflow thi đấu (practice → feedback → coaching → tracking) thay vì chỉ cung cấp một phần rời rạc.].

---

## 5. Moat Hypothesis

**Moat mechanism:** [Domain-learning flywheel + data compounding]

If we deploy nhiều phiên luyện debate trong cùng context (debate competition), the following improve:
1. **Challenge mode (opponent)**
   - AI hiểu rõ hơn cách lập luận phổ biến trong debate (POI, rebuttal, framing)
   - Mô phỏng opponent ngày càng “giống người thật” và phù hợp trình độ user

2. **Coach mode (evaluation & feedback)**
   - Hệ thống đánh giá ngày càng sát với tiêu chí chấm điểm thực tế (content, style, strategy)
   - Feedback chuyển từ generic → actionable (chỉ rõ sửa như nào)

3. **Tracking & personalization**
   - Hệ thống học được pattern điểm yếu lặp lại của từng user
   - Đề xuất luyện tập cá nhân hóa (focus vào lỗi thường gặp)

Why competitors cannot easily replicate this:
>  Vì moat không nằm ở model AI chung mà nằm ở dữ liệu workflow-specific: transcript debate + feedback + progression theo thời gian.  
> Càng nhiều session, hệ thống càng hiểu sâu cách tranh luận và cách chấm điểm, tạo ra vòng lặp học (practice → feedback → improve) mà đối thủ khó replicate nếu không có dữ liệu tương tự.

---

## 6. Initial TAM / SAM / SOM view

| Layer | Estimate | Key assumptions | Confidence |
|---|---|---|---|
| TAM | Medium (global debate + public speaking learners) | Bao gồm sinh viên tham gia debate competition, CLB debate, và các nhóm luyện public speaking có format tranh luận | low |
| SAM | Small–Medium (student debate community) | Tập trung vào sinh viên đại học tham gia CLB debate, thi đấu nội bộ hoặc liên trường | medium |
| SOM | Small (early adopters trong 12–24 tháng) | Target ban đầu là sinh viên trong các CLB debate lớn, quen dùng AI tools và có nhu cầu luyện thi thường xuyên | medium |

---

**Estimation logic (high-level):**

- TAM dựa trên toàn bộ người học debate/critical thinking toàn cầu  
- SAM thu hẹp vào student debate ecosystem (CLB, competition)  
- SOM tập trung vào early adopters:  
  - active debaters  
  - có nhu cầu luyện thường xuyên  
  - có khả năng tiếp cận sản phẩm (online, AI-friendly)

---

**Top 3 unknowns requiring further research:**

1. Quy mô thực tế của cộng đồng debate student (theo khu vực/geography)  
2. Tần suất luyện tập (sessions/week) → ảnh hưởng trực tiếp đến usage  
3. Willingness to pay của nhóm debater (có coi đây là tool “must-have” không)

---

**Judgment:**

- [x] Worth pursuing now  
- [ ] Worth pursuing but not now (need to validate willingness to pay)  
- [ ] Not worth pursuing as currently framed

## 7. Positioning Note (2 sentences)

**What we are:**
> Một nền tảng luyện tập debate cho sinh viên thi đấu, mô phỏng round tranh luận thực tế và cung cấp feedback + coaching theo tiêu chí chấm điểm.

**What we are not / not yet:**
> Không phải chatbot hỏi đáp hay tool brainstorm ý tưởng, và chưa phải một chương trình đào tạo debate hoàn chỉnh thay thế CLB hoặc coach thật.

---

## 8. Self-assessment before Day 17
Trong 6 mắt xích (Idea → Customer → Need → Strategy → Moat → Market Size), mắt xích yếu nhất:

> Market Size và willingness to pay. Hiện tại mới dừng ở mức assumptions, chưa có dữ liệu thực tế về quy mô cộng đồng debater cũng như việc họ có sẵn sàng trả tiền cho sản phẩm này hay không.

---

Open questions chúng tôi muốn khám phá thêm ở Day 17:

1. Sinh viên debate có coi đây là một công cụ “must-have” trong quá trình luyện thi hay chỉ là “nice-to-have”?  
2. Người dùng sẵn sàng trả tiền cho phần nào: trải nghiệm sparring (challenge mode) hay phần feedback/coaching?  
3. Yếu tố nào quyết định việc họ quay lại sử dụng: chất lượng opponent, độ hữu ích của feedback hay khả năng theo dõi tiến bộ?
---
