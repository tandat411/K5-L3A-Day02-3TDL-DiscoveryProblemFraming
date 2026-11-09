# Báo cáo cá nhân — 2A202603646_NguyenManhTuong

## 1. Thông tin học viên

- Họ tên: Nguyễn Mạnh Tường
- MSSV: 2A202603646
- Tên nhóm: 3TDL
- Repo nhóm: https://github.com/tandat411/K5-L3A-Day02-3TDL-DiscoveryProblemFraming

## 2. Scan problem (CP1)

Tôi bắt đầu từ những việc có người làm, có thời điểm xảy ra và có hậu quả nếu làm chậm. Với các con số chưa có nhật ký theo dõi, tôi ghi rõ đó là ước lượng cần kiểm tra, không coi là kết quả khảo sát.

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu và mức độ chắc chắn |
|---:|---|---|---|---|
| 1 | Lặp lại, tốn thời gian | Khi kỳ thi cuối kỳ còn xa, tôi muốn chia việc ôn tập thành những việc đủ nhỏ để bắt đầu trong tuần này, để không dồn cả lượng kiến thức vào sát ngày thi. | Tôi, sinh viên chuẩn bị thi cuối kỳ. | Tôi đã có lúc trì hoãn **1–2 tuần** vì đích thi quá xa nên không thấy động lực. Đây là trải nghiệm tôi đã nêu; chưa có nhật ký đo số buổi học bị bỏ lỡ. |
| 2 | Lặp lại, cần tổng hợp nhiều nguồn | Khi đến cuối tuần và cần chia tiền sinh hoạt phòng trọ, tôi muốn gom các khoản đã ứng và hóa đơn chung về một bảng có thể đối soát, để không bỏ sót tiền và tránh tranh cãi khi chia. | Người đứng ra tổng hợp tiền và các bạn cùng phòng. | Tình huống nháp tôi đưa ra có **3 nguồn**: ảnh hóa đơn, lịch sử chuyển khoản, tin nhắn; quy trình được ước tính **90 phút/tuần**, riêng đối soát **35 phút**. Chưa có log của một phòng cụ thể để xác nhận thời gian này. |
| 3 | Lặp lại, tốn thời gian | Khi đi chợ cho vài ngày và nấu ăn một mình, tôi muốn biết nguyên liệu nào có thể dùng chung cho nhiều bữa, để mua vừa đủ và không phải bỏ thức ăn hỏng. | Sinh viên ở trọ tự nấu ăn. | Quy trình nháp tôi đưa ra là **90 phút/tuần**, trong đó bước chọn món khoảng **35 phút**. Mức lãng phí thực phẩm chưa được cân hoặc ghi sổ, nên không dùng tỷ lệ phần trăm làm bằng chứng. |
| 4 | Tốn thời gian, cần tổng hợp nhiều nguồn | Khi tìm phòng trọ mới, tôi muốn biết tổng tiền phải trả và những điều kiện sinh hoạt trước khi đi xem, để không mất một chuyến đi vì giá đăng thiếu phụ phí. | Sinh viên đang tìm trọ. | Bản nháp tôi đưa ra có **5–7 tin đăng/tuần** cần lọc, khoảng **40 phút** hỏi giá và phụ phí. Đây là ước lượng của tình huống, chưa có danh sách tin đã đối chiếu. |
| 5 | Cần tổng hợp nhiều nguồn | Khi sắp nộp một bài lab có notebook, báo cáo và tệp minh chứng riêng, tôi muốn kiểm tra đủ từng thành phần theo hướng dẫn, để không mất điểm vì thiếu tệp dù đã làm bài. | Tôi và người chấm bài. | Bài Day 01 của tôi từng phải bổ sung ảnh `hand_calc.jpg` ở một commit sau khi notebook và báo cáo đã có. Lịch sử commit của [repo Day 01](https://github.com/manhtuongqt/K5-L3A-DAY01-NguyenManhTuong-2A202603646-AIFoundation) là bằng chứng cho **1 tệp minh chứng được thêm sau**; tôi chưa đo số phút kiểm tra bài. |

**Cách tôi dùng gợi ý từ AI:** Tôi giữ vấn đề kiểm tra thành phần bài nộp vì có dấu vết trong repo Day 01. Tôi không đưa ý tưởng “làm chatbot học tập” vào bảng: nó là một cách giải quyết, chưa nói rõ tình huống và bước đang nghẽn. Ba tình huống phòng trọ, nấu ăn và tìm trọ là giả thuyết cần kiểm chứng thêm; số phút ở đó phục vụ việc vẽ quy trình nháp, không phải số liệu đo từ người dùng.

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Vì sao tôi chọn ba vấn đề này

| Thứ tự | Vấn đề | Lý do chọn | Điều chưa chắc |
|---:|---|---|---|
| 1 | Bắt đầu ôn thi khi hạn còn xa (#1) | Đây là trải nghiệm tôi nêu rõ nhất: chậm 1–2 tuần. Có thể kiểm tra bằng ngày bắt đầu học và số phiên học hoàn thành. | Cơ chế phần thưởng có thực sự giúp bắt đầu hay chỉ làm tôi phân tâm? |
| 2 | Đối soát tiền sinh hoạt phòng trọ (#2) | Actor, dữ liệu đầu vào và điểm nghẽn gom chứng từ đều cụ thể. Có thể thử trên một bộ hóa đơn mẫu trong buổi lab. | Thời gian 35 phút ở bước đối soát cần đo lại với người thực sự đang giữ tiền. |
| 3 | Soát đủ thành phần bài nộp (#5) | Có dấu vết thiếu ảnh ở bài Day 01; cách đo số mục thiếu rõ ràng và phạm vi thử rất nhỏ. | Một checklist viết tay có thể đã đủ, không cần can thiệp bằng AI. |

### Problem Card #1 — Bắt đầu ôn thi khi đích còn xa

| Trường | Nội dung |
|---|---|
| Job Story | Khi kỳ thi cuối kỳ còn xa, tôi muốn biết việc ôn tập nhỏ nhất nên làm trong tuần này, để bắt đầu đều hơn thay vì để trôi qua 1–2 tuần rồi mới học dồn. |
| Actor | Tôi; rộng hơn là sinh viên có lịch thi cuối kỳ và nhiều môn cùng lúc. |
| Bối cảnh | Đã biết kỳ thi sẽ đến nhưng còn vài tuần; mục tiêu “ôn xong cả môn” quá xa để tạo cảm giác phải làm ngay. |
| Quy trình hiện tại | Xem ngày thi → nghĩ đến toàn bộ kiến thức cần ôn → tự nhủ còn thời gian và chuyển sang việc khác → khi gần hạn mới chia bài → học dồn. |
| Bottleneck | Bước 3: thời gian **chờ để bắt đầu** từng kéo dài 7–14 ngày. Đây là thời gian trôi qua, không phải 10.080–20.160 phút lao động. |
| Impact | Quỹ thời gian ôn rải đều giảm đi 1–2 tuần; buổi học đầu dễ trở thành buổi chạy theo khối lượng đã dồn. |
| Success metric | Baseline tự báo: bắt đầu muộn 7–14 ngày. Target thử trong hai tuần: bắt đầu phiên ôn đầu tiên trong **48 giờ** sau khi lập kế hoạch; đếm ngày bắt đầu và số phiên 25 phút thực sự hoàn thành. |
| Phương án không dùng AI | Chia mỗi môn thành đầu việc 25 phút trên giấy/lịch; xong một phiên mới nhận phần thưởng nhỏ đã đặt trước. |
| Giả thuyết về AI | Chỉ hỗ trợ tách đề cương thành đầu việc ngắn và gợi ý thứ tự; tôi kiểm tra lại độ ưu tiên và tự quyết định phần thưởng. |
| Cảm nhận nhanh | **Rule hoặc No AI** đủ để thử trước. Chưa có lý do dùng Agent. |

Quy trình nháp hiện tại (phút ở các bước chủ động là **ước lượng để thử bấm giờ**, không phải log đã đo):

```text
Biết ngày thi và mở đề cương (5 phút)
  → Nghĩ lượng kiến thức phải học (10 phút)
  → [NGHẼN] Trì hoãn việc bắt đầu (7–14 ngày trôi qua; gần 0 phút học chủ động)
  → Gần hạn mới chọn phần cần học trước (15 phút)
  → Bắt đầu buổi ôn đầu tiên (25 phút)
```

**Phản biện PM hoài nghi:** “Nếu chỉ thêm điểm thưởng hoặc lời nhắc, vì sao người học không tiếp tục bỏ qua? Có thể vấn đề là đầu việc quá lớn và khó chọn điểm bắt đầu.” Tôi sửa card từ “cần một hệ thống thưởng” thành **đo độ trễ đến phiên học đầu tiên**, thử chia đầu việc và phần thưởng nhỏ như hai giả thuyết riêng. Nếu sau hai tuần thời gian bắt đầu không giảm, tôi sẽ bỏ giả thuyết phần thưởng.

### Problem Card #2 — Đối soát chi tiêu chung

| Trường | Nội dung |
|---|---|
| Job Story | Khi đến cuối tuần và cần chia tiền sinh hoạt phòng trọ, tôi muốn đối chiếu các khoản đã ứng với hóa đơn chung, để chia tiền rõ ràng và không bỏ sót khoản nhỏ. |
| Actor | Một sinh viên đứng ra tổng hợp tiền cho phòng 3–4 người. |
| Bối cảnh | Hóa đơn giấy, ảnh chuyển khoản và tin nhắn mua đồ chung nằm ở các nơi khác nhau. |
| Quy trình hiện tại | Nhắc gửi hóa đơn → tìm giao dịch đã ứng → nhập và đối chiếu từng khoản → tính phần của mỗi người → gửi bảng và theo dõi chuyển tiền. |
| Bottleneck | Bước 3: **35 phút/tuần theo quy trình ước lượng** để đọc ảnh, phân biệt chi chung với chi riêng và nhập tay; cần kiểm chứng bằng một tuần hóa đơn thật. |
| Impact | Một khoản không được ghi sẽ làm sai số tiền mỗi người phải trả; con số tiền thất thoát hàng tháng chưa có chứng từ để khẳng định. |
| Success metric | Baseline nháp: 35 phút đối soát/tuần. Target thử: dưới **10 phút** trên cùng một bộ chứng từ, và tổng tiền chia phải khớp tổng chi được xác nhận. Bấm giờ và đối chiếu tổng hai chiều. |
| Phương án không dùng AI | Dùng một biểu mẫu gửi chi phí chung theo đợt cuối tuần, có người ứng, số tiền, ảnh và xác nhận của người khác. |
| Giả thuyết về AI | Có thể trích số tiền/ngày từ ảnh để giảm gõ tay, nhưng người đứng tiền vẫn xác nhận khoản nào là chi chung. |
| Cảm nhận nhanh | Thử **No AI/Rule** trước; ảnh mờ và giao dịch riêng là ranh giới phải kiểm tay. |

Quy trình nháp hiện tại (**90 phút/tuần là ước lượng của tình huống**, chưa bấm giờ):

```text
Nhắc các bạn gửi chứng từ (10 phút)
  → Tìm giao dịch trong lịch sử chuyển khoản (15 phút)
  → [NGHẼN] Đọc chứng từ và nhập bảng, xác định chi chung (35 phút)
  → Chia tiền, tính khoản bù trừ (15 phút)
  → Gửi bảng và theo dõi chuyển tiền (15 phút)
```

**Phản biện PM hoài nghi:** “Bảng tính chia tiền đã có. Nếu không ai ghi khoản chi lúc phát sinh thì cuối tuần vẫn thiếu dữ liệu.” Tôi sửa phạm vi từ “công cụ chia tiền” sang **bước gom chứng từ và xác nhận chi chung theo đợt**. Cách thử là dùng lại bảng tính hiện có, không xây ứng dụng mới trong bốn giờ lab.

### Problem Card #3 — Kiểm tra bài nộp trước hạn

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị đẩy bài lab lên GitHub, tôi muốn biết từng tệp và mục bắt buộc đã có hay chưa, để không bỏ sót minh chứng dù phần code đã chạy xong. |
| Actor | Tôi, người nộp bài lab có nhiều loại tệp. |
| Bối cảnh | Hướng dẫn nằm trong nhiều file; bài Day 01 có notebook, báo cáo và ảnh tính tay. |
| Quy trình hiện tại | Đọc hướng dẫn → rà file và output → commit/push → phát hiện hoặc được nhắc về mục thiếu → bổ sung bằng commit sau. |
| Bottleneck | Bước 2: so khớp các yêu cầu với file thực tế. **20 phút** là thời gian giả định để lập kế hoạch đo; chưa có số phút thật. |
| Impact | Day 01 đã có **1 ảnh minh chứng được thêm sau** các commit nội dung chính. Nếu chỉ xem commit đầu, bài chưa đủ thành phần. |
| Success metric | Baseline quan sát ở Day 01: **1 mục bổ sung sau**. Target cho bài tiếp theo: **0 mục bắt buộc bị phát hiện thiếu sau lần kiểm cuối**. Đo bằng checklist đối chiếu yêu cầu và lịch sử commit. |
| Phương án không dùng AI | Checklist một trang với đường dẫn tệp, trạng thái và link minh chứng; tích xong rồi mới push bản nộp. |
| Giả thuyết về AI | Có thể hỗ trợ đọc hướng dẫn để gợi ý checklist, nhưng phải tự mở tệp và đối chiếu; AI không xác nhận “đủ bài” thay người nộp. |
| Cảm nhận nhanh | **No AI** là điểm xuất phát; nếu checklist thường thiếu yêu cầu vì nhiều tài liệu thì mới thử hỗ trợ trích yêu cầu. |

Quy trình nháp hiện tại (các mốc phút là **ước lượng cần đo**, riêng việc bổ sung ảnh là sự kiện đã có trong lịch sử commit):

```text
Đọc lại yêu cầu trong nhiều file (15 phút)
  → [NGHẼN] So từng yêu cầu với file và output (20 phút)
  → Commit và kiểm tra trang GitHub (10 phút)
  → Phát hiện ảnh còn thiếu, tìm và bổ sung ảnh (thời gian chưa đo)
  → Kiểm tra lại bản nộp (5 phút)
```

**Phản biện PM hoài nghi:** “Một lần quên ảnh chưa chứng minh đây là vấn đề lặp lại; có thể chỉ cần checklist giấy.” Tôi sửa metric từ “tiết kiệm thời gian” chưa có baseline sang **số mục thiếu được phát hiện sau kiểm cuối**. Tôi sẽ thử checklist không dùng AI trước và chỉ mở rộng nếu còn bỏ sót ở những bài có nhiều tệp.

### Card tôi muốn pitch nhất

- **Card #1 — Bắt đầu ôn thi khi đích còn xa.** Đây là trải nghiệm rõ nhất tôi đã nêu: trì hoãn 1–2 tuần. Tôi muốn nhóm phản biện cơ chế nào tác động vào việc bắt đầu, trước khi bàn tới ứng dụng hay AI.
- **Câu hỏi tôi chuẩn bị hỏi nhóm:** “Nếu tôi hoàn thành một phiên 25 phút chỉ để lấy thưởng nhưng vẫn không tiến gần phần kiến thức cần thi, metric nào sẽ chỉ ra việc đó?”

### Tôi đã dùng AI ở CP1–CP2 như thế nào

AI giúp sắp các ý thành Job Story, tách “điểm nghẽn” khỏi ý tưởng giải pháp và đóng vai PM hoài nghi. Tôi giữ lại phản biện về **đầu việc quá lớn** ở card ôn thi; các số phút chưa có log được ghi là ước lượng, không trình bày thành kết quả phỏng vấn. Ba card này là bản chuẩn bị để pitch, không phải quyết định cuối của nhóm.

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

Phần này cần điền theo buổi làm nhóm thực tế: card đã pitch, câu hỏi tôi đã hỏi và nhận, kiểm chứng tôi trực tiếp làm, chỗ nhóm đổi ý. Tôi chưa ghi một hoạt động là “đã làm” khi chưa có ghi chép hoặc bằng chứng từ buổi nhóm.

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI thiếu hoặc sai ở đâu? | Tôi đã kiểm tra/sửa gì? |
|---|---|---|---|---|
| CP1 | Hỗ trợ trình bày các tình huống tôi nêu và gợi ý thêm góc nhìn. | Chuyển vấn đề thành Job Story, tránh nêu giải pháp trước. | Không thể tự biết thời gian hay tần suất thật của tôi và người khác. | Gắn nhãn ước lượng; chỉ giữ sự kiện trì hoãn 1–2 tuần và lịch sử repo Day 01 là dấu hiệu đã có. |
| CP2 | Đóng vai PM hoài nghi với ba card. | Hỏi đúng điểm chưa chắc ở bước bắt đầu học, gom chứng từ và tính lặp lại của việc sót tệp. | Có thể đề xuất ngay app/phần thưởng khi chưa biết cơ chế nào có tác dụng. | Chuyển các ý tưởng đó thành giả thuyết để thử, ưu tiên No AI hoặc Rule. |

## 6. Reflection (CP7)

Phần này tôi sẽ tự viết sau khi đối chiếu ghi chép buổi nhóm. Theo yêu cầu của lab, câu trả lời 6.1–6.6 phải dựa trên trải nghiệm thật của tôi và có ít nhất 200 từ; AI không viết thay phần reflection.

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào nghĩ giải pháp trước khi hiểu vấn đề không? Nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Một lần cụ thể là gì?**

**6.4. Kết quả kiểm chứng hoặc research có làm tôi bất ngờ không?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì và phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Tôi tự giải thích chuỗi problem → quy trình → metric → boundary → mức can thiệp AI → quyết định của bài nhóm bằng 5–8 câu:**

## 7. Tài liệu tham khảo

- [CHECKPOINTS.md](../../CHECKPOINTS.md), [RULES.md](../../RULES.md), [RUBRIC.md](../../RUBRIC.md) của lab Day 02.
- [Repo Day 01 của tôi](https://github.com/manhtuongqt/K5-L3A-DAY01-NguyenManhTuong-2A202603646-AIFoundation): dùng để đối chiếu sự kiện bổ sung ảnh minh chứng.
