# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên:Nguyễn Quang Hữu
- Mã học viên:2A202602756
- Nhóm: A1-Nhóm 1
- Candidate problem nhóm chọn: Tổng hợp vị trí việc làm từ nhiều nguồn, loại bỏ tin tuyển dụng trùng lặp và tìm thêm trên trang tuyển dụng chính thức của doanh nghiệp

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Đưa ra 8 problems về quy trình xử lý lỗi phần mềm | Nhóm có thêm 3 Problem Cards rõ workflow và thời gian |
| Pitch Problem Card | Pitch bài viết báo cáo chi tiết về lỗi đã sửa | Bài được đưa vào shortlist và xếp thứ hai |
| Challenge bài của bạn khác | Hỏi cách đo tỷ lệ tin trùng và giới hạn lấy dữ liệu tuyển dụng | Nhóm thu hẹp nguồn dữ liệu và giữ bước người dùng kiểm tra |
| Gom trùng / cluster | Hỗ trợ gom 15 candidates thành 4 cụm | Nhóm nhìn rõ các ý trùng và chọn được 3 bài vào shortlist |
| Chọn candidate problem | Điều phối chấm điểm theo 7 tiêu chí | Nhóm thống nhất chọn candidate #7 |
| Validation / research | Cùng kiểm tra số liệu và link nguồn | Nhóm tách rõ bằng chứng và giả định cần thử nghiệm |
| Workflow nhóm | Rà lại bước nghẽn và thời gian trước/sau | góp phần Workflow giảm kỳ vọng từ 60–90 phút xuống dưới 30 phút |
| Problem Statement | Góp ý metric và boundary | Có mục tiêu đo được và giới hạn không tự nộp hồ sơ |
| Rule / Workflow / Agent | Lập luận chọn Workflow thay vì Agent | Nhóm dùng Rule cho phần rõ ràng, AI hỗ trợ đọc hiểu và người dùng review |
| Decision | Góp ý chọn Go với pilot nhỏ | Có dữ liệu thử nghiệm, metric và điều kiện rollback rõ |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Tôi điều phối việc chấm điểm và giúp nhóm giữ bài toán ở phạm vi có thể kiểm soát. Dấu tay rõ nhất của tôi là làm rõ metric, giới hạn dữ liệu và bước người dùng kiểm tra trước khi chốt danh sách việc làm.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Mở rộng góc nhìn sau khi đã tự liệt kê các vấn đề của Backend Dev | Gợi ý thêm pain point từ phía người nhận kết quả (Tester thiếu thông tin tái hiện, PM khó hiểu code) | Gợi ý các ý tưởng quá rộng và số đo mơ hồ kiểu "tốn nhiều thời gian" | Tự bổ sung các mốc thời gian định lượng cụ thể (10–30 phút/lần) dựa trên thực tế công việc |
| Problem Card | Đóng vai PM để phản biện điểm nghẽn và tính khả thi | Chỉ ra lỗ hổng: AI không thể nắm hết ngữ cảnh nghiệp vụ nếu chỉ nhìn commit diff | AI có xu hướng khuyên dùng Agent tự động tạo ticket và assign người gây lỗi | Hạ cấp giải pháp xuống Workflow, bổ sung ranh giới con người kiểm tra để tránh xung đột nội bộ |
| Workflow | Gợi ý phân tách các bước Before/After và cú pháp luồng | Giúp hình dung rõ các điểm chuyển giao (handoff) giữa Dev và Tester | AI tự động bỏ qua bước fallback khi AI trích xuất sai | Tự thêm nhánh xử lý dự phòng (fallback) quay về quy trình thủ công nếu AI sinh sai dữ liệu |
| Research | Tìm kiếm các giải pháp, công cụ và tiện ích tương tự trên thị trường | Liệt kê nhanh các công cụ như Teal, Huntr, Simplify | Đưa ra các số liệu tính năng mà không dẫn link chính thức để kiểm chứng | Trực tiếp tra cứu tài liệu và điều khoản LinkedIn để xác thực tính pháp lý và giới hạn kỹ thuật |
| Problem Statement | Kiểm tra xem các trường mục có bị lẫn lộn giữa vấn đề và giải pháp không | Phát hiện mục tiêu đo lường ban đầu bị thiếu chỉ số chất lượng đề xuất | AI diễn giải văn phong quá hoa mỹ và làm loãng ranh giới (Boundary) | Tự rút gọn, thiết lập ranh giới cứng: dứt khoát không cào dữ liệu trái phép và không tự nộp CV |
| Rule / Workflow / Agent | Phản biện xem Rule đã giải quyết được bao nhiêu % bài toán | Chỉ ra các trường hợp Rule đơn giản có thể giải quyết tốt (chuẩn hóa URL, lọc từ khóa) | AI thiên vị việc dùng Agent tự hành để xử lý toàn bộ quy trình | Quyết định chọn Workflow kết hợp Rule và AI, giữ con người làm chốt chặn cuối cùng |
| Decision | Liệt kê các rủi ro tiềm ẩn trước khi quyết định Go / Not Yet / No-Go | Nhắc nhở về rủi ro dữ liệu đầu vào chưa được kiểm chứng đầy đủ | Đưa ra kết luận Go quá dễ dãi mà không kèm điều kiện thử nghiệm an toàn | Đưa ra quyết định Go có điều kiện: chỉ thử nghiệm quy mô nhỏ bán thủ công trên tập dữ liệu sạch |

> Nếu phase nào không dùng AI, ghi `Không dùng` và vì sao tự làm.

---

## 3. Reflection câu hỏi mở

Chọn 3-4 câu trong 6 câu dưới để viết thành đoạn 8-12 câu (không trả lời bullet 1 dòng):
- Tôi học được gì khi nghe top 3 problems của các bạn khác?
- Nhóm có lúc nào bị solution-first, đòi làm Agent cho ngầu không?
- Tôi có thay đổi ý kiến sau khi bị challenge không, vì sao đổi?
- Tôi đóng góp gì thật sự vào artifact cuối, phần nào có dấu tay của tôi?
- Điều khó nhất khi viết Problem Statement là gì, metric hay boundary?
- Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?


**Reflection:**

Khi lắng nghe top 3 problems của các bạn khác, tôi nhận ra vấn đề tìm việc của sinh viên (Candidate #7) có tác động lớn hơn và tần suất gây ức chế cao hơn nhiều so với quy trình nội bộ của dev. Nhóm tôi ban đầu cũng có lúc bị cuốn vào tư duy solution-first, muốn dựng ngay một Agent tự động cào mọi website tuyển dụng và nộp CV tự động. Tuy nhiên, sau khi đối chiếu với rủi ro pháp lý từ chính sách cấm bot của LinkedIn, tôi và nhóm đã dừng lại để chọn mô hình Workflow bán tự động có con người kiểm soát. Bản thân tôi cũng thay đổi nhận thức sau khi bị nhóm challenge về tính khả thi của việc dùng AI tóm tắt code: tôi nhận ra chỉ cần chuẩn hóa lại template báo cáo cho PM là đã giảm được phần lớn thời gian mà không cần lạm dụng AI. Điều khó nhất khi viết Problem Statement chính là xác định Boundary (làm gì và không làm gì) để tránh phạm vi bị phình to. Ngoài ra, việc xác định metric đo lường chất lượng đề xuất của AI cũng rất thử thách vì tính phù hợp mang tính chủ quan của từng người tìm việc. Dấu tay rõ nhất của tôi là việc giữ vai trò Facilitator, kiên quyết bổ sung bước người dùng kiểm tra bắt buộc trước khi chốt danh sách việc làm rút gọn. Nếu được làm lại, tôi sẽ challenge nhóm quyết liệt hơn ở khâu validation. Tôi cũng sẽ yêu cầu phỏng vấn sâu người dùng thật thay vì chỉ dựa vào số liệu khảo sát mô phỏng.

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [X] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [X] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1)
- [X] Nhóm có nhật ký hội tụ từ candidates về 1 bài
- [X] [15đ] Nhóm có workflow trước/sau
- [X] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ
- [X] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent
- [X] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ
- [X] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [X] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI
