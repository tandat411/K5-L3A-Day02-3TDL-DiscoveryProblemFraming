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
| 5 | Lặp lại, pain từ người khác | Khi đến lượt dọn bếp và đổ rác trong phòng trọ ở ghép, tôi muốn mọi người thống nhất rõ ai làm việc nào trước cuối tuần, để khu sinh hoạt chung sạch mà không phải nhắc đi nhắc lại hoặc đổ lỗi cho nhau. | Những người ở cùng phòng; người thường đứng ra nhắc việc chịu thêm công điều phối. | Tình huống để khảo sát là phòng **3–4 người** với hai việc dễ bị bỏ quên: dọn bếp và đổ rác. Tôi chưa có lịch trực, tin nhắn nhắc việc hay số lần tranh cãi của một phòng cụ thể; cần hỏi và ghi lại trước khi coi đây là pain đã được xác nhận. |

**Cách tôi dùng gợi ý từ AI:** Tôi không đưa ý tưởng “làm chatbot học tập” vào bảng vì đó là cách giải quyết, chưa chỉ ra bước nào trong việc học đang nghẽn. Tôi giữ vấn đề học bị trì hoãn vì đã nêu được khoảng chậm 1–2 tuần của mình. Bốn tình huống sinh hoạt còn lại là các hướng để khảo sát thêm, chưa phải kết quả phỏng vấn. Những con số dự tính trong quy trình chỉ là điểm xuất phát để bấm giờ khi kiểm chứng.

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Vì sao tôi chọn ba vấn đề này

| Thứ tự | Vấn đề | Lý do chọn | Điều chưa chắc |
|---:|---|---|---|
| 1 | Bắt đầu ôn thi khi hạn còn xa (#1) | Đây là trải nghiệm tôi nêu rõ nhất: chậm 1–2 tuần. Có thể kiểm tra bằng ngày bắt đầu học và số phiên học hoàn thành. | Cơ chế phần thưởng có thực sự giúp bắt đầu hay chỉ làm tôi phân tâm? |
| 2 | Đối soát tiền sinh hoạt phòng trọ (#2) | Actor, dữ liệu đầu vào và điểm nghẽn gom chứng từ đều cụ thể. Có thể thử trên một bộ hóa đơn mẫu trong buổi lab. | Thời gian 35 phút ở bước đối soát cần đo lại với người thực sự đang giữ tiền. |
| 3 | Phân công dọn khu sinh hoạt chung (#5) | Một nhóm nhỏ, hai việc cụ thể và một điểm nghẽn có thể quan sát: xác định ai đang nhận việc nào. Có thể thử quy trình bằng lịch trực một tuần. | Chưa có tin nhắn nhắc việc hoặc nhật ký của một phòng thật để đo tần suất bỏ sót. |

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

### Problem Card #3 — Phân công việc chung trong phòng trọ

| Trường | Nội dung |
|---|---|
| Job Story | Khi đến lượt dọn bếp và đổ rác trong phòng trọ ở ghép, tôi muốn biết rõ ai làm từng việc và khi nào có thể đổi ca, để việc chung được xử lý mà không phải một người nhắc mãi. |
| Actor | Người ở cùng phòng và người đang đứng ra nhắc lịch dọn; người thực hiện việc dọn là người chịu trách nhiệm chính. |
| Bối cảnh | Dọn bếp sau khi nấu và đổ rác trước khi đầy là hai việc lặp lại. Lịch học và lịch làm thêm của từng người có thể khác nhau. Đây là tình huống cần hỏi phòng trọ thật trước khi kết luận. |
| Quy trình hiện tại | Nhận thấy việc chưa làm → nhắn nhóm hỏi ai rảnh → đối chiếu lịch từng người → chốt người nhận việc → người được phân công làm và báo lại. |
| Bottleneck | Bước 3: phải chờ và đối chiếu câu trả lời rời rạc để chốt người làm. **15 phút** chỉ là mức giả định để thử bấm giờ, chưa phải thời gian đã đo. |
| Impact | Nếu không ai nhận trách nhiệm, việc chung dễ bị lùi sang ngày sau và người chủ động phải nhắc lại. Chưa có bằng chứng để khẳng định số lần xảy ra hoặc mức độ mâu thuẫn. |
| Success metric | Tuần đầu đo baseline bằng số lần phải nhắc quá một lần cho cùng một việc và số phút từ lúc hỏi đến khi có người nhận. Target thử: hai việc đều có người nhận trước hạn, thời gian chốt người làm dưới **5 phút**; ghi lại bằng lịch trực và tin nhắn đã được mọi người đồng ý. |
| Phương án không dùng AI | Lập lịch trực trên giấy hoặc bảng chung; mỗi người tự chọn ca phù hợp, đổi ca phải được người còn lại đồng ý và cập nhật ngay. |
| Giả thuyết về AI | Nếu nhóm chat quá nhiều tin, AI có thể tóm tắt ai đã báo bận và những ca còn trống. Mọi phân công và đổi ca phải do người ở cùng phòng xác nhận. |
| Việc con người phải làm | Những người ở cùng phòng thỏa thuận mức công bằng, tự nhận hoặc đổi ca, thực hiện việc dọn và xác nhận đã xong. Người điều phối chỉ cập nhật lịch sau khi các bên đồng ý. |
| Ranh giới và cách quay lại | AI không tự phân việc, phán xét ai lười hoặc gửi tin nhắn nhắc hộ. Nếu bản tóm tắt bỏ sót một tin báo bận, cả phòng quay lại lịch giấy và tin nhắn gốc để chốt. |
| Cảm nhận nhanh | **No AI/Rule** là đủ cho thử nghiệm đầu. Không cần AI tự nhắn nhắc hoặc quyết định ai phải dọn. |

Quy trình nháp hiện tại (phút thao tác là **ước lượng để thiết kế cách đo**, không phải ghi nhận từ một phòng cụ thể; thời gian chờ phản hồi có thể kéo dài hơn):

```text
Thấy bếp cần dọn hoặc thùng rác đã đầy (2 phút)
  → Nhắn nhóm, hỏi lịch rảnh của từng người (3 phút)
  → [NGHẼN] Đối chiếu câu trả lời và chờ chốt người nhận (15 phút giả định)
  → Xác nhận ca trực hoặc đổi ca trên lịch chung (5 phút)
  → Người nhận việc dọn bếp/đổ rác (20 phút giả định)
  → Người đó đánh dấu đã xong; người ở cùng phòng kiểm tra (2 phút)
```

**Phản biện PM hoài nghi:** “Không có nhật ký nhắc việc thì làm sao biết đây là vấn đề của cả phòng, và một tờ lịch trực có thể đã giải quyết xong?” Tôi bỏ nhận định rằng việc dọn chung thường xuyên gây tranh cãi. Card chỉ nêu **giả thuyết** về bước chốt ca; trước tiên cần ghi một tuần xem có bao nhiêu lần phải nhắc lại. Nếu lịch trực giấy hoạt động, không cần thêm AI.

### Card tôi muốn pitch nhất

- **Card #1 — Bắt đầu ôn thi khi đích còn xa.** Đây là trải nghiệm rõ nhất tôi đã nêu: trì hoãn 1–2 tuần. Tôi muốn nhóm phản biện cơ chế nào tác động vào việc bắt đầu, trước khi bàn tới ứng dụng hay AI.
- **Câu hỏi tôi chuẩn bị hỏi nhóm:** “Nếu tôi hoàn thành một phiên 25 phút chỉ để lấy thưởng nhưng vẫn không tiến gần phần kiến thức cần thi, metric nào sẽ chỉ ra việc đó?”

### Tôi đã dùng AI ở CP1–CP2 như thế nào

AI giúp sắp các ý thành Job Story, tách “điểm nghẽn” khỏi ý tưởng giải pháp và đóng vai PM hoài nghi. Ở card ôn thi, phản biện về **đầu việc quá lớn** khiến tôi tách việc chia nhỏ bài học và phần thưởng thành hai giả thuyết để thử. Ở card chi tiêu, AI chỉ được đọc thông tin sơ bộ từ chứng từ; ở card việc nhà, AI thậm chí có thể không cần thiết. Tôi vẫn phải xác nhận số liệu và tự chốt quyết định. Các số phút chưa có log được ghi là ước lượng, không trình bày thành kết quả phỏng vấn. Ba card này là bản chuẩn bị để pitch, không phải quyết định cuối của nhóm.

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

Ở CP3–CP6, tôi tham gia **trao đổi chung** với nhóm. Tôi không nhận mình đã trực tiếp phỏng vấn, khảo sát, research nguồn hay viết các phần của `group_report.md` khi chưa có sản phẩm hoặc ghi chép chứng minh. Các card trong mục 3 là phần tôi chuẩn bị cho thảo luận cá nhân; card muốn pitch và câu hỏi ở đó là **điều tôi chuẩn bị**, không được tính là câu hỏi đã nói trong buổi nhóm.

| Hoạt động | Phần tôi có thể xác nhận | Giới hạn bằng chứng |
|---|---|---|
| CP3 — Pitch và phản biện | Tôi chuẩn bị 3 card, chọn card ôn thi để trao đổi và viết sẵn câu hỏi về việc đo tiến bộ thật thay vì chỉ đếm phiên học nhận thưởng. Tôi tham gia trao đổi chung khi nhóm hội tụ về một candidate. | Chưa có biên bản xác nhận tôi đã đặt câu hỏi nào cho bạn khác hoặc nhận câu hỏi nào từ nhóm; tôi không ghi lời phản biện giả định thành lời đã nói. |
| CP4 — Kiểm chứng và research | Tôi tham gia trao đổi chung về hướng bài nhóm. | Chưa có interview snapshot, survey hay nguồn do tôi trực tiếp kiểm và lưu lại; không nhận phần này là kết quả cá nhân của mình. |
| CP5 — Quy trình và Problem Statement | Tôi tham gia trao đổi chung, nhìn bài toán theo thứ tự người thực hiện → bước làm → bước nghẽn, thay vì bắt đầu từ tên công cụ. | Chưa có phần quy trình hoặc Problem Statement nào trong báo cáo nhóm gắn với một commit của tôi. |
| CP6 — Mức can thiệp và quyết định | Tôi tham gia trao đổi chung về phạm vi can thiệp; với phần cá nhân, tôi chọn thử No AI/Rule trước và giữ quyền chốt cho con người. | Đây không phải quyết định thay nhóm. File nhóm chưa có bảng đánh giá để tôi gán cho mình một kết luận hay metric chung. |

Tôi cần tự bổ sung câu hỏi phản biện mình **đã thực sự đặt và nhận** nếu tìm lại được ghi chép buổi nhóm. Tôi không lấy lời nói hoặc đóng góp riêng của bạn khác để điền vào dòng của mình.

**Cách tôi hiểu hướng bài nhóm ở thời điểm viết:** Theo `TEAM.md`, nhóm đang xét việc hộ bán hàng thủ công cần tổng hợp thông tin đóng gói và báo giá vận chuyển trước khi trả lời khách. Tôi thấy phần việc quan trọng vẫn là của người bán: xác nhận hàng có thể gửi, tự đo kích thước và cân nặng kiện hàng, hỏi lại nhà vận chuyển khi điều kiện báo giá không rõ, kiểm tra phụ phí rồi mới quyết định giá báo cho khách. Công thức đổi đơn vị hoặc tính khối lượng quy đổi là phép tính theo quy tắc; bảng tính cũng làm được. Nếu có dùng AI, tôi chỉ đề xuất cho AI đọc sơ bộ văn bản báo giá và gợi ý đưa các dòng phí về cùng một bảng để người bán dễ kiểm tra. AI không được tự đo hàng từ ảnh, tự cam kết giá với khách hay thay nhà vận chuyển xác nhận điều kiện dịch vụ. Nếu bản trích xuất thiếu một khoản phí, người bán quay lại chứng từ gốc và nhập tay. Để biết hướng này có ích hay không, nhóm cần đo thời gian từ lúc nhận yêu cầu đến lúc có **báo giá đã được xác nhận**, cùng số lần phải hỏi lại nhà vận chuyển; hiện tôi chưa có số đo để điền baseline hoặc target thay nhóm.

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI thiếu hoặc sai ở đâu? | Tôi đã kiểm tra/sửa gì? |
|---|---|---|---|---|
| CP1 | Hỗ trợ trình bày các tình huống và gợi ý thêm góc nhìn. | Chuyển vấn đề thành Job Story, tránh nêu giải pháp trước. | Không thể tự biết thời gian hay tần suất thật của tôi và người khác. | Gắn nhãn ước lượng; chỉ coi mốc trì hoãn 1–2 tuần do tôi nêu là trải nghiệm đã xác nhận. Bốn tình huống còn lại cần khảo sát. |
| CP2 | Đóng vai PM hoài nghi với ba card. | Hỏi đúng điểm chưa chắc ở bước bắt đầu học, gom chứng từ và phân công việc nhà. | Có thể đề xuất ngay app/phần thưởng khi chưa biết cơ chế nào có tác dụng; không thể thay con người xác nhận giao dịch hay nhận ca trực. | Chuyển các ý tưởng thành giả thuyết để thử, ưu tiên No AI hoặc Rule. Việc học, chia tiền và phân ca đều do con người chốt. |

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
