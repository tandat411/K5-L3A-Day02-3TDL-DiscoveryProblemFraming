# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Phạm Duy Đức
- MSSV: 2A202603611
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: 3TDL
- Link repo nhóm: https://github.com/tandat411/K5-L3A-Day02-3TDL-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi xuất hàng thủ công (gỗ, mây tre, gốm) đi quốc tế, tôi muốn biết chính xác lô hàng cần giấy tờ gì (C/O, hun trùng, khai báo gỗ/mây tre), để không bị hải quan giữ hàng | Hộ kinh doanh xuất khẩu nhỏ | Hàng tháng: thường mất 2 -3 ngày |
| 2 | Lặp lại | Khi nhận yêu cầu hỏi giá vận chuyển từ hộ kinh doanh nhỏ, tôi muốn nhận đủ thông tin (số thùng, CBM, loại hàng, địa chỉ Mỹ) ngay từ đầu, để báo giá nhanh mà không tốn công hỏi đi hỏi lại | Nhà cung cấp vận chuyển (Forwarder nhỏ) | Hàng tháng: thường mất 10 - 12 giờ |
| 3 | Pain từ người khác | Sếp của một công ty cần có bản tóm tắt (kế hoạch, dự trù) ngắn gọn ngay sau cuộc họp | doanh nghiệp | Hàng tuần: cần mất 1 - 2 giờ |
| 4 | Lặp lại | Sinh viên cần có kế hoạch lịch trình học trước kỳ thi để đạt kết quả cao | Sinh viên | Hàng tuần: mất khoảng 5 - 7 tiếng |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Nhân viên cần chuẩn bị bản báo cáo (doanh thu, đánh giá nhân viên) trước cuộc họp đầu tuần | Nhân viên, PM | Hàng tuần: mất khoảng 2 - 3 giờ |
| 6 | Tốn thời gian | Sinh viên cần có không gian, môi trường học tập vào cuối tuần | Sinh viên | Hàng tháng: mất khoảng 3 - 4 ngày |
| 7 |Lặp lại | Bà nội trợ cần một danh sách các thứ cần chi tiêu vào đầu tháng | gia đình| Hàng tuần: mất khoảng 2 - 3 giờ |
| 8 | Tốn thời gian | Giáo viên cần hệ thống ghi chép các hoạt động của lớp (điểm số, phê bình) để họp vào cuối tuần | Lớp học | Hàng tuần: thường mất khoảng 1 - 2 giờ |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Các ý tưởng 1 và 2 tôi được AI gợi ý mà tôi giữ lại, không bỏ ý từ ý tưởng ban đầu

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Khi xuất hàng thủ công (gỗ, mây tre, gốm) đi quốc tế, tôi muốn biết chính xác lô hàng cần giấy tờ gì (C/O, hun trùng, khai báo gỗ/mây tre), để không bị hải quan giữ hàng | Các thương nhân cần tiết kiệm thời gian, tiền bạc để vận hành các công đoạn khác | thủ tục pháp lý liên quan|
| 2 | Khi nhận yêu cầu hỏi giá vận chuyển từ hộ kinh doanh nhỏ, tôi muốn nhận đủ thông tin (số thùng, CBM, loại hàng, địa chỉ Mỹ) ngay từ đầu, để báo giá nhanh mà không tốn công hỏi đi hỏi lại | Tối ưu thời gian, công đoạn vận hành, đảm bảo trải nghiệm phục vụ khách hàng | rào quản thuế quan, ngôn ngữ |
| 3 | Nhân viên cần chuẩn bị bản báo cáo (doanh thu, đánh giá nhân viên) trước cuộc họp đầu tuần | Nhu cầu tối ưu nội dung, tinh gọn thời gian họp, đảm bảo kết quả công ty | đảm bảo về nội dung, dữ liệu cá nhân |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi xuất hàng thủ công (gỗ, mây tre, gốm) đi quốc tế, tôi muốn biết chính xác lô hàng cần giấy tờ gì (C/O, hun trùng, khai báo gỗ/mây tre), để hông bị hải quan giữ hàng |
| Actor | Hộ kinh doanh xuất khẩu nhỏ |
| Thời điểm / bối cảnh | Vào đầu tháng, vào lúc 10h00 |
| Quy trình hiện tại (3–7 bước) | 1. Tìm thông tin từ bên nhà cung cấp - 2. Liên hệ với bên cung cấp - 3. Tìm hiểu quy định quốc gia gửi - 4. Báo lại với khách hàng thông tin - 5. Tiến hành các bước đóng gói |
| Bottleneck (bước nào, mất bao nhiêu phút) | 3. Tìm hiểu quy định quốc gia gửi, mất khoảng 2 - 3 giờ |
| Impact (nếu không giải thì sao) | Mất khoảng thời gian tương đương 2 - 3 ngày theo tháng|
| Success metric (baseline → target) | Tổng thời gian xuống 2 - 3 giờ |
| Phương án không dùng AI | Google + giấy tờ pháp lý |
| Giả thuyết về AI (nếu có) | AI tự đưa ra luật khoogn có thật |
| Cảm nhận nhanh | Agent |

Quy trình nháp hiện tại:

```HIỆN TẠI — 5 giờ

[1 Tìm thông tin từ bên nhà cung cấp: 1h] → [2 Liên hệ với bên cung cấp: 30'] → [3 Tìm hiểu quy định quốc gia gửi: 2h] ← BOTTLENECK
→ [4 Báo lại với khách hàng thông tin: 30'] → [5  Tiến hành các bước đóng gói: 1h] 

```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi Khi nhận yêu cầu hỏi giá vận chuyển từ hộ kinh doanh nhỏ, tôi muốn nhận đủ thông tin (số thùng, CBM, loại hàng, địa chỉ Mỹ) ngay từ đầu, để báo giá nhanh mà không tốn công hỏi đi hỏi lại |
| Actor | Nhà cung cấp vận chuyển (Forwarder nhỏ) |
| Thời điểm / bối cảnh | Mỗi ngày, khoảng thời gian chốt đơn 18h00 |
| Quy trình hiện tại (3–7 bước) | 1. Kiểm tra thông tin khách hàng - 2. Liên hệ lại để chốt đơn - 3. Tiến hành chọn nhà vận chuyển - 4. Tiến hành đóng gói |
| Bottleneck (bước nào, mất bao nhiêu phút) | Liên hệ lại để chốt đơn, mất khoảng 4 - 6 giờ |
| Impact (nếu không giải thì sao) | Mất khoảng 10 - 12 giờ để chốt lại đơn hàng |
| Success metric (baseline → target) | Tổng thời gian xuống tầm 4 - 6 giờ |
| Phương án không dùng AI | Thông qua công cụ mạng xã hội |
| Giả thuyết về AI (nếu có) | AI tự đưa ra yêu cầu |
| Cảm nhận nhanh | Agent |

Quy trình nháp hiện tại:

```HIỆN TẠI — 6 giờ

[1 Kiểm tra thông tin khách hàng: 1h] → [2 Liên hệ lại để chốt đơn: 4h] ← BOTTLENECK 
→ [3 Tiến hành chọn nhà vận chuyển: 30']
→ [4 Tiến hành đóng gói: 30'] 
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi muốn nộp báo cáo hàng tuần, tôi muốn bản tóm tắt ngắn gọn, xúc tích, để PM hiểu các vấn đề tồn đọng |
| Actor | Doanh nghiệp |
| Thời điểm / bối cảnh | Vào thứ 2, lúc 10h00 |
| Quy trình hiện tại (3–7 bước) | 1. Tìm kiếm tài liệu buổi họp - 2. Viết prompt để AI tạo bản tóm tắt - 3. Chỉnh sửa các phần thiếu - 4. Đánh giá lại tổng thể - 5. Gửi Email |
| Bottleneck (bước nào, mất bao nhiêu phút) | 3. Chỉnh sửa các phần thiếu, thường mất khoảng 30 - 60 phút |
| Impact (nếu không giải thì sao) | Mất khoảng 2 - 3 giờ tóm tắt kỹ |
| Success metric (baseline → target) | Tổng thể giảm xuống 30 - 45 phút|
| Phương án không dùng AI | Sử dụng bản giấy ghi chép, record buổi họp trước |
| Giả thuyết về AI (nếu có) | AI tự tạo bản sao lưu tóm tắt |
| Cảm nhận nhanh | Agent |

Quy trình nháp hiện tại:

```HIỆN TẠI — 1 giờ

[1 Tìm kiếm tài liệu buổi họp: 5'] → [2 Viết prompt để AI tạo bản tóm tắt: 10'] → [3 Chỉnh sửa các phần thiếu: 30'] ← BOTTLENECK
→ [4 Đánh giá lại tổng thể: 10'] → [5 Gửi Email: 5'] 

```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Vấn đề mà nhiều tiểu thương quan tâm khi vận chuyển đơn hàng xa, giải quyết bài toán logistic hiệu quả
- Câu hỏi muốn nhóm phản biện: Cần đưa ra biện pháp tối ưu lại hệ thống

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Điểm yếu liên quan đến pháp lý, bảo mật, ảo giác AI | Đồng ý | thay thế phần quyết định liên quan đến pháp lý của AI |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Tôi đã đưa ra 2 card vấn đề vào bàn bạc | nhận lại được 2 câu hỏi vấn đề, không ảnh hưởng tới nhóm|
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: "Người dùng có kiên nhẫn nhập lại nguyên liệu tồn trong tủ lạnh mỗi tối không? | nhận ra được kiến thức liên quan câu hỏi |
| Nhận phản biện | Câu hỏi tôi nhận được: Quy định hải quan Mỹ thay đổi liên tục, nếu AI tư vấn sai thì ai chịu trách nhiệm? | Tôi đã sửa gì: Vấn đề này liên quan đến pháp lý các quốc gia khác nhau |
| Gom cluster / cây OST | Tôi đã đưa ra cluster liên quan đến thông tin các hộ kinh doanh nhỏ lẻ, kênh phân phối | Tối ưu bài toán kinh doanh |
| Chọn candidate problem | Nhóm thống nhất vấn đề pháp lý cần được nghiên cứu, AI hỗ trợ phụ | Vấn đề được đặt ra về AI trong việc phân tích luật |
| Kiểm chứng / research | Tôi so sánh với với các đơn vị truyền thống như Zalo, đối thủ Easyship | đưa ra giải pháp thay thế các bước tìm kiếm bên dịch vụ |
| Quy trình nhóm | Tiến hành liên hệ bên nhà vận chuyển => tìm hiểu luật quốc tế => trao đổi thông tin với khách hàng | Thông tin phản hổi của khách hạn chế |
| Problem Statement | Khách hàng đóng mắt xích quan trọng về thời gian | Không thể dùng AI |
| Mức can thiệp AI | Mức cơ bản | Agent trong khoản đóng gói |
| Quyết định | Áp dụng AI mức tối thiểu | Cần số liệu đo đạc thực tế |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Sử dụng AI đưa ra các chủ đề mới | Đưa ra các đề tài thực tế | Chưa thể giải quyết bài toán luật | Tôi bổ sung các ý kiến mới |
| CP2 Problem Card | AI đưa ra hoàn cảnh khó khăn | Cho tôi gợi ý về thời gian| Tự tính toán thời lượng chưa có số liệu | Hiểu rõ các mốc thời gian |
| CP4 Research | Nhờ AI đưa ra các đối thủ cạnh tranh | Đề cập các bài toán thực tế | Chưa có thống kê chi tiết | Thay đổi, loại bỏ 1 vài đối tượng không phù hợp |
| CP5 Quy trình | Nhờ AI đưa quy trình phù hợp với bài toán cụ thể | Quy trình rõ ràng | Tuy nhiên 1 vài quy trình cần do con người quyết định | thay đổi quyền hạn AI |
| CP5–6 Problem Statement | Nhờ AI đánh giá lại metrics và tối ưu | Đưa ra 1 vài gợi ý về vấn đề mở rộng| Mới đề cập các chủ đề nông | Tôi bổ sung một vài yếu tố quyết định của bài toán |
| CP6 Mức can thiệp / quyết định | So sánh lợi ích khi áp dụng bài toán tối ưu | Yếu tố con người được nhắc đến | AI chưa phân biệt được rủi ro khi sử dụng dữ liệu cá nhân | Kết luận not yet |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
- Nhận ra rằng các vấn đề không chỉ xoay quanh khía cạnh cá nhân (như quản lý thời gian, thói quen học tập) mà còn mở rộng ra các bài toán vận hành phức tạp trong doanh nghiệp nhỏ và chuỗi cung ứng (như thủ tục hải quan, phối hợp liên phòng ban).

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
- Ở giai đoạn đầu, nhóm thường có xu hướng lao ngay vào việc nghĩ xem “Sẽ dùng mô hình AI gì?”, “Viết code Agent ra sao?” (ví dụ như nghĩ ngay đến việc dựng tool tra cứu hoặc viết prompt phức tạp) trước khi mổ xẻ kỹ xem nguyên nhân gốc rễ của nút cổ chai nằm ở đâu. Nhóm đã xử lý bằng cách quay ngược lại bước phân tích bottleneck (ví dụ: xác định rõ khâu tra cứu quy định tốn 2-3 giờ), từ đó mới thiết kế giải pháp AI bám sát vào đúng điểm nghẽn đó.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
- Tôi lấy ví dụ trong bài toán xuất khẩu hàng thủ công đi quốc tế, ban đầu tôi cho rằng khâu liên hệ và thu thập thông tin từ nhà cung cấp (Bước 1 & 2) là phức tạp nhất vì mất nhiều thời gian chờ đợi. Sau khi nghe phản biện và mổ xẻ lại thời gian thực tế, nhóm nhận ra khâu "Tìm hiểu quy định quốc gia gửi" (Bước 3) mới là nút cổ chai chí mạng (chiếm 2-3 giờ và tiềm ẩn rủi ro giữ hàng cao nhất). Từ đó, tôi đã thay đổi trọng tâm: chuyển từ việc tập trung tối ưu hóa giao tiếp với nhà cung cấp sang xây dựng hệ thống tự động tra cứu và kiểm chứng quy định pháp lý quốc tế.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
- Tôi bất ngờ vì các tác vụ tưởng chừng nhỏ nhặt (như tìm kiếm quy định C/O, hun trùng hay viết prompt chỉnh sửa báo cáo thủ công) lại ngốn một lượng thời gian lớn hơn nhiều so với dự tính ban đầu trong một chu kỳ tuần/tháng. "Ảo giác của AI" (Hallucination) khi nghiên cứu giải pháp, nhận ra rằng việc ứng dụng AI vào các lĩnh vực đòi hỏi tính chính xác pháp lý (như thủ tục hải quan, xuất nhập khẩu) rất nguy hiểm nếu AI tự bịa ra luật, từ đó thấy được tầm quan trọng sống còn của việc thiết kế cơ chế kiểm soát dữ liệu (Grounding).

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
- Thách thức lớn nhất là diễn đạt đúng trọng tâm "Pain Point" mà không bịa đặt hoặc ngầm định sẵn giải pháp bên trong câu phát biểu vấn đề. Việc gắn liền vấn đề với một con số cụ thể (thời gian mất đi, tần suất xảy ra) để thấy rõ mức độ nghiêm trọng thay vì chỉ dùng cảm tính ("mất thời gian", "khó khăn").

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

- Nếu làm lại tôi, sẽ thu thập dữ liệu và đo lường thời gian thực tế của từng bước ngay từ ngày đầu tiên thay vì ước lượng cảm tính, giúp việc xác định bottleneck chính xác hơn.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

--- Từ bài toán các hộ bán hàng thủ công từ VN sang Mỹ gặp khó khăn khi xin và đối chiếu báo giá vận chuyển từ nhiều nhà cung cấp. về quy trình đòi hỏi người bán phải ước lượng cách đóng gói, gửi và đợi các nhà cung cấp phản hồi để báo giá cho khách. Điểm mấu chốt là cung cấp thông tin nhiều lần và có thể không cùng định dạng, metric thì đo thời gian lúc có giá, số tin nhắn với nhà cung cấp, boundary do AI không được tự chốt phí, làm việc liên quan đến giấy tờ, hay gửi báo giá nếu chưa được kiểm tra. Sau đó đưa mô hình AI xử lý


## 7. Tài liệu tham khảo

-  - Easyship: https://www.easyship.com
  - Flexport: https://www.flexport.com
  - Tài liệu hướng dẫn và Framework quốc tế của môn học: [docs/01-worksheet.md](../../docs/01-worksheet.md), [docs/03-international-frameworks.md](../../docs/03-international-frameworks.md).
  - Canvas phân tích đề tài nhóm 3TDL — *Báo Giá Liền Tay: báo giá vận chuyển trong vài phút cho hộ làm hàng thủ công bán sang Mỹ*: https://gemini.google.com/share/c8c627a09658
