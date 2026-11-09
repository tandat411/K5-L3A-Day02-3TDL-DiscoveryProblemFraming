# Báo cáo cá nhân — Nguyễn Thùy Lam

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Thùy Lam
- MSSV:2A202603026
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: 3TDL
- Link repo nhóm: https://github.com/tandat411/K5-L3A-Day02-3TDL-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

Nhân vật: Lam, nhân viên Cybersecurity của một công ty công nghệ, phụ trách kiểm tra bảo mật các website của công ty trong phạm vi được giao. Lam sử dụng công cụ quét kết hợp kiểm tra thủ công, xác minh cảnh báo, tổng hợp bằng chứng và lập báo cáo lỗ hổng cho đội phát triển. Sau khi đội phát triển sửa lỗi, Lam kiểm tra lại và cập nhật trạng thái xử lý.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi website có phiên bản mới, tôi muốn thực hiện đầy đủ các bước kiểm tra bảo mật định kỳ, để phát hiện lỗi phát sinh sau thay đổi. | Lam; đội phát triển | Lam chạy lại các công cụ, kiểm tra từng mục trong checklist rồi sao chép kết quả vào bảng theo dõi sau mỗi đợt phát hành. Thời gian thao tác ước tính: 2–4 giờ cho một website mỗi đợt phát hành, chưa tính thời gian chờ công cụ quét. |
| 2 | Tốn thời gian | Khi công cụ quét đưa ra cảnh báo, tôi muốn xác định cảnh báo nào là lỗ hổng thực sự, để đội phát triển tập trung xử lý đúng lỗi. | Lam; đội phát triển | Lam phải mở từng cảnh báo và kiểm tra thủ công; có cảnh báo sau khi xác minh không phải lỗi nhưng vẫn mất thời gian điều tra. Thời gian ước tính: 15–30 phút cho một cảnh báo đơn giản, kể cả cảnh báo cuối cùng được xác định là không phải lỗi. |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận kết quả từ nhiều công cụ kiểm tra, tôi muốn gom các phát hiện trùng nhau và liên kết bằng chứng, để có danh sách lỗ hổng rõ ràng. | Lam; nhóm bảo mật | Cùng một lỗi xuất hiện trong nhiều kết quả quét; Lam phải đối chiếu URL, tham số và bằng chứng để tránh ghi nhận trùng. Thời gian ước tính: 45–60 phút cho một đợt tổng hợp khoảng 20 cảnh báo. |
| 4 | Tốn thời gian | Khi xác nhận một lỗ hổng, tôi muốn lập báo cáo đầy đủ bằng chứng, các bước tái hiện và ảnh hưởng, để đội phát triển hiểu và sửa được lỗi. | Lam; lập trình viên phụ trách | Lam chụp ảnh, chép thông tin từ công cụ và viết lại các bước kiểm tra; lập trình viên phải hỏi bổ sung nếu báo cáo thiếu chi tiết. Thời gian ước tính: 45–90 phút cho một báo cáo lỗ hổng đã xác minh, chưa tính thời gian xác minh trước đó. |
| 5 | Pain từ người khác | Khi lập trình viên nhận báo cáo nhưng không tái hiện được lỗi, tôi muốn cung cấp đủ điều kiện và bằng chứng liên quan, để hai bên thống nhất cách kiểm tra và xử lý. | Lập trình viên; Lam; người phụ trách sản phẩm | Lập trình viên trả lại yêu cầu với phản hồi “không tái hiện được”; Lam phải trao đổi thêm hoặc cùng kiểm tra trực tiếp. Thời gian trao đổi hoặc kiểm tra cùng nhau ước tính: mỗi người mất thêm 20–40 phút cho một trường hợp, chưa tính thời gian chờ phản hồi. |
| 6 | Lặp lại | Khi đội phát triển thông báo đã sửa lỗi, tôi muốn kiểm tra lại và cập nhật trạng thái cùng bằng chứng mới, để xác nhận lỗ hổng đã được xử lý. | Lam; đội phát triển; quản lý bảo mật | Lam mở lại từng báo cáo, thực hiện lại các bước tái hiện rồi cập nhật kết quả vào bảng theo dõi. Thời gian ước tính: 15–30 phút cho một lỗ hổng đơn giản mỗi lần kiểm tra lại. |


**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Giữ tình huống Security theo lựa chọn cuối trong chat; các ý về HR, thực đơn và đóng gói đã được cân nhắc rồi thay thế trong bản scan này. AI hỗ trợ tách 6 problem, viết Job Story và bổ sung thời gian ước tính.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)
### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Lập báo cáo lỗ hổng đã xác minh mất nhiều thời gian (CP1 #4). | Đầu vào và đầu ra rõ; ước tính 45–90 phút/báo cáo; ảnh hưởng trực tiếp đến khả năng tiếp nhận và sửa lỗi của lập trình viên. | Mỗi tuần có bao nhiêu báo cáo? Thời gian chủ yếu nằm ở gom bằng chứng hay viết nội dung? Mẫu báo cáo có đủ để giảm thời gian không? |
| 2 | Xác minh từng cảnh báo từ công cụ quét mất nhiều thời gian (CP1 #2). | Ước tính 15–30 phút/cảnh báo đơn giản; cảnh báo không phải lỗi vẫn tiêu tốn công sức điều tra. | Tỷ lệ cảnh báo không phải lỗi là bao nhiêu? Loại cảnh báo nào gặp thường xuyên? Có đủ bằng chứng để hỗ trợ xác minh không? |
| 3 | Đối chiếu và loại bỏ phát hiện trùng giữa nhiều công cụ còn thủ công (CP1 #3). | Ước tính 45–60 phút/đợt khoảng 20 cảnh báo; có thể làm tăng số đầu việc nếu một lỗi bị ghi nhận nhiều lần. | Đang sử dụng những công cụ nào? Bao nhiêu cảnh báo thực sự trùng? Có thể ghép bằng quy tắc đơn giản đến mức nào? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi xác nhận một lỗ hổng trên website công ty, tôi muốn lập báo cáo đầy đủ bằng chứng, các bước tái hiện và ảnh hưởng, để đội phát triển hiểu và sửa được lỗi. |
| Actor | Lam, nhân viên Cybersecurity; người nhận là lập trình viên phụ trách và quản lý bảo mật. |
| Thời điểm / bối cảnh | Sau khi đã xác minh lỗ hổng, trước khi chuyển việc sửa lỗi cho đội phát triển; chỉ xét website thuộc phạm vi được giao. |
| Quy trình hiện tại (3–7 bước) | 1. Mở ghi chú và kết quả xác minh; 2. Gom ảnh, thông tin yêu cầu/phản hồi và điều kiện kiểm tra; 3. Viết các bước tái hiện; 4. Viết ảnh hưởng và đề xuất xử lý; 5. Tự kiểm tra báo cáo; 6. Gửi cho đội phát triển và bổ sung khi được hỏi. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Ước tính bước 1–2: 10–20 phút; bước 3–4: 25–50 phút; bước 5–6: 10–20 phút. Tổng 45–90 phút/báo cáo, chưa tính thời gian chờ và trao đổi bổ sung sau khi gửi. |
| Impact (nếu không giải thì sao) | Lam dành nhiều thời gian viết lại và sao chép; báo cáo thiếu chi tiết có thể khiến lập trình viên hỏi lại, làm chậm việc tiếp nhận và sửa lỗi. |
| Success metric (baseline → target) | Thời gian thao tác từ bằng chứng đã xác minh đến báo cáo sẵn sàng gửi: baseline ước tính 45–90 → target không quá 30 phút/báo cáo tương đương. Theo dõi thêm số lượt yêu cầu bổ sung; không giảm thời gian bằng cách bỏ bằng chứng hoặc bước kiểm tra. So sánh ít nhất 5 báo cáo trước và 5 báo cáo thử nghiệm có độ phức tạp tương đương. |
| Phương án không dùng AI | Dùng mẫu báo cáo bắt buộc các trường; gom bằng chứng vào một thư mục theo mã lỗi; tự động điền dữ liệu có cấu trúc vào mẫu và kiểm tra trường còn thiếu. |
| Giả thuyết về AI (nếu có) | AI có thể soạn bản nháp từ bằng chứng đã được Lam xác minh và chỉ ra trường thiếu. Dữ kiện phải truy về được nguồn; chỗ thiếu để trống, không tự suy diễn kết quả hay mức ảnh hưởng. Lam duyệt trước khi gửi; chỉ sử dụng dữ liệu trong môi trường được công ty cho phép. |
| Cảm nhận nhanh | Workflow — ưu tiên chuẩn hóa thu thập bằng chứng và mẫu báo cáo; thử AI ở bước soạn nháp nếu vẫn còn tốn thời gian. |

Quy trình nháp hiện tại:

```text
Lỗ hổng đã được Lam xác minh
→ Mở ghi chú và kết quả kiểm tra
→ Gom bằng chứng và điều kiện tái hiện [bước 1–2: 10–20 phút]
→ Viết bước tái hiện, ảnh hưởng và đề xuất [bước 3–4: 25–50 phút]
→ Tự kiểm tra và gửi báo cáo [bước 5–6: 10–20 phút]
→ Nếu đội phát triển thiếu thông tin: bổ sung rồi gửi lại
(Tổng ước tính 45–90 phút, chưa tính vòng bổ sung và thời gian chờ)
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi công cụ quét đưa ra cảnh báo, tôi muốn xác định cảnh báo nào là lỗ hổng thực sự, để đội phát triển tập trung xử lý đúng lỗi. |
| Actor | Lam; nhóm bảo mật; đội phát triển nhận các lỗi đã xác minh. |
| Thời điểm / bối cảnh | Sau một lượt quét website công ty; giới hạn bản nháp ở các cảnh báo đơn giản có thể kiểm tra trong môi trường và phạm vi được giao. |
| Quy trình hiện tại (3–7 bước) | 1. Mở cảnh báo; 2. Đọc vị trí, mô tả và bằng chứng; 3. Kiểm tra lại trong môi trường được giao; 4. Đối chiếu kết quả với điều kiện của lỗi; 5. Ghi kết luận và bằng chứng, hoặc đánh dấu cần điều tra thêm. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Ước tính bước 1–2: 3–5 phút; bước 3–4: 10–20 phút; bước 5: 2–5 phút. Tổng 15–30 phút/cảnh báo đơn giản; chủ yếu ở kiểm tra và đối chiếu kết quả. |
| Impact (nếu không giải thì sao) | Hàng chờ xác minh kéo dài; cảnh báo không phải lỗi vẫn chiếm công sức; kết luận vội có thể khiến đội phát triển nhận lỗi chưa được chứng minh hoặc bỏ sót lỗi thật. |
| Success metric (baseline → target) | Thời gian thao tác xác minh cảnh báo đơn giản: baseline ước tính 15–30 → target 10–20 phút/cảnh báo. Thử trên cùng bộ tối thiểu 20 cảnh báo có kết luận được người có kinh nghiệm rà soát; theo dõi lỗi thật bị bỏ sót và cảnh báo sai bị chuyển cho đội phát triển, yêu cầu không tăng so với cách hiện tại. |
| Phương án không dùng AI | Chuẩn hóa checklist xác minh theo loại cảnh báo; tập hợp bằng chứng tại một chỗ; lưu các mẫu cảnh báo sai đã xác nhận kèm điều kiện áp dụng. |
| Giả thuyết về AI (nếu có) | AI có thể tóm tắt bằng chứng, chỉ ra dữ kiện còn thiếu và đề xuất checklist kiểm tra để Lam duyệt. AI không tự kết luận cảnh báo sai, đóng cảnh báo hoặc tự thực hiện kiểm tra trên hệ thống. |
| Cảm nhận nhanh | Chưa biết — cần xác định thời gian nằm ở đọc hiểu hay kiểm tra thực tế trước khi chọn AI. |

Quy trình nháp hiện tại:

```text
Nhận cảnh báo từ công cụ quét
→ Mở và đọc vị trí, mô tả, bằng chứng [3–5 phút]
→ Kiểm tra lại và đối chiếu điều kiện lỗi [10–20 phút]
→ Ghi kết luận cùng bằng chứng [2–5 phút]
→ Lỗi thật: chuyển sang lập báo cáo
→ Không phải lỗi: ghi lý do; chưa đủ bằng chứng: tiếp tục điều tra
(Tổng ước tính 15–30 phút/cảnh báo đơn giản)
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận kết quả từ nhiều công cụ kiểm tra, tôi muốn gom các phát hiện trùng nhau và liên kết bằng chứng, để có danh sách lỗ hổng rõ ràng. |
| Actor | Lam; nhóm bảo mật sử dụng danh sách phát hiện; đội phát triển nhận báo cáo sau xác minh. |
| Thời điểm / bối cảnh | Sau khi có kết quả từ nhiều công cụ, trước khi tạo danh sách công việc xác minh; bản nháp xét một đợt khoảng 20 cảnh báo trên cùng website và phiên bản. |
| Quy trình hiện tại (3–7 bước) | 1. Xuất và mở kết quả từng công cụ; 2. Chép thông tin vào bảng chung; 3. Chuẩn hóa tên trường, URL và tham số; 4. So sánh loại cảnh báo và bằng chứng; 5. Gom các mục trùng, giữ nguồn gốc; 6. Rà soát danh sách trước khi bàn giao xác minh. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Ước tính bước 1–2: 10–15 phút; bước 3–5: 25–35 phút; bước 6: 10 phút. Tổng 45–60 phút/đợt khoảng 20 cảnh báo; tập trung ở đối chiếu các cách mô tả khác nhau. |
| Impact (nếu không giải thì sao) | Một lỗi có thể được giao xác minh nhiều lần; số liệu bị đếm trùng. Nếu gom nhầm các lỗi khác nhau, nhóm có thể bỏ mất đầu việc cần xử lý. |
| Success metric (baseline → target) | Thời gian tổng hợp: baseline ước tính 45–60 → target không quá 20 phút/đợt khoảng 20 cảnh báo. Thử tối thiểu 3 đợt có số lượng tương đương; đối chiếu với danh sách Lam rà soát, ghi số mục trùng còn sót và số cặp bị gom nhầm; mọi nhóm phải giữ được bằng chứng gốc. |
| Phương án không dùng AI | Chuẩn hóa dữ liệu xuất; dùng quy tắc theo website, phiên bản, vị trí, tham số và loại cảnh báo để gợi ý nhóm; Lam kiểm tra trước khi gộp. Không gộp chỉ vì cùng URL. |
| Giả thuyết về AI (nếu có) | AI có thể gợi ý các cảnh báo có mô tả tương tự nhưng quy tắc chưa ghép được, kèm lý do và liên kết bằng chứng. Lam quyết định gộp; không xóa bản ghi gốc. Chỉ thử sau khi đo giới hạn của phương án dùng quy tắc. |
| Cảm nhận nhanh | Rule — thử chuẩn hóa và ghép theo quy tắc trước; cân nhắc AI cho các trường hợp chưa rõ. |

Quy trình nháp hiện tại:

```text
Kết quả từ các công cụ trên cùng website và phiên bản
→ Xuất và chép vào bảng chung [bước 1–2: 10–15 phút]
→ Chuẩn hóa, đối chiếu bằng chứng và gom mục trùng [bước 3–5: 25–35 phút]
→ Rà soát các nhóm, giữ liên kết nguồn [bước 6: 10 phút]
→ Danh sách cảnh báo để xác minh
(Tổng ước tính 45–60 phút/đợt khoảng 20 cảnh báo)
```

### Card muốn pitch nhất

- Card số: 1 — Lập báo cáo lỗ hổng đã xác minh mất nhiều thời gian (đề xuất để học viên cân nhắc).
- Vì sao: Phạm vi rõ từ bằng chứng đã xác minh đến báo cáo sẵn sàng gửi; dễ so sánh thời gian và mức đầy đủ của báo cáo; có phương án mẫu biểu để thử trước khi dùng AI.
- Câu hỏi muốn nhóm phản biện: Nút thắt chính là viết báo cáo hay thiếu bằng chứng từ lúc kiểm tra? Nếu mẫu báo cáo và điền tự động đã đủ, AI mang lại thêm giá trị gì? Đo thế nào để bảo đảm báo cáo nhanh hơn vẫn giúp lập trình viên tái hiện được lỗi?

### AI đã phản biện card thế nào

*Đây là phản biện do AI đưa ra cho bản nháp; cột Đồng ý? để học viên tự quyết định, không đại diện cho ý kiến đã xác nhận của học viên.*

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Thời gian ở CP1 chưa được đo, dễ làm baseline thiếu căn cứ. | Chờ học viên xác nhận. | Ghi rõ ước tính và bổ sung cách thu thập số liệu trước/sau trong từng card. |
| Chọn AI quá sớm khi mẫu biểu hoặc quy tắc có thể đủ. | Chờ học viên xác nhận. | Bổ sung phương án không dùng AI và điều kiện mới thử AI. |
| Báo cáo nhanh hơn nhưng thiếu bằng chứng vẫn khiến lập trình viên hỏi lại. | Chờ học viên xác nhận. | Thêm theo dõi yêu cầu bổ sung và giữ bước Lam duyệt báo cáo. |
| Xác minh hoặc gom cảnh báo sai có thể làm mất lỗi thật. | Chờ học viên xác nhận. | Thêm kiểm tra chất lượng, người rà soát và giữ bằng chứng gốc; AI chỉ gợi ý. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card (CP3) | Tôi đưa ra vấn đề các hộ kinh doanh phải tự ước lượng cách đóng thùng khi chưa có quy cách đã kiểm chứng để tham khảo. | Ý tưởng được đưa vào nhóm vấn đề đóng gói và vận chuyển hàng thủ công sang Mỹ. |
| Phản biện bài của bạn khác (CP3) | Tôi hỏi liệu ghi chú cố định có đủ thay AI trong việc lên kế hoạch bữa ăn và có thể ghép bước hỏi thông tin khách vào luồng báo giá không. | Gợi mở việc so sánh giải pháp đơn giản và liên kết các bước công việc. |
| Nhận phản biện (CP3) | Tôi nhận câu hỏi về việc hộ kinh doanh có sợ lộ mẫu mã, giá bán khi chia sẻ dữ liệu đóng gói. | Làm rõ vấn đề quyền riêng tư khi xây dựng dữ liệu dùng chung. |
| Gom cluster / cây OST (CP3) | Tôi góp ý gom các vấn đề về đóng gói, hỏi phí ship và giấy tờ vào cùng một nhóm. | Giúp nhìn rõ các nhu cầu trong hành trình báo giá cho khách. |
| Chọn candidate problem (CP3) | Tôi tham gia trao đổi về phạm vi bài toán và góp ý tập trung vào hàng thủ công đi Mỹ. | Giữ phạm vi đề tài cụ thể hơn để nhóm tiếp tục kiểm chứng. |
| Kiểm chứng / research (CP4) | Tôi gợi ý tìm hiểu cả khó khăn của hộ kinh doanh và phía vận chuyển. | Bổ sung góc nhìn hai phía, nhất là việc NCC ngại công khai bảng giá. |
| Quy trình nhóm (CP5) | Tôi góp ý cho nhập thông tin lô hàng một lần, dùng lại khi hỏi nhiều NCC. | Hạn chế gửi lặp thông tin và hỏi bổ sung qua nhiều lượt tin nhắn. |
| Problem Statement (CP5–CP6) | Tôi góp ý nêu rõ bước ước lượng đóng gói và chờ báo giá là các điểm nghẽn. | Giúp mô tả vấn đề cụ thể hơn thay vì chỉ nói báo giá chậm. |
| Mức can thiệp AI (CP6) | Tôi góp ý dùng công thức để tính toán, AI hỗ trợ đọc báo giá và con người duyệt trước khi gửi. | Phân biệt việc có thể hỗ trợ tự động với quyết định cần người kiểm tra. |
| Quyết định (CP6) | Tôi góp ý kiểm chứng nhu cầu và sự tham gia của NCC trước khi triển khai. | Phù hợp hướng Not Yet của nhóm, ưu tiên kiểm chứng ở GĐ 0. |
| Tổng kết (CP7) | Tôi tổng hợp lại điểm nghẽn, giới hạn của AI và những giả định còn cần kiểm chứng. | Làm cơ sở viết reflection và rà soát tính thống nhất của báo cáo. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Tôi hỏi AI cách nhận diện vấn đề theo 4 lăng kính và cách viết Job Story theo mẫu “Khi… tôi muốn… để…”. | AI giải thích cách tách tình huống, nhu cầu và kết quả mong muốn, giúp tôi có cách tiếp cận để tự scan vấn đề. | Ví dụ đôi lúc quá chung, đưa giải pháp vào phần vấn đề và kèm thời gian chưa có căn cứ. | Tôi giới hạn vào bối cảnh cụ thể, chọn ý phù hợp và phân biệt thời gian ước tính với số liệu thực tế. |
| CP2 Problem Card | Tôi hỏi AI cách mô tả quy trình hiện tại, xác định bước nghẽn và đặt chỉ số so sánh trước–sau cho một Problem Card. | AI gợi ý chia quy trình thành các bước và đo thời gian ở từng bước, đồng thời xem xét phương án không dùng AI. | Gợi ý đôi lúc nghiêng ngay sang tự động hóa, chưa xét dữ liệu đầu vào và việc cần người kiểm tra. | Tôi giữ quy trình ở mức đang thực hiện, thu hẹp phạm vi và bổ sung bước con người xác nhận; các mục tiêu cần được kiểm chứng thêm. |
| CP3 Hội tụ nhóm | Tôi hỏi AI cách gom các problem có liên quan và xây tiêu chí chọn vấn đề để thảo luận với nhóm. | AI giải thích cách so sánh actor, điểm nghẽn, tác động và phạm vi thực hiện. | Một số gợi ý gom nhóm chỉ dựa vào chủ đề, chưa xét các bước trong cùng hành trình. | Tôi đối chiếu các ý đóng gói, hỏi giá và giấy tờ với quy trình thực tế; việc chọn cuối cùng vẫn do nhóm trao đổi. |
| CP4 Kiểm chứng / research | Tôi hỏi AI cách đặt câu hỏi phỏng vấn về lần gần nhất người dùng gặp vấn đề và cách tìm giải pháp đã có. | AI giúp phân biệt câu hỏi về hành vi thực tế với câu hỏi chỉ hỏi người dùng có thích ý tưởng không. | Một số câu hỏi còn dẫn dắt; thông tin công cụ được gợi ý cần kiểm tra lại nguồn. | Tôi ưu tiên hỏi cách người dùng đang làm, thời gian mất và khó khăn ở cả phía hộ kinh doanh lẫn NCC. |
| CP5 Quy trình / Problem Statement | Tôi hỏi AI cách tách thời gian thao tác với thời gian chờ và viết Problem Statement từ các bước bị nghẽn. | AI hướng dẫn liên kết actor, quy trình, ảnh hưởng và chỉ số đo thay vì chỉ mô tả “báo giá chậm”. | Gợi ý đôi lúc trộn quy trình hiện tại với quy trình tương lai và dùng số liệu chưa kiểm chứng. | Tôi tách rõ trước–sau, tập trung vào đóng gói và đối chiếu báo giá; các mốc thời gian được xem là giả định cần đo. |
| CP6 Mức can thiệp / quyết định | Tôi hỏi AI cách phân biệt Rule, Workflow và Agent, cùng tiêu chí cân nhắc Go, Not Yet hoặc No-Go. | AI giúp làm rõ công việc có thể dùng công thức, phần cần xử lý ngôn ngữ và quyết định cần con người duyệt. | Có gợi ý tự động hóa quá nhiều khi chưa rõ dữ liệu và mức sẵn sàng tham gia của NCC. | Tôi đối chiếu với hướng của nhóm: tính toán bằng công thức, AI hỗ trợ đọc/soạn nháp, người duyệt; giữ Not Yet để kiểm chứng thêm. |
| CP7 Rà soát / reflection | Tôi hỏi AI cách tự rà soát báo cáo và các câu hỏi giúp nhìn lại điều đã học, thay đổi và còn chưa chắc. | AI gợi ý kiểm tra sự thống nhất giữa problem, metric và quyết định, giúp tôi nhận ra phần cần xem lại. | AI không biết trải nghiệm của tôi nên có thể đưa nhận xét chung hoặc suy diễn đóng góp. | Tôi chỉ dùng câu hỏi làm gợi ý, đối chiếu với việc mình tham gia và tự xác nhận nội dung trước khi nộp. |


---

## 6. Reflection (CP7)


**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Tôi nhận thấy những vấn đề như đóng gói, hỏi phí ship và chuẩn bị giấy tờ có thể thuộc cùng một quy trình. Tôi cần nhìn vào người gặp vấn đề, bước bị nghẽn và ảnh hưởng thực tế trước khi nghĩ đến công cụ.

**6.2. Nhóm có lúc nào bị "solution-first" không? Nhóm xử lý thế nào?**

Tôi thấy nhóm có những ý đi thẳng vào xây chatbot hoặc chợ so giá. Nhóm đã quay lại xác định nhu cầu đóng gói, hỏi giá và giấy tờ, rồi thu hẹp phạm vi vào hàng thủ công đi Mỹ.

**6.3. Tôi có đổi ý sau khi bị phản biện không?**

Sau câu hỏi về nguy cơ lộ mẫu mã và giá bán, tôi cần xem xét kỹ hơn điều kiện chia sẻ dữ liệu đóng gói. Tôi thấy hướng chỉ chia sẻ thông số vật lý đã ẩn danh, khi hộ đồng ý, phù hợp hơn việc chia sẻ toàn bộ dữ liệu.

**6.4. Kết quả kiểm chứng có làm tôi bất ngờ không?**

Qua phần kiểm chứng trong báo cáo nhóm, tôi chú ý việc NCC không muốn công khai bảng giá dù người bán cần so sánh. Tôi hiểu rằng giải pháp phải có lợi cho cả hai phía; các số liệu hiện tại vẫn cần được đo thêm.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Tôi thấy khó ở việc mô tả điểm nghẽn cụ thể thay vì chỉ nói “báo giá chậm”. Tôi cần tách thời gian thao tác và thời gian chờ, đồng thời nêu rõ tác động và cách đo kết quả.

**6.6. Nếu làm lại, tôi sẽ đổi gì?**

Tôi sẽ ưu tiên hỏi người dùng và kiểm tra số liệu sớm hơn. Tôi cũng sẽ hỏi kỹ hơn liệu bảng tính, mẫu yêu cầu chuẩn hoặc quy tắc đơn giản đã đủ giải quyết vấn đề trước khi thêm AI.

**6.7. Hiểu bài: problem → quy trình → metric → boundary → mức can thiệp AI → quyết định.**

Tôi hiểu vấn đề nhóm chọn là hộ kinh doanh mất nhiều thời gian đóng gói và hỏi giá ship hàng thủ công sang Mỹ. Quy trình gồm xác định thông tin lô hàng, hỏi NCC, so sánh và báo giá cho khách. Tôi theo dõi các mục tiêu: báo giá dưới 4 giờ, giảm ít nhất 50% tin nhắn, lệch giá dưới 10% và tỷ lệ chốt ít nhất 30%. Các mục tiêu này cần kiểm chứng bằng dữ liệu thật. Tôi hiểu AI không tự tính tiền, tự chốt NCC hay tự gửi báo giá; con người vẫn phải duyệt. Nhóm chọn Workflow kết hợp công thức, AI và người kiểm tra. Quyết định hiện tại là Not Yet, cần kiểm chứng nhu cầu và sự tham gia của NCC trước khi triển khai.

---

## 7. Tài liệu tham khảo
- [Worksheet hướng dẫn checkpoint](../../docs/01-worksheet.md): yêu cầu về Job Story, dấu hiệu, card và checkpoint.
- [Các framework của môn học](../../docs/03-international-frameworks.md): tài liệu được báo cáo nhóm dẫn; chưa kiểm tra độc lập nội dung trong lần chỉnh sửa này.
