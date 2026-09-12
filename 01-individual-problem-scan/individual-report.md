# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Nguyễn Quang Hữu
- Mã học viên: 2A202602756
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): BackEnd Dev trong 1 công ty 50 người
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem): Mỗi ngày kiểm tra lỗi ở trên jira, sau khi sửa xong phải viết báo cáo về lỗi đã sửa cho PM, phải tra lại dev gây ra lỗi (nếu có), và tạo ticket cho người đó, đồng thời cũng phải tạo ticket để báo cho tester đã sửa code

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 |Lặp lại |Vào Jira, kiểm tra tên của mình cũng như những bug được assign cho mình |Dev |10 phút/lần |
| 2 |Tốn thời gian |Viết báo cáo thủ công chi tiết về các lỗi đã sửa | Dev, PM|30 phút/lần |
| 3 | Pain từ người khác |Truy tra lịch sử git/commit để tìm ra dev gây ra bug gốc |Dev |10 phút/lần |
| 4 |Lặp lại |Tạo thủ công ticket mới trên Jira giao cho dev gây lỗi |Dev, Peer Dev |10 phút/lần |
| 5 |Pain từ người khác |Tester phản hồi thông tin bug thiếu chi tiết, phải hỏi lại |Backend Dev, Tester |Tốn thêm thời gian trao đổi qua chat |
| 6 |Tốn thời gian |Dev được tra là người gây ra bug có thể không thật sự tạo bug, mà do lỗi từ người khác |Peer Dev | Tốn thêm thời gian trao đổi|
| 7 |AI có thể tốt hơn |Thiếu hệ thống tự động gợi ý đoạn code/nguyên nhân gây lỗi từ git log | Backend Dev|Phải đọc lại lịch sử commit thủ công |
| 8 |AI có thể tốt hơn |Tạo thủ công ticket báo cho tester đã sửa code | Backend Dev, Tester| 5-10 phút/lần |

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi: Tôi có 1 context như sau: 1 người dev backend Mỗi ngày kiểm tra lỗi ở trên jira, sau khi sửa xong phải viết báo cáo về lỗi đã sửa, phải tra lại dev gây ra lỗi (nếu có), và tạo ticket cho người đó, đồng thời cũng phải tạo ticket để báo cho tester đã sửa code, cho tôi 10 problems bạn nhìn ra từ đây, có thể là những vấn đề ảnh hưởng đến tốc độ làm việc, mẫu như sau:*02-deliverable-example.md*
- Ý dùng được:3,5
- Ý bỏ vì không phải pain thật: Jira không tự động phân loại nguyên nhân gốc rễ của bug, vì đây không phải vấn đề liên quan đến loại bug

**Self-check Phase 1:**
- [X] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [X] Dùng ít nhất 3/4 lăng kính
- [X] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 |Viết báo cáo thủ công chi tiết về các lỗi đã sửa | Rõ work flow, mất nhiều thời gian, ai có thể hỗ trợ mạnh |Ai sẽ chỉ cần suy xét về technical hay cả business |
| 2 |Truy tra lịch sử git/commit để tìm ra dev gây ra bug gốc |Workflow rõ, có thể dễ dàng tự động hóa | Việc sử dụng lịch sử git có thể không thật sự đáng tin |
| 3 | Tạo thủ công ticket báo cho tester đã sửa code| Lặp lại, có thể dùng data từ phần sửa lỗi để tạo ticket tự động|Tester cần các bước tái hiện chính xác |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — Viết báo cáo thủ công chi tiết về các lỗi đã sửa

```text
Problem 1 câu: Dev mất 30 phút mỗi lần fix bug để dịch các thay đổi kỹ thuật trong code thành báo cáo chi tiết, dễ hiểu cho PM.

Actor: Backend Dev

Thời điểm / bối cảnh:Ngay sau khi commit code fix bug thành công và cần cập nhật trạng thái lên Jira/gửi report.

Current workflow 3-7 bước:
1. Hoàn tất commit code.
2. Mở lại các file đã sửa để rà soát thay đổi 
3. Viết nháp báo cáo giải thích nguyên nhân gốc rễ và cách khắc phục 
4. Format lại ngôn từ để PM (non-tech) có thể hiểu được 
5. Đăng lên Jira hoặc gửi qua chat

Bottleneck: Bước 3 và 4 (Dịch từ logic code sang ngôn ngữ business/quản lý)

Impact: Giảm thời gian làm report từ 30 phút xuống còn 5 phút/bug. Tăng thời gian code thực tế.

Success metric: Thời gian hoàn thành báo cáo < 5 phút; PM không cần hỏi lại để làm rõ báo cáo.

Non-AI alternative: Tạo template mẫu  để dev điền vào, script tự động copy tên file đã sửa.

AI hypothesis: AI sẽ đóng vai trò cầu nối, phân tích code thay đổi và viết ra báo cáo gồm: Nguyên nhân, Cách sửa, Ảnh hưởng.

Quick gut:
Workflow
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE — 30 phút

[1 Commit code: 0'] → [2 Rà soát file: 5'] → [3 Viết nháp giải thích: 15'] <-- bottleneck → [4 Format cho PM: 5'] → [5 Gửi: 5']

FUTURE STATE — 5 phút

[1 Commit code: 0'] → [2 AI tự đọc git diff + Jira ticket tạo draft report: 1'] → [3 Dev review & tinh chỉnh: 3'] <-- human boundary → [4 Gửi: 1']

Fallback: Nếu AI sinh báo cáo sai ngữ cảnh, dev bỏ draft và gõ tay theo template (như Current State) hoặc chỉ prompt lại với context ngắn gọn.
```



---

#### Problem Card #2 — Truy tra lịch sử git/commit để tìm ra dev gây ra bug gốc

```text
Problem 1 câu: Mất 10-20 phút để truy xuất lịch sử git nhằm tìm ra người thực sự gây ra lỗi và tạo ticket giao việc cho họ trên hệ thống.

Actor: Backend Dev

Thời điểm / bối cảnh: Khi phát hiện bug không thuộc module của mình hoặc cần phân công người fix tận gốc.

Current workflow 3-7 bước:
1. Nhận diện dòng code gây lỗi.
2. Chạy `git blame` hoặc tra cứu lịch sử commit trên IDE 
3. Đọc commit log để xác nhận đó là logic lỗi hay chỉ là refactor/typo 
4. Vào Jira tạo ticket mới
5. Assign cho dev tương ứng và link vào ticket gốc 

Bottleneck: Bước 2 - Tốn thời gian đọc code và xác định lỗi.

Impact: Tránh gián đoạn mạch làm việc (context switching), giảm thời gian điều tra xuống < 5 phút.

Success metric:  Thời gian xử lý < 5 phút.

Non-AI alternative: Dùng Git hooks hoặc CLI script để tự động lấy tên người commit cuối cùng và gọi API Jira tạo ticket.

AI hypothesis: Một agent nhận file và line number gây lỗi, tự động gọi Git log/blame để lấy lịch sử 5 commit gần nhất, dùng AI đánh giá commit nào thực sự thay đổi logic kinh doanh dẫn tới lỗi, sau đó format sẵn payload API để tạo Jira ticket.

Quick gut:
[x] Agent
```

**Draft workflow Card #2:**

```text
CURRENT STATE — 20 phút

[1 Nhận diện lỗi: 0'] → [2 Chạy git blame: 5'] → [3 Đọc & xác minh commit log: 10'] <-- bottleneck → [4 Tạo ticket Jira: 5'] 

FUTURE STATE — 4 phút

[1 Chọn dòng lỗi & gọi Agent: 1'] → [2 Agent đọc Git history + đề xuất người chịu trách nhiệm & draft nội dung ticket: 1'] → [3 Dev review xác nhận: 2'] <-- human boundary → [4 Hệ thống tự tạo ticket: 0']

Fallback: AI không chắc chắn ai là người tạo bug -> Đẩy ticket về backlog chung hoặc dev tự đọc lại log thủ công.
```


---

#### Problem Card #3 — Tạo thủ công ticket báo cho tester đã sửa code

```text
Problem 1 câu: Dev tốn 10 phút để dịch lại cách thức tái hiện lỗi và kịch bản test cho Tester sau khi hoàn thành code.

Actor: Backend Dev, Tester

Thời điểm / bối cảnh: Code đã được merge, cần tạo sub-task hoặc comment trên Jira để Tester tiến hành verify.

Current workflow 3-7 bước:
1. Mở ticket đã fix.
2. Nhớ lại luồng data/API đã thay đổi 
3. Viết các bước "Steps to test" từ góc nhìn của user/tester
4. Đính kèm cURL hoặc payload API (nếu có)
5. Chuyển trạng thái ticket 

Bottleneck: Bước 3 (Dev quen suy nghĩ theo logic code, mất công chuyển đổi góc nhìn sang kịch bản test UI/API).

Impact: Chuẩn hóa chất lượng đầu vào cho Tester, giảm bớt số lần Tester phải ping hỏi lại qua chat.

Success metric: Thời gian viết kịch bản test < 2 phút; Giảm 80% tin nhắn ping hỏi lại từ Tester.

Non-AI alternative: Bắt buộc dev điền template "Steps to Verify" trên Jira (Vẫn tốn thời gian nghĩ và gõ).

AI hypothesis: Tận dụng luôn draft báo cáo từ Problem 1. Đưa draft report + mô tả bug ban đầu vào LLM để tạo ra checklist "Steps to reproduce & verify" chuẩn chỉnh.

Quick gut:
[x] Workflow
```

**Draft workflow Card #3:**

```text
CURRENT STATE — 10 phút

[1 Mở ticket: 0'] → [2 Viết "Steps to test": 5'] <-- bottleneck → [3 Chuẩn bị data test/cURL: 3'] → [4 Chuyển trạng thái: 2']

FUTURE STATE — 3 phút

[1 Trigger AI (từ lúc có báo cáo PM): 0'] → [2 AI gen checklist test & API payload: 1'] → [3 Dev rà soát lại: 2'] <-- human boundary → [4 Update Jira: 0']

Fallback: AI sinh kịch bản test vô lý, dev sửa thẳng vào ô text của Jira trước khi submit.
```

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Viết báo cáo thủ công chi tiết về các lỗi đã sửa
```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Workflow tuyến tính, không đòi hỏi thay đổi quá nhiều. Số đo impact lớn nhất
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
1.AI chỉ thấy được những dòng code bị thay đổi, làm sao nó biết được toàn bộ context business của tính năng đó để báo cáo cho PM?
```