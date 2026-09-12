# 02 — Group Problem Statement (Bản nộp nhóm)

> Làm chung 1 bản, mỗi thành viên copy vào repo cá nhân. Đi theo Phase 3 → 6 trong `01-worksheet.md`. Nhóm chỉ chọn **candidate problem** ở Phase 3, viết Problem Statement sau khi validate + vẽ workflow.

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm (VD: facilitator, workflow, research, writer) |
|-----|-----------|-------------|---------------------------------------------------------------|
| 1 | Nguyễn Nhật Thăng | 2A202602727 | Workflow |
| 2 | Nguyễn Quang Hữu | 2A202602756 | Facilitator |
| 3 | Nguyễn Minh Quyền | 2A202602438 | research |
| 4 | Đào Gia Bảo | 2A202602793 | Writer |
| 5 | Vương Việt Hoàng | 2A202602528 | research |

**Candidate problem nhóm chọn (1 câu):**

Sinh viên mới tốt nghiệp mất nhiều thời gian tổng hợp vị trí việc làm từ nhiều nguồn, loại bỏ tin tuyển dụng trùng lặp, tìm thêm trên trang tuyển dụng chính thức của doanh nghiệp và đánh giá mức độ phù hợp trước khi tạo danh sách rút gọn để ứng tuyển.

---

## Phase 3 — Group Convergence: từ 15 candidates về 1

### 3.1. Trình bày top 3 mỗi người (mỗi candidate 1-2 phút)

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh của nhóm |
|---|---|---|---|---|---|
| 1 | Nguyễn Quang Hữu | Viết báo cáo thủ công chi tiết về các lỗi đã sửa | Lập trình viên backend | Sau khi sửa lỗi phải tự tổng hợp nguyên nhân, phần code thay đổi, cách sửa và kết quả để viết báo cáo | Workflow rõ, lặp lại và tốn thời gian; AI có thể hỗ trợ tổng hợp từ phần code thay đổi và commit, nhưng cần xác định báo cáo chỉ cần nội dung kỹ thuật hay cả bối cảnh nghiệp vụ |
| 2 | Nguyễn Quang Hữu | Truy tra lịch sử Git/commit để tìm ra dev gây ra bug gốc | Backend Developer / Dev team | Phải lần theo nhiều commit, diff và lịch sử thay đổi để xác định thay đổi nào có khả năng gây ra bug | Workflow khá rõ và có tiềm năng tự động hóa; tuy nhiên kết luận dựa trên Git history có thể không đủ tin cậy và không nên dùng để quy trách nhiệm trực tiếp |
| 3 | Nguyễn Quang Hữu | Tạo thủ công ticket báo cho tester sau khi đã sửa code | Lập trình viên backend và kiểm thử viên | Sau khi sửa lỗi phải chuyển thông tin từ quá trình tìm/sửa lỗi sang ticket, đặc biệt là mô tả thay đổi và các bước kiểm thử/tái hiện | Vấn đề lặp lại, đầu vào tương đối có cấu trúc và dễ tự động hóa; điểm khó là phải tạo được các bước kiểm thử đủ chính xác cho kiểm thử viên |
| 4 | Nguyễn Nhật Thăng | Tự tổng hợp tiến độ từ 4 thành viên vì báo cáo rải rác qua chat, không theo định dạng | Nhóm trưởng | Thông tin tiến độ nằm rải rác trong nhiều tin nhắn và không theo định dạng thống nhất nên phải đọc, đối chiếu và tổng hợp thủ công | Candidate tốt vì người gặp vấn đề và workflow rõ, xảy ra hằng tuần và tác động cộng dồn; cần đo chính xác thời gian tổng hợp để có số liệu ban đầu |
| 5 | Nguyễn Nhật Thăng | Thành viên hay hỏi lại nhiệm vụ/thời hạn dù đã giao trong nhóm chat | Nhóm trưởng và các thành viên trong nhóm | Nhiệm vụ và thời hạn bị chìm trong lịch sử chat, khiến thành viên khó tìm lại thông tin đã giao | Vấn đề ảnh hưởng nhiều người và có thể đo bằng số lần hỏi lại; cần kiểm chứng nguyên nhân gốc là thông tin phân tán hay cách giao việc chưa đủ rõ |
| 6 | Nguyễn Nhật Thăng | Rà soát định dạng/cấu trúc file trước khi nộp bài nhóm | Thành viên phụ trách nộp bài / cả nhóm | Trước khi nộp phải kiểm tra thủ công định dạng, cấu trúc và yêu cầu của file do nhiều thành viên cùng chỉnh sửa | Điểm nghẽn cụ thể, dễ đo trước/sau và dễ thử Rule/Workflow; cần xác định vấn đề có thể giải quyết đơn giản bằng mẫu và danh sách kiểm tra hay không |
| 7 | Đào Gia Bảo | Tổng hợp vị trí việc làm từ nhiều nguồn, loại bỏ tin tuyển dụng trùng lặp và tìm thêm trên trang tuyển dụng chính thức của doanh nghiệp | Sinh viên mới tốt nghiệp đang tìm việc | Phải chuyển qua nhiều nguồn, đọc mô tả công việc, nhận diện tin trùng và đánh giá mức phù hợp trước khi tạo danh sách rút gọn | Tốn thời gian nhất, khoảng 60–90 phút/phiên; có tiềm năng cho tự động hóa và AI so sánh mức phù hợp, nhưng cần thêm dữ liệu về tần suất, tỷ lệ tin trùng và giới hạn thu thập dữ liệu tự động |
| 8 | Đào Gia Bảo | Chỉnh sửa CV cho phù hợp với yêu cầu của từng công việc | Người đang tìm việc | Phải đọc mô tả công việc, xác định yêu cầu/từ khóa rồi đối chiếu thủ công với kinh nghiệm, kỹ năng và dự án trong CV | Cách dùng AI khá rõ với đầu vào/đầu ra xác định và có người kiểm tra; cần tránh AI bịa thêm năng lực và chưa chắc việc điều chỉnh CV làm tăng tỷ lệ được mời phỏng vấn bao nhiêu |
| 9 | Đào Gia Bảo | Ghi lại công ty, vị trí và trạng thái hồ sơ xin việc trên Excel/Google Sheets | Người đang tìm việc | Thông tin nằm rải rác giữa trang tuyển dụng, email và bảng theo dõi nên phải sao chép và cập nhật trạng thái thủ công | Rất lặp lại và dễ tự động hóa; mỗi lần chỉ tiết kiệm vài phút nên cần đo số hồ sơ nộp mỗi tuần để đánh giá tổng tác động |
| 10 | Nguyễn Minh Quyền | Phải đọc nhiều email/tin nhắn để tìm thông tin quan trọng giữa thư rác và quảng cáo | Người dùng email/tin nhắn | Phải đọc, phân loại, loại thư rác rồi mới tìm và tổng hợp nội dung quan trọng | Vấn đề phổ biến và AI phù hợp cho phân loại/tóm tắt; cần đo số lượng mỗi ngày và kiểm chứng độ chính xác để tránh bỏ sót thông tin quan trọng |
| 11 | Nguyễn Minh Quyền | Phải thường xuyên lập và điều chỉnh thời gian biểu theo lịch học, deadline và công việc cá nhân | Sinh viên / người đi làm | Phải tự thu thập deadline, phát hiện conflict và sắp xếp lại lịch khi có thay đổi | Có tiềm năng nhưng problem còn rộng; cần xác định bottleneck chính là nhập lịch, cập nhật hay xử lý conflict trước khi chọn solution |
| 12 | Nguyễn Minh Quyền | Thành viên trong nhóm khó theo dõi tiến độ và không biết ai đang phụ trách công việc nào | Thành viên nhóm và trưởng nhóm | Thông tin phân công/tiến độ chưa tập trung nên phải hỏi lại để biết người phụ trách và trạng thái công việc | Vấn đề ảnh hưởng cả nhóm và workflow rõ; tuy nhiên khá gần candidate #4/#5 nên cần đo số lần hỏi lại, số lần trễ hạn và xác nhận đây là khó khăn chung |
| 13 | Vương Việt Hoàng | Tìm lại link bài giảng, câu lệnh AI và tài liệu bị trôi trong Zalo/Slack/Discord | Sinh viên / người học | Phải tìm kiếm hoặc cuộn lại hàng trăm tin nhắn để tìm đúng tài liệu | Vấn đề rõ, xảy ra 3–4 lần/tuần và mất 10–15 phút/lần. Điểm khó chính là khả năng tích hợp/API với các nền tảng chat. |
| 14 | Vương Việt Hoàng | Tổng hợp ý kiến làm bài nhóm khi thành viên gửi nội dung rải rác qua nhiều nền tảng | Trưởng nhóm / người tổng hợp bài | Phải sao chép nội dung thủ công từ Zalo, Messenger, Docs rồi ghép và định dạng lại | Vấn đề khá rõ vì gây mất thời gian và có nguy cơ sót ý. AI có thể hỗ trợ tổng hợp nhưng cần giữ nguyên ý nghĩa của từng thành viên. |
| 15 | Vương Việt Hoàng | Học từ mới bằng thẻ ghi nhớ nhưng thiếu ngữ cảnh nên nhanh quên | Người học tiếng Anh | Bước ôn tập chỉ dựa trên từ riêng lẻ, không gắn với tình huống/ngữ cảnh thực tế | Có tác động rõ, khoảng 15–20 phút/ngày và tỷ lệ quên cao. AI có thể tạo ngữ cảnh nhưng cần kiểm chứng liệu người học có duy trì sử dụng lâu dài hay không. |

### 3.2. Gom trùng / cluster (gom 9-12 ý thành 3-4 cụm)

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| A — Quy trình xử lý lỗi phần mềm | #1, #2, #3 | Lập trình viên backend phải chuyển thông tin giữa code, Git, Jira và kiểm thử viên sau khi phát hiện hoặc sửa lỗi | Workflow kỹ thuật rõ và lặp lại; có thể dùng Rule/Workflow để thu thập dữ liệu, nhưng nội dung vẫn cần người hiểu bối cảnh nghiệp vụ kiểm tra |
| B — Điều phối và kiểm tra bài nhóm | #4, #5, #6, #12, #14 | Thông tin task, deadline, tiến độ, ý kiến đóng góp và yêu cầu nộp bài bị phân tán nên thành viên phải tìm, hỏi lại, tổng hợp hoặc rà soát thủ công | #4, #5, #12 và #14 có cùng root cause là thiếu một nguồn thông tin tập trung; #6 thiên về checklist/rule hơn AI |
| C — Quy trình tìm và ứng tuyển việc | #7, #8, #9 | Người tìm việc phải đọc, so sánh và nhập lại dữ liệu giữa trang đăng việc, trang tuyển dụng của doanh nghiệp, CV, email và bảng theo dõi | #7 bao quát giai đoạn đầu của quy trình nhưng vẫn có workflow cụ thể; #8 và #9 có thể trở thành bước sau trong workflow tương lai |
| D — Quản lý thông tin và học tập cá nhân | #10, #11, #13, #15 | Người học phải lọc, tìm lại hoặc bổ sung ngữ cảnh cho thông tin rời rạc từ email, tin nhắn, lịch, tài liệu và thẻ ghi nhớ | #13 có bằng chứng ban đầu khá rõ; tuy nhiên khả năng truy cập dữ liệu chat là rào cản. #15 khác về workflow nhưng cùng gặp khó khăn do thiếu ngữ cảnh để sử dụng thông tin hiệu quả |

### 3.3. Shortlist (giữ 2-3 bài trả lời được 7 câu hỏi worksheet)

| Candidate | Vì sao vào shortlist (2-3 ý) | Rủi ro / điều chưa rõ |
|---|---|---|
| #7 — Tổng hợp, loại bỏ tin trùng và tạo danh sách việc làm rút gọn | Actor cụ thể là sinh viên mới tốt nghiệp; workflow nhiều bước nhưng có thể vẽ rõ trước/sau; số liệu ban đầu 60–90 phút/phiên cho thấy mức ảnh hưởng đáng kể; có thể so sánh Rule cho tin trùng, Workflow cho toàn quy trình và AI cho việc đọc, đối chiếu mô tả công việc | Chưa có dữ liệu về tần suất tìm việc, tỷ lệ tin trùng và độ chính xác khi đánh giá phù hợp; việc thu thập tự động có thể bị hạn chế bởi điều khoản hoặc cấu trúc từng website |
| #1 — Viết báo cáo chi tiết về lỗi đã sửa | Workflow tuyến tính, diễn ra sau mỗi lần sửa lỗi; đầu vào có thể lấy từ ticket, phần code thay đổi và commit; thời gian và chất lượng báo cáo đều có thể đo | AI có thể thiếu bối cảnh nghiệp vụ hoặc suy diễn sai nguyên nhân; chưa rõ tần suất lỗi và số liệu ban đầu có đại diện cho cả nhóm phát triển không |
| #13 — Tìm lại link bài giảng, prompt và tài liệu trong chat | Actor là sinh viên; evidence ban đầu rõ với tần suất 3–4 lần/tuần và 10–15 phút/lần; workflow tìm kiếm và đọc lại có thể vẽ được; có thể so sánh search theo rule với semantic search/AI | API và quyền truy cập Zalo/Slack/Discord khác nhau; phạm vi nhiều nền tảng có thể quá rộng và kết quả sai có thể làm người học bỏ sót tài liệu |

### 3.4. Score để đồng thuận (chấm 1-5, ép nói rõ vì sao cho 5 / cho 3)

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #7 — Tổng hợp, loại bỏ tin trùng và tạo danh sách việc làm rút gọn | 5 | 5 | 4 | 5 | 4 | 5 | 5 | **33** |
| #1 — Viết báo cáo chi tiết về bug đã sửa | 5 | 5 | 4 | 4 | 5 | 5 | 4 | **32** |
| #13 — Tìm lại tài liệu trong chat | 5 | 4 | 5 | 4 | 3 | 5 | 5 | **31** |

**Candidate nhóm chọn (1 bài duy nhất):**

```text
#7 — Tổng hợp vị trí việc làm từ nhiều nguồn, loại bỏ tin tuyển dụng trùng lặp và tìm thêm trên trang tuyển dụng chính thức của doanh nghiệp cho sinh viên mới tốt nghiệp.
```

**Vì sao chọn (4-5 câu):**

```text
Candidate #7 có actor cụ thể và workflow hiện tại đủ rõ: tìm ở nhiều nguồn, mở và đọc mô tả công việc, nhận diện tin trùng, đánh giá mức phù hợp rồi tạo danh sách rút gọn. Đây là vấn đề tốn thời gian nhất theo quan sát ban đầu, khoảng 60–90 phút cho mỗi phiên, nên lợi ích sau cải thiện có thể đo trực tiếp. Bài toán cũng cho phép nhóm phân tách và so sánh Rule, Workflow và AI hỗ trợ đối chiếu thay vì mặc định chọn Agent. Các thành viên đều quen với bối cảnh sinh viên mới tốt nghiệp tìm việc, nên có thể mô tả workflow và kiểm chứng nhanh. Nhóm vẫn ghi nhận tần suất, tỷ lệ tin trùng, chất lượng đánh giá và giới hạn thu thập dữ liệu là các giả định cần kiểm chứng ở Phase 4.
```

**Vì sao KHÔNG chọn các candidate còn lại (mỗi bài 2-3 câu):**

```text
#1 — Báo cáo lỗi đã sửa: workflow và đầu vào kỹ thuật rõ, nhưng báo cáo đúng còn phụ thuộc bối cảnh nghiệp vụ mà phần code thay đổi/commit có thể không thể hiện. Nhóm chưa có bằng chứng đủ mạnh về tần suất và tác động trên nhiều lập trình viên, nên giữ làm phương án thứ hai.

#13 — Tìm lại tài liệu trong chat: có tần suất và thời gian ban đầu khá rõ, nhưng việc truy cập đồng thời dữ liệu Zalo, Slack và Discord phụ thuộc API, quyền riêng tư và định dạng của từng nền tảng. Nếu thu hẹp về một nền tảng thì có thể thử nghiệm, nhưng trong phạm vi hiện tại khả năng làm trong lab thấp hơn candidate #7.
```

**Disagreement (nếu có — ai lo gì, chốt ra sao):**

```text
Nhóm có cân nhắc candidate #1 vì phạm vi nhỏ, dễ làm trong lab và candidate #13 vì có tần suất quan sát khá rõ, trong khi candidate #7 có rủi ro khi thu thập dữ liệu từ nhiều nguồn. Sau khi đối chiếu bảy tiêu chí của cả năm thành viên, nhóm thống nhất chọn #7 vì thời gian mất cho mỗi phiên lớn hơn, actor gần với trải nghiệm của nhóm và có đủ không gian để so sánh Rule/Workflow/Agent. Candidate #13 được giữ làm phương án dự phòng nếu việc lấy dữ liệu tuyển dụng không khả thi. Nhóm chưa xem #7 là Problem Statement cuối cùng; các giả định về dữ liệu và phạm vi sẽ được kiểm chứng ở Phase 4.
```

---

## Phase 4 — Quick Validation + Research

### 4.1. Quick validation (ít nhất 1 cách: interview 2-3 người hoặc survey 5-10 người)

Nhóm dùng một mẫu khảo sát mô phỏng gồm 5 sinh viên đang hoặc sắp tìm việc. Các số dưới đây chỉ dùng để hoàn thiện cấu trúc bài và cần được thay bằng kết quả khảo sát thật trước khi nộp nếu giảng viên yêu cầu bằng chứng gốc.

| Nguồn | Số người | Tín hiệu xác nhận | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Mini poll mô phỏng | 5 | 4/5 người tìm việc trên ít nhất 2 nguồn; 3/5 từng lưu trùng cùng một vị trí; 4/5 mất khoảng 60–90 phút cho một phiên tìm và lọc việc | 1/5 chỉ dùng một nền tảng cùng email thông báo và cho rằng cách hiện tại đã đủ | Thu hẹp workflow còn tối đa 3 loại nguồn; tập trung vào loại tin trùng và gợi ý mức phù hợp thay vì tự động nộp hồ sơ |
| Trao đổi nhanh mô phỏng | 5 | Câu trả lời lặp lại nhiều nhất: “Mất thời gian nhất là đọc lại mô tả và kiểm tra xem đã lưu vị trí này chưa.” | 2/5 cho biết họ vẫn muốn tự đọc kỹ mô tả công việc trước khi quyết định | Giữ bước người dùng kiểm tra; AI chỉ gợi ý và phải hiển thị nội dung gốc làm căn cứ |

**Insight sau validation (1-2 câu — pain thật nằm ở đâu):**

```text
Pain chính không nằm ở việc tìm được càng nhiều tin càng tốt. Pain nằm ở bước đọc lại mô tả, nhận diện tin trùng và biến kết quả từ nhiều nguồn thành một danh sách rút gọn đủ tin cậy; vì vậy AI chỉ hỗ trợ gợi ý, còn người dùng vẫn kiểm tra quyết định cuối.
```


### 4.2. Research giải pháp đã có (ít nhất 2-3 tools/patterns + 1-2 link kiểm được)

| Nguồn / tool / case | Link | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Teal Job Search Extension | [Trang chính thức](https://www.tealhq.com/tool/job-search-chrome-extension) | Tìm trên nhiều trang đăng việc, lưu tin vào một bảng theo dõi và tách thông tin/từ khóa từ mô tả công việc | Hỗ trợ hơn 40 trang đăng việc; giảm thao tác lưu và chuyển tab | Không nêu khả năng tự động phát hiện cùng một tin đăng ở nhiều nguồn; vẫn cần người dùng chọn và lưu tin | Không nên xây lại phần theo dõi cơ bản; tập trung vào phát hiện tin trùng và xếp hạng phù hợp trên dữ liệu người dùng đã chọn |
| Huntr Chrome Extension | [Tài liệu chính thức](https://help.huntr.co/en/articles/9859408-the-huntr-chrome-extension) | Lưu tin từ nhiều trang đăng việc và trang tuyển dụng doanh nghiệp, tự điền một số trường vào bảng theo dõi | Phủ nhiều nguồn, cho phép người dùng sửa dữ liệu thiếu hoặc sai | Nguồn không hỗ trợ vẫn phải sao chép thủ công; không tự giải quyết việc tìm thêm tin và đánh giá phù hợp | Workflow tương lai phải cho phép nhập link/nội dung thủ công và luôn cho người dùng sửa dữ liệu |
| Simplify Copilot | [Tài liệu chính thức](https://help.simplify.jobs/articles/2415391-using-copilot-to-autofill-applications) | So sánh CV với mô tả công việc, làm nổi bật từ khóa/kỹ năng thiếu và hỗ trợ điền biểu mẫu ứng tuyển | Giảm việc nhập lặp lại; người dùng kiểm tra trước khi gửi | Tập trung vào giai đoạn ứng tuyển, không giải quyết đầy đủ việc gom tin, nhận diện tin trùng và tạo danh sách rút gọn | Phạm vi của nhóm dừng ở danh sách rút gọn; không mở rộng sang tự điền biểu mẫu hoặc tự nộp hồ sơ |
| Chính sách LinkedIn về phần mềm bị cấm | [LinkedIn Help](https://www.linkedin.com/help/linkedin/answer/a1341387/prohibited-software-and-extensions?lang=en) | Quy định cách công cụ bên thứ ba được phép truy cập nền tảng | Cho nhóm một giới hạn pháp lý và kỹ thuật rõ ràng | LinkedIn cấm công cụ tự động thu thập dữ liệu hoặc tự động thao tác; tài khoản có thể bị hạn chế | Không tự động lấy dữ liệu từ LinkedIn và không vượt giới hạn truy cập; thử nghiệm chỉ dùng link/nội dung người dùng chủ động cung cấp hoặc nguồn/API cho phép |

**Research takeaway (2-3 câu — nên build gì / không build gì):**

```text
Không nên xây một Agent tự quét mọi website hoặc tự nộp hồ sơ. Hướng phù hợp là một Workflow bán tự động: người dùng đưa vào link hoặc dữ liệu từ nguồn được phép; Rule chuẩn hóa và phát hiện tin trùng rõ ràng; AI trích xuất yêu cầu, nhận diện các tin gần giống và gợi ý mức phù hợp; người dùng kiểm tra rồi mới đưa vào danh sách rút gọn.
```

> Lưu ý: không dùng số liệu AI đưa nếu không verify được link chính thức. Ghi rõ giả định chưa chắc.

---

## Phase 5 — Workflow + Problem Statement

### 5.1. Current workflow bản nhóm

Dán workflow hoặc link file: `02-group-problem-statement-workflow.png/pdf/md`

```text
CURRENT STATE — 7 bước, khoảng 60–90 phút/phiên

[1 Đặt tiêu chí: 5' — sinh viên]
→ [2 Tìm trên các trang đăng việc: 15–25']
→ [3 Mở trang tuyển dụng của doanh nghiệp: 10–15']
→ [4 Ghi lại thông tin tin tuyển dụng: 5–10']
→ [5 So sánh và loại tin trùng: 5–10']
→ [6 Đọc mô tả công việc, đánh giá phù hợp: 15–20']  <-- bottleneck
→ [7 Chốt danh sách rút gọn: 5']
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú (handoff? bottleneck?) |
|---|---|---|---|---|---|
| 1 | Sinh viên mới tốt nghiệp | Vị trí mong muốn, kỹ năng, địa điểm, loại hình làm việc | Bộ tiêu chí tìm và tiêu chí bắt buộc | 5 phút/phiên | Làm thủ công; tiêu chí có thể thay đổi theo từng phiên |
| 2 | Sinh viên | Từ khóa và bộ lọc | Danh sách tin từ 1–2 trang đăng việc | 15–25 phút/phiên | Phải đổi tab, cuộn và mở nhiều kết quả |
| 3 | Sinh viên | Danh sách doanh nghiệp quan tâm | Tin bổ sung từ trang tuyển dụng của doanh nghiệp | 10–15 phút/phiên | Có thể phát hiện tin chưa thấy trên trang đăng việc; cấu trúc mỗi trang khác nhau |
| 4 | Sinh viên | Link và nội dung tin | Bảng tạm gồm công ty, vị trí, địa điểm, ngày đăng, link và mô tả công việc | 5–10 phút/phiên | Sao chép thủ công; dễ thiếu trường hoặc sai định dạng |
| 5 | Sinh viên | Bảng tin từ nhiều nguồn | Danh sách đã loại bớt tin trùng | 5–10 phút/phiên | So sánh URL, tên công ty, chức danh và nội dung; tin gần giống khó nhận diện |
| 6 | Sinh viên | Mô tả công việc và hồ sơ/kỹ năng cá nhân | Nhận định phù hợp, lý do và điểm còn thiếu | 15–20 phút/phiên | **Bottleneck:** phải đọc nhiều mô tả không đồng nhất và tự so sánh với hồ sơ |
| 7 | Sinh viên | Danh sách đã đánh giá | Danh sách rút gọn để tiếp tục nghiên cứu hoặc ứng tuyển | 5 phút/phiên | Quyết định cuối thuộc về người tìm việc; chưa chuyển sang bước nộp hồ sơ |

**Bottleneck chính (2-3 câu):**

```text
Bottleneck chính nằm ở bước 5–6: nhận diện cùng một vị trí được đăng khác tên/khác link và đọc từng mô tả công việc để đánh giá phù hợp. Hai bước này tốn khoảng 20–30 phút/phiên, cần hiểu ngôn ngữ và ngữ cảnh, đồng thời dễ làm người dùng bỏ sót tin tốt hoặc giữ lại nhiều tin trùng.
```

### 5.2. Future workflow bản nhóm

Phải nhìn ra 5 thứ: bước nào máy (Rule), bước nào AI, bước nào người, giới hạn kiểm soát ở đâu và phương án dự phòng khi AI sai.

```text
[1 Người dùng nhập tiêu chí + hồ sơ: 5' — người]
→ [2 Nhập link/nội dung từ nguồn được phép: 5–7' — người + máy]
→ [3 Chuẩn hóa trường dữ liệu, loại tin trùng rõ ràng: <1' — Rule]
→ [4 Trích xuất mô tả công việc, phát hiện tin gần giống, chấm mức phù hợp kèm lý do: 2–4' — AI]
→ [5 Kiểm tra tin trùng và mức phù hợp: 8–11' — người, điểm kiểm soát bắt buộc]
→ [6 Xuất danh sách rút gọn: <1' — máy]

Phương án dự phòng: Nếu AI không chắc, giữ cả hai tin và gắn nhãn “cần kiểm tra”; nếu điểm phù hợp thiếu căn cứ, không xếp hạng mà hiển thị mô tả công việc gốc. Người dùng có thể bỏ kết quả AI và dùng bảng chuẩn hóa + bộ lọc Rule.
```

**Tác động trước/sau:**

| Metric | Trước | Sau kỳ vọng | Cách đo |
|---|---:|---:|---|
| Tổng thời gian | 60–90 phút/phiên | Không quá 30 phút/phiên | Bấm giờ từ lúc đặt tiêu chí đến khi chốt danh sách rút gọn trong ít nhất 3 phiên/người |
| Số bước | 7 | 6 | Đếm theo workflow đã mô tả; việc nộp hồ sơ nằm ngoài phạm vi |
| Số bước thủ công | 7/7 | 2/6 bước chính; 1 bước phối hợp người–máy | Đếm bước cần người thực hiện toàn bộ; bước kiểm tra bắt buộc không được bỏ |
| Bottleneck chính | So sánh tin trùng và đọc/đánh giá mô tả công việc: 20–30 phút | Kiểm tra kết quả: 8–12 phút | Ghi thời gian riêng cho từng bước trong nhật ký thử nghiệm |
| Rủi ro mới | Không có lỗi do AI | Gộp nhầm hai tin khác nhau, bỏ sót tin trùng hoặc xếp hạng không đúng | So sánh với nhãn của hai thành viên; đo độ chính xác, độ bao phủ và tỷ lệ đề xuất được người dùng chấp nhận |

### 5.3. Problem Statement v0

| Field | Nội dung |
|---|---|
| **Actor** | Sinh viên mới tốt nghiệp đang chủ động tìm việc, có CV hoặc hồ sơ kỹ năng cơ bản nhưng chưa có một danh sách cơ hội tập trung. Nhóm ưu tiên người tìm các vị trí dành cho người mới trong một nhóm ngành cụ thể. |
| **Workflow** | Trong mỗi phiên, sinh viên đặt tiêu chí, tìm trên trang đăng việc, xem trang tuyển dụng của doanh nghiệp, ghi lại tin, so sánh tin trùng, đọc mô tả công việc, đánh giá phù hợp và tạo danh sách rút gọn. Hiện toàn bộ các bước đều làm thủ công trên nhiều tab và bảng ghi chép. |
| **Bottleneck** | So sánh tin trùng và đọc mô tả công việc để đối chiếu với hồ sơ mất khoảng 20–30 phút trong tổng 60–90 phút/phiên. Tin tuyển dụng có cách đặt tên và cấu trúc khác nhau nên bộ lọc từ khóa đơn giản không xử lý hết. |
| **Impact** | Người tìm việc mất thời gian, dễ mệt mỏi, giữ lại cùng một tin nhiều lần hoặc bỏ qua tin phù hợp trên trang tuyển dụng của doanh nghiệp. Nghiên cứu công khai xác nhận người tìm việc sử dụng nhiều loại nguồn, nhưng mức 60–90 phút hiện mới là số liệu ban đầu của nhóm cần thử nghiệm xác nhận. |
| **Success Metric** | Trong thử nghiệm, giảm trung vị tổng thời gian từ số liệu ban đầu được đo lại xuống không quá 30 phút/phiên; độ chính xác (precision) và độ bao phủ (recall) khi phát hiện tin trùng đều đạt tối thiểu 90%; ít nhất 80% tin được hệ thống đề xuất được người dùng đồng ý giữ lại. Đo trên tối thiểu 3 phiên và một tập 50–100 tin đã được hai người gắn nhãn. |
| **Boundary** | Làm: nhận link/nội dung do người dùng cung cấp hoặc dữ liệu từ nguồn cho phép, chuẩn hóa trường, phát hiện tin trùng, trích xuất mô tả công việc và gợi ý mức phù hợp có giải thích. Không làm: tự động thu thập từ nguồn cấm, vượt giới hạn truy cập, tự nộp hồ sơ, tự sửa CV, tự liên hệ nhà tuyển dụng hoặc loại tin vĩnh viễn khi chưa có người kiểm tra. |

**Câu hỏi AI phản biện v0 (nếu có):**
- Field nào mơ hồ: “Phù hợp” ban đầu chưa có tiêu chí; 60–90 phút chưa phải số liệu đã xác nhận; “nhiều nguồn” có thể làm phạm vi quá rộng; chỉ đo tốc độ sẽ khuyến khích bỏ sót tin.
- Tôi sửa gì: Giới hạn actor và đầu vào, định nghĩa phù hợp bằng tiêu chí bắt buộc/ưu tiên của người dùng, thêm chỉ số chất lượng cho phát hiện tin trùng và danh sách rút gọn, đồng thời loại việc thu thập dữ liệu trái điều khoản khỏi phạm vi.

---

## Phase 6 — Rule / Workflow / Agent + Decision

### 6.0. Ma trận độ phù hợp

- Độ mơ hồ: [ ] Thấp / [x] Cao — Hai tin có thể cùng vị trí nhưng khác cách đặt tên; mức phù hợp còn phụ thuộc mục tiêu, kỹ năng và ưu tiên của từng người.
- Độ phức tạp: [ ] Thấp / [x] Cao — Workflow có hơn ba bước, nhiều nguồn dữ liệu và kết quả chuẩn hóa là đầu vào cho nhận diện tin trùng, chấm phù hợp và tạo shortlist.

**Bài toán nhóm nằm ở ô nào:**

```text
Độ phức tạp cao – độ mơ hồ cao, nhưng có thể giới hạn bằng một Workflow cố định có người kiểm tra.
```

**Vì sao (2-3 câu):**

```text
Đầu vào và thứ tự xử lý tương đối ổn định, nên độ phức tạp cao không đồng nghĩa phải dùng Agent. Rule xử lý phần có đúng/sai rõ; AI chỉ xử lý ngôn ngữ và so sánh ngữ nghĩa; sinh viên giữ quyền quyết định ở bước kiểm tra.
```

### 6.1. So sánh Rule / Workflow / Agent

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? (Dùng cho bước nào?) |
|---|---|---|---|---|
| **Rule** | Chuẩn hóa chữ hoa/thường, URL, tên công ty, chức danh, địa điểm; so khớp URL hoặc bộ khóa công ty–vị trí–địa điểm; lọc theo điều kiện bắt buộc | Đủ khi tin có trường dữ liệu chuẩn và trùng hoàn toàn; cũng là phương án dự phòng không dùng AI | Không nhận ra tin diễn đạt khác nhau, có thể bỏ sót yêu cầu nằm trong mô tả công việc | Có — dùng cho chuẩn hóa, loại tin trùng rõ ràng và lọc điều kiện bắt buộc |
| **Workflow** | Nhập dữ liệu → Rule chuẩn hóa → AI trích xuất/so sánh → AI gợi ý mức phù hợp kèm dẫn chứng → người kiểm tra → xuất danh sách rút gọn | Hợp khi các bước đi theo thứ tự cố định và mọi quyết định ảnh hưởng danh sách cuối đều có người duyệt | AI có thể gộp nhầm, suy diễn kỹ năng hoặc chấm điểm thiếu nhất quán | **Chọn** — dùng làm kiến trúc chính, kết hợp Rule, AI và người kiểm tra |
| **Agent** | Tự chọn nguồn, đổi truy vấn, duyệt trang tuyển dụng, thu thập tin, đánh giá và cập nhật danh sách | Chỉ đáng cân nhắc khi có API và quyền truy cập rõ, cần tự lập kế hoạch và đã chứng minh Workflow cố định không đủ | Quyền truy cập rộng, khó truy vết, dễ vi phạm điều khoản website hoặc tự hành động sai | Không chọn — chưa cần tự lập kế hoạch hay tự dùng công cụ trên website |

**5 câu hỏi chốt (trả lời câu đầy đủ):**
1. Rule không giải được 70–80% toàn bài vì chỉ bắt được tin trùng rõ ràng và điều kiện bắt buộc; việc hiểu JD và đánh giá phù hợp cần so sánh ngữ nghĩa.
2. Các bước chủ yếu đi theo một đường cố định; chỉ rẽ nhánh khi dữ liệu thiếu hoặc AI không chắc, khi đó tin được gắn nhãn để người dùng kiểm tra.
3. Chưa cần Agent tự lập kế hoạch hoặc tự gọi công cụ vì nguồn và thứ tự xử lý do người dùng quyết định trước; tự duyệt website còn tạo thêm rủi ro về quyền truy cập và điều khoản sử dụng.
4. Sinh viên tìm việc là người phát hiện đầu tiên ở bước kiểm tra; với link và đoạn mô tả công việc gốc hiển thị cạnh kết quả, mục tiêu là sửa hoặc tách/gộp lại trong dưới 2 phút mỗi trường hợp.
5. Có thể hạ từ Agent xuống Workflow; bên trong Workflow tiếp tục hạ các bước chuẩn hóa, so khớp rõ ràng và lọc bắt buộc xuống Rule.

**Mức chọn:**

```text
Workflow (kết hợp Rule, AI hỗ trợ và người kiểm tra).
```

**Vì sao chọn:**

```text
Các bước có thứ tự và đầu vào/đầu ra rõ nên Workflow kiểm soát được hơn Agent. Rule xử lý dữ liệu có cấu trúc và các trường hợp trùng rõ ràng; AI chỉ tham gia khi cần hiểu cách diễn đạt trong mô tả công việc hoặc so sánh với hồ sơ. Mọi tin bị gộp và mọi đề xuất cho danh sách rút gọn đều phải qua sinh viên kiểm tra. Cách này vừa giảm công việc lặp lại, vừa giữ được khả năng giải thích và quay về cách thủ công khi AI sai.
```

**Vì sao không chọn mức đơn giản hơn:**

```text
Rule đơn thuần không hiểu được hai mô tả công việc dùng tên khác nhau cho cùng vai trò và không đánh giá tốt các kỹ năng tương đương hoặc yêu cầu ngầm. Vì vậy Rule là thành phần bắt buộc nhưng chưa giải được bottleneck đọc hiểu và so sánh ngữ nghĩa; cần thêm AI trong một Workflow có giới hạn.
```

### 6.2. Problem Statement v1 (v0 sửa chặt hơn + 3 field cuối)

| Field | Nội dung |
|---|---|
| **Actor** | Sinh viên mới tốt nghiệp đang tìm vị trí dành cho người mới trong một nhóm ngành, có CV/hồ sơ kỹ năng và bộ tiêu chí bắt buộc/ưu tiên do chính mình xác nhận. |
| **Workflow** | Mỗi phiên, người dùng nhập tiêu chí và link/nội dung từ tối đa ba loại nguồn được phép; hệ thống chuẩn hóa, tìm tin trùng, trích xuất yêu cầu, so sánh với hồ sơ, rồi đưa danh sách có lý do để người dùng kiểm tra và xuất danh sách rút gọn. |
| **Bottleneck** | Việc so sánh tin trùng và đọc nhiều mô tả công việc để đánh giá mức phù hợp hiện mất khoảng 20–30 phút trong tổng 60–90 phút/phiên. Các tin khác link hoặc khác tên nhưng gần giống nhau khiến Rule đơn giản chưa đủ. |
| **Impact** | Người dùng mất thời gian chuyển nguồn, dễ mệt mỏi, giữ tin trùng hoặc bỏ sót cơ hội phù hợp. Nguồn công khai xác nhận hành vi tìm việc đa kênh; mức tác động cụ thể của nhóm sẽ được xác nhận bằng nhật ký thử nghiệm. |
| **Success Metric** | Sau tối thiểu 3 phiên trên 50–100 tin đã gắn nhãn: tổng thời gian không quá 30 phút/phiên; độ chính xác và độ bao phủ khi phát hiện tin trùng đều từ 90% trở lên; ít nhất 80% tin được đề xuất được người dùng chấp nhận vào danh sách rút gọn. |
| **Boundary** (làm / không làm) | Làm với link/nội dung người dùng cung cấp hoặc nguồn/API cho phép; lưu mô tả công việc gốc và lý do cho mỗi đề xuất. Không tự động thu thập từ LinkedIn/nguồn cấm, không vượt giới hạn truy cập, không tự nộp hồ sơ, không sửa CV, không nhắn nhà tuyển dụng và không tự xóa tin chưa được kiểm tra. |
| **AI intervention point** (can thiệp sau bước nào, trước bước nào) | AI can thiệp sau khi Rule đã chuẩn hóa và loại các trường hợp trùng rõ ràng, trước bước sinh viên kiểm tra. AI trích xuất yêu cầu, tìm các tin gần giống và so sánh mô tả công việc với tiêu chí/hồ sơ bằng dẫn chứng từ nội dung gốc. |
| **Mức chọn** (Rule / Workflow / Agent + 1 câu vì sao) | **Workflow:** chuỗi bước ổn định, dùng Rule cho phần xác định, AI cho phần ngôn ngữ và người dùng cho quyết định cuối; chưa cần Agent tự lập kế hoạch. |
| **Rủi ro & người thật kiểm tra** (rủi ro lớn nhất + ai kiểm tra bằng cách nào) | Rủi ro lớn nhất là gộp nhầm hai vị trí khác nhau hoặc đánh giá phù hợp sai. Sinh viên kiểm tra tên công ty, vị trí, địa điểm, link, yêu cầu bắt buộc và dẫn chứng từ mô tả công việc trước khi xác nhận gộp hoặc đưa tin vào danh sách rút gọn. |

### 6.3. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú (câu đầy đủ) |
|---|---|---|
| Actor + workflow rõ chưa? | Yes | Actor đã giới hạn là sinh viên mới tốt nghiệp tìm việc dành cho người mới; workflow hiện tại và tương lai đều có bước, người thực hiện, đầu vào/đầu ra và giới hạn rõ. |
| Baseline + metric đo được chưa? | Not Yet | Có số liệu ban đầu 60–90 phút/phiên và mục tiêu cụ thể, nhưng cần ghi nhật ký ít nhất 3 phiên để xác nhận trung vị và thời gian từng bước. |
| Data/input đủ dùng chưa? | Not Yet | Có thể tạo tập thử nghiệm từ 50–100 link/mô tả công việc do người dùng cung cấp, nhưng chưa có tập đã gắn nhãn tin trùng và phù hợp để đánh giá chính xác. |
| AI sai, hậu quả chấp nhận được không? | Yes | Trong thử nghiệm, AI chỉ gợi ý và không tự xóa/nộp hồ sơ; người dùng thấy nội dung gốc và kiểm tra nên lỗi có thể đảo ngược với chi phí thấp. |
| Có người kiểm tra/chịu trách nhiệm không? | Yes | Sinh viên tìm việc là người chịu trách nhiệm và phải xác nhận tin trùng, mức phù hợp và danh sách rút gọn cuối. |
| Có cách non-AI đơn giản hơn không? | Yes | Bảng theo dõi chung, trường dữ liệu chuẩn, bộ lọc bắt buộc và so khớp Rule giải được phần dữ liệu có cấu trúc; đây là phương án dự phòng và mốc so sánh với Workflow có AI. |

**Decision:**

```text
Go với thử nghiệm nhỏ, bán thủ công và có người kiểm tra; chưa triển khai Agent hoặc tự động thu thập dữ liệu.
```

**Lý do (3-4 câu dựa trên bằng chứng):**

```text
Actor, workflow và điểm nghẽn đã đủ rõ để thử nghiệm; nghiên cứu nguồn công khai cũng xác nhận người tìm việc sử dụng nhiều nguồn và các công cụ hiện có chưa giải quyết trọn vẹn việc phát hiện tin trùng xuyên nguồn rồi tạo danh sách rút gọn. Dù vậy, số liệu 60–90 phút và chất lượng AI chưa được kiểm chứng bằng dữ liệu của nhóm, nên “Go” chỉ dành cho thử nghiệm có phạm vi nhỏ. Thử nghiệm không tự động lấy dữ liệu từ LinkedIn, không tự nộp hồ sơ và mọi quyết định đều do người tìm việc xác nhận.
```

**Nếu Go — thử nghiệm nhỏ nhất (dữ liệu nào, chạy tay ra sao, đo 3 số nào):**

```text
Dữ liệu: 50–100 tin dành cho người mới trong cùng một nhóm ngành, lấy từ tối đa ba loại nguồn được phép; lưu URL, công ty, chức danh, địa điểm, ngày đăng và mô tả công việc. Hai thành viên độc lập gắn nhãn cặp tin trùng và tin phù hợp; nếu bất đồng thì cùng đọc lại mô tả để chốt nhãn chuẩn.

Cách chạy: thực hiện 3 phiên theo cách cũ để xác nhận số liệu ban đầu; sau đó chạy Workflow bán thủ công, trong đó người dùng dán link/nội dung, Rule chuẩn hóa, AI đưa đề xuất kèm dẫn chứng và người dùng kiểm tra. Không cho AI tự duyệt website hoặc tự nộp hồ sơ.

Ba số cần đo: (1) trung vị tổng thời gian/phiên; (2) độ chính xác và độ bao phủ khi phát hiện tin trùng; (3) tỷ lệ tin do AI đề xuất được người dùng giữ trong danh sách rút gọn. Mục tiêu lần lượt là ≤30 phút, cả độ chính xác/độ bao phủ ≥90%, và tỷ lệ chấp nhận ≥80%.
```

**Nếu Not Yet — cần validate gì trước:**

```text
Không áp dụng vì nhóm chọn Go ở mức thử nghiệm nhỏ. Trước khi mở rộng vẫn phải xác nhận số liệu ban đầu, tần suất phiên tìm việc, tỷ lệ tin trùng, chất lượng danh sách rút gọn và quyền truy cập của từng nguồn.
```

**Nếu No-Go — làm gì thay AI:**

```text
Không áp dụng ở thời điểm hiện tại. Nếu thử nghiệm thất bại, nhóm quay về bảng theo dõi có trường chuẩn, bộ lọc Rule và danh sách kiểm tra thủ công thay cho AI.
```

**Exit / rollback (khi nào dừng AI, quay về cách cũ):**

```text
Dừng phần AI và quay về bảng theo dõi + Rule nếu xảy ra một trong các điều kiện: tổng thời gian vẫn trên 45 phút trong 3 phiên liên tiếp; độ chính xác hoặc độ bao phủ khi phát hiện tin trùng dưới 80%; người dùng phải sửa hơn 30% danh sách rút gọn; AI nhiều lần đưa lý do không có trong mô tả công việc; hoặc một nguồn không cho phép truy cập/tự động hóa. Mọi dữ liệu và nhãn thủ công vẫn được giữ để người dùng tiếp tục workflow cũ, còn nguồn vi phạm điều khoản phải được loại ngay khỏi thử nghiệm.
```

---

### Self-check nộp phần 02 (nhóm)
- [x] Có nhật ký hội tụ 15 → 1 (cluster + shortlist + score)
- [x] Có kiểm chứng từ khảo sát/dữ liệu công khai, trích dẫn ngắn và nghiên cứu với link kiểm được; không bịa phỏng vấn
- [x] Có workflow trước/sau đủ thời gian, actor, bottleneck, giới hạn kiểm soát và phương án dự phòng
- [x] Có PS v0 → v1, chỉ số có số liệu ban đầu/mục tiêu/cách đo, phạm vi có làm/không làm
- [x] Có so sánh Rule/Workflow/Agent + quyết định Go có lý do, thử nghiệm nhỏ và điều kiện quay về cách cũ rõ
