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
| 5 | Lặp lại, cần tổng hợp nhiều nguồn | Khi nhiều môn cùng giao bài trong một tuần, tôi muốn biết bài nào đến hạn trước và cần làm bước nào hôm nay, để không tới sát giờ nộp mới phát hiện còn việc chưa xong. | Sinh viên đang học nhiều môn và có bài tập, bài lab cùng lúc. | Tôi đang làm bài Day 01 và Day 02 trong hai repo khác nhau; đây là **2 đầu việc học tập** cần theo dõi. Tôi chưa ghi nhật ký số lần quên hạn hoặc số phút lập lịch, nên chưa coi việc trễ hạn là kết quả đã đo. |

**Cách tôi dùng gợi ý từ AI:** Tôi không đưa ý tưởng “làm chatbot học tập” vào bảng vì đó là cách giải quyết, chưa chỉ ra bước nào trong việc học đang nghẽn. Tôi giữ vấn đề học bị trì hoãn vì đã nêu được khoảng chậm 1–2 tuần của mình. Các tình huống còn lại là hướng để khảo sát thêm, chưa phải kết quả phỏng vấn. Những con số dự tính trong quy trình chỉ là điểm xuất phát để bấm giờ khi kiểm chứng.

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Vì sao tôi chọn ba vấn đề này

| Thứ tự | Vấn đề | Lý do chọn | Điều chưa chắc |
|---:|---|---|---|
| 1 | Bắt đầu ôn thi khi hạn còn xa (#1) | Đây là trải nghiệm tôi nêu rõ nhất: chậm 1–2 tuần. Có thể kiểm tra bằng ngày bắt đầu học và số phiên học hoàn thành. | Cơ chế phần thưởng có thực sự giúp bắt đầu hay chỉ làm tôi phân tâm? |
| 2 | Đối soát tiền sinh hoạt phòng trọ (#2) | Actor, dữ liệu đầu vào và điểm nghẽn gom chứng từ đều cụ thể. Có thể thử trên một bộ hóa đơn mẫu trong buổi lab. | Thời gian 35 phút ở bước đối soát cần đo lại với người thực sự đang giữ tiền. |
| 3 | Sắp thứ tự bài tập trong tuần (#5) | Khác với card #1 về bắt đầu ôn thi dài hạn, card này tập trung vào các hạn nộp gần và việc chọn bước tiếp theo trong ngày. Có thể thử bằng lịch bài tập một tuần. | Chưa có nhật ký số lần quên hạn hay thời gian lập lịch để làm baseline. |

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
| Việc con người phải làm | Tôi chọn môn và phần kiến thức thật sự cần ôn, kiểm tra đầu việc AI gợi ý có khớp đề cương, tự bắt đầu phiên học và ghi lại mình đã học được gì. Tôi tự quyết định phần thưởng sau khi hoàn thành việc học, không giao việc đánh giá tiến độ cho AI. |
| Ranh giới và cách quay lại | Nếu AI chia sai chương hoặc gợi ý việc quá lớn, tôi dùng đề cương gốc để chia lại trên giấy. Không để AI tự đổi lịch thi hay đánh dấu một phiên là đã học. |
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
| Việc con người phải làm | Người ứng tiền xác nhận hóa đơn nào là chi chung, cả phòng thống nhất cách chia, người tổng hợp rà lại tổng chi và số tiền mỗi người phải trả trước khi gửi. Mỗi người tự xác nhận phần của mình; AI không được tự kết luận ai đang nợ. |
| Ranh giới và cách quay lại | AI chỉ được đề xuất số tiền và ngày từ ảnh. Ảnh mờ hoặc số tiền không khớp thì nhập tay và hỏi lại người đã chi. Bảng đã được mọi người xác nhận mới dùng để chuyển tiền. |
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

### Problem Card #3 — Quản lý hạn bài tập trong tuần của sinh viên

| Trường | Nội dung |
|---|---|
| Job Story | Khi đầu tuần tôi nhận bài tập từ nhiều môn với hạn nộp khác nhau, tôi muốn nhìn rõ việc nào cần làm hôm nay và cần bắt đầu từ đâu, để hoàn thành từng bài trước hạn thay vì xử lý tất cả vào tối cuối cùng. |
| Actor | Sinh viên học nhiều môn, tự chịu trách nhiệm theo dõi và nộp bài. |
| Bối cảnh | Thông báo bài tập nằm ở LMS, tài liệu môn học hoặc nhóm chat; thời gian rảnh còn phải chia cho giờ học và việc cá nhân. Card này xét hạn bài tập trong tuần, không xét động lực ôn thi cuối kỳ của card #1. |
| Quy trình hiện tại | Xem thông báo từng môn → ghi nhớ hạn nộp → ước lượng khối lượng từng bài → chọn việc làm hôm nay → làm bài → kiểm lại và nộp. |
| Bottleneck | Bước 3–4: khó ước lượng việc nào tốn công và ưu tiên theo hạn gần. **15 phút** là ước lượng để thử bấm giờ, chưa phải số đo thực tế. |
| Impact | Việc gấp dễ bị lẫn với việc quan trọng; có nguy cơ dồn bài vào sát hạn. Tôi chưa có log chứng minh số lần trễ hạn. |
| Success metric | Tuần đầu ghi baseline: số bài nộp sát hạn, số lần quên hạn và phút lập kế hoạch. Target thử: **0 lần quên hạn** trong tuần tiếp theo và mỗi bài có bước đầu tiên được xếp lịch ít nhất 24 giờ trước hạn. Đối chiếu lịch với thời điểm nộp thật. |
| Phương án không dùng AI | Một bảng giấy hoặc lịch điện thoại ghi môn, hạn, việc nhỏ tiếp theo và trạng thái; mỗi tối tự rà 5 phút. |
| Giả thuyết về AI | AI có thể giúp trích hạn và đầu việc từ thông báo dài, nhưng chỉ tạo bản nháp; tôi đối chiếu lại thông báo gốc. |
| Việc con người phải làm | Tôi xác nhận hạn, tự ước lượng sức mình, chọn thứ tự ưu tiên, làm bài và kiểm tra bản nộp. Tôi quyết định đổi lịch khi có việc đột xuất. |
| Ranh giới và cách quay lại | AI không tự đổi hạn nộp, đánh dấu bài đã xong hay nộp bài thay tôi. Nếu trích sai hạn, tôi sửa trực tiếp trên lịch từ thông báo gốc. |
| Cảm nhận nhanh | **No AI/Rule** là đủ để thử trước; chỉ cân nhắc AI nếu việc đọc nhiều thông báo thật sự chiếm thời gian. |

Quy trình nháp hiện tại (phút là **ước lượng để thử đo**, chưa phải nhật ký thời gian):

```text
Xem thông báo của từng môn (10 phút)
  → Ghi hạn nộp vào lịch chung của bản thân (5 phút)
  → [NGHẼN] Ước lượng khối lượng và chọn bài cần làm trước (15 phút)
  → Chia bài ưu tiên thành bước có thể làm hôm nay (10 phút)
  → Làm bước đầu tiên (25 phút)
  → Rà hạn và cập nhật trạng thái cuối ngày (5 phút)
```

**Phản biện PM hoài nghi:** “Sinh viên đã có lịch điện thoại; khó khăn có thật sự ở việc ghi hạn hay ở việc bắt tay làm bài?” Tôi thu hẹp card vào **chọn thứ tự và bước đầu tiên cho các bài đến hạn trong tuần**. Trước tiên thử bảng lịch thủ công một tuần; nếu vẫn quên hạn hoặc không bắt đầu, cần xem lại nguyên nhân trước khi thêm AI.

### Card tôi muốn pitch nhất

- **Card #1 — Bắt đầu ôn thi khi đích còn xa.** Đây là trải nghiệm rõ nhất tôi đã nêu: trì hoãn 1–2 tuần. Tôi muốn nhóm phản biện cơ chế nào tác động vào việc bắt đầu, trước khi bàn tới ứng dụng hay AI.
- **Câu hỏi tôi chuẩn bị hỏi nhóm:** “Nếu tôi hoàn thành một phiên 25 phút chỉ để lấy thưởng nhưng vẫn không tiến gần phần kiến thức cần thi, metric nào sẽ chỉ ra việc đó?”

### Tôi đã dùng AI ở CP1–CP2 như thế nào

AI giúp sắp các ý thành Job Story, tách “điểm nghẽn” khỏi ý tưởng giải pháp và đóng vai PM hoài nghi. Ở card ôn thi, phản biện về **đầu việc quá lớn** khiến tôi tách việc chia nhỏ bài học và phần thưởng thành hai giả thuyết để thử. Ở card chi tiêu, AI chỉ được đọc thông tin sơ bộ từ chứng từ; ở card lịch bài tập, AI chỉ có thể trích thông báo để tôi kiểm lại. Tôi vẫn phải xác nhận số liệu và tự chốt quyết định. Các số phút chưa có log được ghi là ước lượng, không trình bày thành kết quả phỏng vấn. Ba card này là bản chuẩn bị để pitch, không phải quyết định cuối của nhóm.

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

Ở CP3–CP6, tôi tham gia trao đổi chung và theo dõi cách nhóm chuyển từ các ý tưởng ban đầu sang vấn đề vận chuyển của hộ bán hàng thủ công. Phần tôi tập trung là nhìn lại cách đặt vấn đề, điểm nghẽn và phạm vi con người cần tự quyết định.

| Hoạt động | Tôi đã tham gia và rút ra điều gì? | Ảnh hưởng đến cách tôi nhìn bài nhóm |
|---|---|---|
| CP3 — Hội tụ vấn đề | Tôi chuẩn bị ba Problem Card cá nhân, trong đó quan tâm nhất đến chuyện trì hoãn ôn thi. Khi tham gia trao đổi chung về hướng vận chuyển, tôi so sánh các card theo actor, bước nghẽn và dấu hiệu thực tế thay vì chọn ý tưởng nghe hấp dẫn nhất. | Tôi nhận ra một vấn đề cần được mô tả rõ trước khi bàn đến ứng dụng hay AI. |
| CP4 — Kiểm chứng | Tôi tham khảo thảo luận về việc người bán phải hỏi từng nhà vận chuyển và tự đối chiếu báo giá. Khi đọc lại báo cáo nhóm, điều tôi chú ý là chưa có số đo thực tế từ người bán. | Tôi muốn kiểm tra xem thời gian bị mất chủ yếu ở lúc chờ phản hồi hay lúc đọc và chuẩn hóa các báo giá. |
| CP5 — Quy trình và Problem Statement | Tôi tham gia trao đổi về việc mô tả quy trình từ lúc nhận yêu cầu của khách đến lúc có báo giá. Khi nghĩ về cách viết Problem Statement, tôi thấy đóng gói, hỏi giá, so phí và giấy tờ là những việc khác nhau, không nên gộp thành một điểm nghẽn chung. | Theo tôi, bài cần chọn một bước chính để đo và nói rõ ai chịu trách nhiệm ở bước đó. |
| CP6 — Mức can thiệp và quyết định | Tôi tham gia trao đổi chung về phạm vi AI có thể hỗ trợ. Tôi nghiêng về việc dùng quy tắc cho phép tính quy đổi, chỉ cân nhắc AI để đọc sơ bộ báo giá, còn người bán kiểm tra thông tin và chốt giá. | Tôi hiểu quyết định **Not Yet** trong `TEAM.md` là cần kiểm chứng với người bán và nhà vận chuyển trước khi làm tiếp. |
| CP7 — Nhìn lại bài làm | Tôi tự viết phần reflection ở mục 6, nêu cả điểm mình học được, chỗ báo cáo còn đặt vấn đề theo hướng “thiếu AI” và điều mình sẽ hỏi sớm hơn nếu làm lại. | Tôi hiểu rõ hơn rằng một ý tưởng hợp lý trên giấy vẫn cần dữ liệu thực tế trước khi kết luận. |

**Cách tôi hiểu hướng bài nhóm ở thời điểm viết:** Theo `TEAM.md`, nhóm đang xét việc hộ bán hàng thủ công cần tổng hợp thông tin đóng gói và báo giá vận chuyển trước khi trả lời khách. Tôi thấy phần việc quan trọng vẫn là của người bán: xác nhận hàng có thể gửi, tự đo kích thước và cân nặng kiện hàng, hỏi lại nhà vận chuyển khi điều kiện báo giá không rõ, kiểm tra phụ phí rồi mới quyết định giá báo cho khách. Công thức đổi đơn vị hoặc tính khối lượng quy đổi là phép tính theo quy tắc; bảng tính cũng làm được. Nếu có dùng AI, tôi chỉ đề xuất cho AI đọc sơ bộ văn bản báo giá và gợi ý đưa các dòng phí về cùng một bảng để người bán dễ kiểm tra. AI không được tự đo hàng từ ảnh, tự cam kết giá với khách hay thay nhà vận chuyển xác nhận điều kiện dịch vụ. Nếu bản trích xuất thiếu một khoản phí, người bán quay lại chứng từ gốc và nhập tay. Để biết hướng này có ích hay không, nhóm cần đo thời gian từ lúc nhận yêu cầu đến lúc có **báo giá đã được xác nhận**, cùng số lần phải hỏi lại nhà vận chuyển; hiện tôi chưa có số đo để điền baseline hoặc target thay nhóm.

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI thiếu hoặc sai ở đâu? | Tôi đã kiểm tra/sửa gì? |
|---|---|---|---|---|
| CP1 | Hỗ trợ trình bày các tình huống và gợi ý thêm góc nhìn. | Chuyển vấn đề thành Job Story, tránh nêu giải pháp trước. | Không thể tự biết thời gian hay tần suất thật của tôi và người khác. | Gắn nhãn ước lượng; chỉ coi mốc trì hoãn 1–2 tuần do tôi nêu là trải nghiệm đã xác nhận. Bốn tình huống còn lại cần khảo sát. |
| CP2 | Đóng vai PM hoài nghi với ba card. | Hỏi đúng điểm chưa chắc ở bước bắt đầu ôn thi, gom chứng từ và xếp bài theo hạn. | Có thể đề xuất ngay app/phần thưởng khi chưa biết cơ chế nào có tác dụng; không thể thay con người xác nhận giao dịch hoặc ưu tiên học tập. | Chuyển các ý tưởng thành giả thuyết để thử, ưu tiên No AI hoặc Rule. Việc học, chia tiền và lập lịch đều do con người chốt. |

## 6. Reflection (CP7)

Phần này là nhận xét của tôi sau khi xem lại bài cá nhân và tài liệu của nhóm.

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

So với hướng vận chuyển của nhóm, bài học lớn nhất tôi rút ra từ card ôn thi là không được vội vã đưa ra công cụ. Cần chỉ rõ ai là người gặp khó khăn (actor), họ bị nghẽn chính xác ở bước nào và có biểu hiện/dấu hiệu cụ thể ra sao trước khi tính đến bất kỳ giải pháp hay công nghệ nào.

**6.2. Nhóm có lúc nào nghĩ giải pháp trước khi hiểu vấn đề không? Nhóm nhận ra và xử lý thế nào?**

Khi đọc lại báo cáo của nhóm, tôi nhận thấy văn bản vẫn còn câu “hộ kinh doanh thiếu công cụ AI” — đây là cách đặt vấn đề ngược, xuất phát từ giải pháp thay vì thực tế. Trong file TEAM.md, vấn đề được mô tả đúng bản chất hơn: người bán tốn nhiều thời gian ước tính quy cách đóng gói, phải liên hệ hỏi giá từng đơn vị vận chuyển và tự đối chiếu các báo giá rời rạc. Đây là quan sát riêng của tôi khi rà soát lại bài, nhóm chưa chính thức thảo luận để chỉnh sửa câu này trong báo cáo.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Một lần cụ thể là gì?**

Tôi không có lần thay đổi quyết định đáng kể nào xuất phát từ phản biện của các thành viên trong nhóm mà tôi nhớ rõ. Tuy nhiên, ở chặng CP2, chính phản biện từ AI đã khiến tôi thay đổi góc nhìn: tôi nhận ra tính năng “phần thưởng” chỉ là một giả thuyết cần được kiểm chứng thực tế, chứ không thể mặc định xem nó là một giải pháp chắc chắn đúng.

**6.4. Kết quả kiểm chứng hoặc research có làm tôi bất ngờ không?**

Điều khiến tôi bất ngờ nhất là báo cáo của nhóm vẫn hoàn toàn thiếu các số đo và dữ liệu thực tế thu thập từ người bán. Việc này khiến tôi muốn tập trung kiểm tra tiếp bước xác thực nhu cầu thực tế của họ ở các chặng sau, thay vì giả định quy trình vận hành trên giấy tờ.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Khâu khó khăn nhất là thu hẹp phạm vi vấn đề. Đóng gói, hỏi giá, so sánh biểu phí và xử lý chứng từ hải quan là các nghiệp vụ hoàn toàn khác nhau. Một Problem Statement đạt yêu cầu bắt buộc phải cô lập đúng một điểm nghẽn then chốt, xác định một thước đo cụ thể và vạch rõ ranh giới những việc con người bắt buộc phải trực tiếp can thiệp để xác nhận.

**6.6. Nếu làm lại, tôi sẽ đổi gì và phản biện nhóm mạnh hơn ở điểm nào?**

Nếu được thực hiện lại từ đầu, tôi sẽ tìm cách tiếp cận người bán và các bên vận chuyển sớm hơn để làm rõ: họ mất nhiều thời gian nhất ở khâu chờ phản hồi hay ở khâu đọc và chuẩn hóa dữ liệu báo giá. Đồng thời, tôi sẽ phản biện quyết liệt hơn khi nhóm định nghĩa vấn đề là “thiếu AI”, bởi nhóm chưa hề chứng minh được bước nào trong luồng xử lý thực sự cần đến AI.

**6.7. Tôi tự giải thích chuỗi problem → quy trình → metric → boundary → mức can thiệp AI → quyết định của bài nhóm bằng 5–8 câu:**

1. Người bán hàng thủ công gửi hàng tuyến Việt Nam – Mỹ là đối tượng chính gặp khó khăn trong quy trình này.
2. Họ phải tự ước tính kích thước đóng gói rồi liên hệ hỏi giá riêng lẻ từng nhà vận chuyển.
3. Điểm nghẽn lớn nhất nằm ở việc phải nhập lại thông tin nhiều lần và tự đối chiếu các bảng báo giá khác nhau về định dạng lẫn đơn vị.
4. Hiệu quả cần được đo bằng thời gian từ lúc gửi yêu cầu đến khi chốt báo giá, số lần phải trao đổi lại và sai lệch chi phí thực tế, dù hiện nhóm chưa có số liệu baseline đáng tin cậy.
5. Con người bắt buộc phải tự thực hiện việc đo đạc kiện hàng thực tế, kiểm tra các khoản phụ phí phát sinh, hoàn tất giấy tờ và chốt giá cuối với khách.
6. Các quy tắc tính toán thông thường hoàn toàn đủ sức xử lý việc quy đổi đơn vị; AI nếu đưa vào chỉ đóng vai trò hỗ trợ đọc và bóc tách thông tin từ báo giá để người bán kiểm tra lại.
7. Quyết định hiện tại trong TEAM.md là "Not Yet"; toàn bộ bài toán cần được kiểm chứng trực tiếp với người bán và các đơn vị vận chuyển trước khi bắt tay thực hiện tiếp.

## 7. Tài liệu tham khảo

- [CHECKPOINTS.md](../../CHECKPOINTS.md), [RULES.md](../../RULES.md), [RUBRIC.md](../../RUBRIC.md) của lab Day 02.
