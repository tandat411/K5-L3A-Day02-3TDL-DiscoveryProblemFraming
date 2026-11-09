# Đề tài: Nền tảng báo giá vận chuyển nhanh cho hộ kinh doanh hàng thủ công xuất sang Mỹ

> Tên làm việc: **ShipQuote Craft**, tên tạm, có thể đổi.
> Mọi con số có ghi **(giả định)** là ước lượng ban đầu. Cần đo lại bằng phỏng vấn và dữ liệu thật trước khi pitch.

---

## 0. Bối cảnh và vấn đề

### Ai đang gặp vấn đề?

- **Hộ kinh doanh nhỏ làm hàng thủ công** (gốm, mây tre đan, gỗ, thêu, sơn mài…). Họ có nhiều mẫu, mỗi mẫu một kích thước. Họ muốn bán cho khách lẻ hoặc khách sỉ nhỏ ở Mỹ.
- **Nhà cung cấp vận chuyển nhỏ (NCC vận chuyển)**: công ty forwarder, đại lý chuyển phát nhanh, dịch vụ gom hàng đi Mỹ.

### Quy trình hiện tại (khi khách Mỹ hỏi giá)

```text
1. Khách Mỹ hỏi giá: "50 cái bình gốm mẫu A + 20 giỏ mây mẫu B, giao tới Texas giá bao nhiêu?"
2. Hộ kinh doanh tự đo, tự đoán cách đóng gói: bao nhiêu thùng, mỗi thùng nặng bao nhiêu?
3. Nhắn Zalo / Facebook cho 3–5 NCC vận chuyển, mỗi nơi gửi lại ảnh, kích thước, số lượng.
4. Mỗi NCC hỏi lại thông tin còn thiếu: hàng gì, có gỗ không, cần hun trùng không, giao tận nhà không…
5. Chờ báo giá, mỗi NCC báo một kiểu (theo kg, theo CBM, có hoặc chưa có phụ phí, thuế).
6. Hộ kinh doanh tự quy đổi, so sánh, cộng thêm giá hàng, rồi mới báo cho khách Mỹ.
7. Khách đợi lâu thì chuyển sang người bán khác.
```

### Điểm nghẽn

| Bước | Vấn đề | Dấu hiệu cần đo |
|---|---|---|
| 2. Tính đóng gói | Không biết N sản phẩm xếp vào mấy thùng; dễ tính sai trọng lượng quy đổi (thể tích) | Sai lệch giữa giá báo và hoá đơn thật (%) |
| 3–4. Nhắn đi nhắn lại | Cùng một bộ thông tin phải gửi lại cho từng NCC, mỗi NCC hỏi thêm một kiểu | Số tin nhắn cho mỗi lần báo giá; số NCC phải liên hệ |
| 5. Chờ báo giá | Mỗi NCC trả lời sau vài giờ đến vài ngày **(giả định)** | Thời gian từ lúc khách hỏi đến lúc báo giá |
| 5–6. So sánh | Đơn vị và điều kiện khác nhau (kg / CBM, đã gồm thuế hay chưa, DDP hay DAP) nên khó so | Số lần báo lại giá cho khách vì tính thiếu |
| Giấy tờ | Không rõ NCC có lo được invoice, packing list, C/O, hun trùng, khai báo cho hàng gỗ / mây tre hay không | Số lô bị giữ ở hải quan hoặc phát sinh phí |

### Job Story

- **Hộ kinh doanh:** Khi khách nước ngoài hỏi giá một đơn gồm nhiều mẫu với kích thước khác nhau, tôi muốn có ngay chi phí vận chuyển ước tính kèm vài lựa chọn NCC có giấy tờ đầy đủ, để báo giá cho khách trong ngày mà không phải nhắn đi nhắn lại với từng nơi.
- **NCC vận chuyển:** Khi có khách hỏi gửi hàng, tôi muốn nhận một yêu cầu đã đủ thông tin (kích thước thùng, cân nặng, loại hàng, điểm đến), để báo giá nhanh mà không mất công hỏi lại, và không bị đem giá ra so công khai.

---

## 1. Giá trị và tính năng của sản phẩm

### Giá trị cốt lõi

| Đối tượng | Giá trị nhận được |
|---|---|
| Hộ kinh doanh | Có giá ship ước tính **trong vài phút** thay vì vài ngày; báo giá cho khách nhanh hơn nên ít mất đơn |
| Hộ kinh doanh | Nhập thông tin sản phẩm **một lần**, dùng lại cho mọi đơn sau |
| Hộ kinh doanh | So sánh được nhiều NCC theo cùng một chuẩn: tổng chi phí, thời gian, giấy tờ, độ tin cậy |
| Hộ kinh doanh | Biết trước cần giấy tờ gì để không bị giữ hàng ở hải quan |
| NCC vận chuyển | Nhận **yêu cầu báo giá đã chuẩn hoá, đủ thông tin**, bớt thời gian hỏi qua lại |
| NCC vận chuyển | Có thêm khách mới mà **không phải công khai bảng giá** cho đối thủ thấy |
| Cả hai bên | Giảm chi phí đi tìm nhau: không cần chạy quảng cáo hay lục từng group Facebook |

### Tính năng chính (theo thứ tự ưu tiên)

| # | Tính năng | Mô tả | Có cần AI? |
|---:|---|---|---|
| F1 | **Kho sản phẩm + thư viện dùng chung** | Mỗi mẫu lưu kích thước, cân nặng, chất liệu, độ dễ vỡ, ảnh, cách đóng gói. Sản phẩm mới được so khớp với mẫu tương đồng do doanh nghiệp khác đã kiểm chứng | **Có**. Lúc đầu AI ước tính từ ảnh; về sau AI so khớp với thư viện |
| F2 | **Tính đóng gói** | Nhập "50 cái mẫu A + 20 cái mẫu B", hệ thống ra số thùng, kích thước, cân nặng thật và cân nặng quy đổi (thể tích) | Phép tính dùng công thức; đầu vào (số cái mỗi thùng, kích thước thùng) lấy từ thư viện hoặc AI ước tính |
| F3 | **Gợi ý hình thức vận chuyển** | Chuyển phát nhanh, hàng không hay đường biển gom hàng (LCL), dựa trên khối lượng, giá trị và thời gian khách cần | Quy tắc là chính; AI giải thích lý do bằng lời |
| F4 | **Yêu cầu báo giá chuẩn (RFQ)** | Một form hoặc chatbot gom đủ thông tin rồi gửi cùng lúc tới 3–5 NCC phù hợp | Chatbot AI hỏi bù thông tin còn thiếu |
| F5 | **Đọc báo giá của NCC** | NCC trả lời bằng tin nhắn, ảnh hoặc PDF, hệ thống chuyển về một bảng so sánh chung | **Có**. AI trích xuất từ văn bản và ảnh |
| F6 | **Bảng so sánh riêng tư** | Chỉ hộ kinh doanh đã gửi yêu cầu mới thấy các báo giá; xếp theo tổng chi phí, thời gian, giấy tờ, đánh giá | Không |
| F7 | **Danh sách giấy tờ hải quan** | Theo loại hàng: invoice, packing list, C/O, hun trùng, khai báo hàng gỗ / thực vật khi vào Mỹ… và NCC nào hỗ trợ việc gì | AI gợi ý, **người kiểm duyệt** |
| F8 | **Soạn báo giá cho khách Mỹ** | Ghép giá hàng + giá ship + điều kiện giao hàng thành báo giá tiếng Anh | Có. AI soạn, người bán sửa |
| F9 | **Bảng giá riêng của NCC (giai đoạn sau)** | NCC tự nhập công thức giá riêng; hệ thống tự báo giá thay họ, đối thủ không xem được | Không |

### Giải quyết mâu thuẫn "NCC không muốn bị so giá"

Đây là rủi ro lớn nhất về phía cung, nên thiết kế cần tránh kiểu "chợ so giá công khai":

1. **Không có bảng giá công khai.** Báo giá chỉ hiện cho đúng hộ kinh doanh đã hỏi. NCC khác không thấy.
2. **Không xếp hạng chỉ theo giá.** Điểm xếp hạng gồm: tổng chi phí, thời gian giao, hỗ trợ giấy tờ, tỷ lệ báo giá đúng với hoá đơn, tốc độ phản hồi. NCC làm tốt có thể thắng mà không cần rẻ nhất.
3. **Giới hạn số NCC mỗi yêu cầu** (ví dụ 3–5 nơi), không thả ra cho mọi NCC cùng tranh.
4. **Bán giá trị "khách sạch":** NCC nhận yêu cầu đã đủ thông tin và đúng tuyến họ chạy, nên bớt công tư vấn những khách không chốt.
5. **Giá ước tính của hệ thống chỉ là khoảng giá**, tính từ công thức chung (ví dụ "khoảng 180–240 USD"), không lấy bảng giá riêng của NCC nào ra để so.

---

## 2. Có nên dùng AI không? Dùng ở đâu?

### Kết luận ngắn

**Có, và AI giữ vai trò lớn nhất ở giai đoạn đầu, khi chưa có dữ liệu.** Lõi lâu dài của sản phẩm là **thư viện kích thước và đóng gói dùng chung**, hình thành dần từ nhiều doanh nghiệp làm cùng loại sản phẩm (xem mục 2b).

- **Lúc đầu:** AI phân tích ảnh, mô tả và kích thước để ước tính cách đóng gói. Người bán và NCC xác nhận.
- **Về sau:** hệ thống tái sử dụng dữ liệu đã kiểm chứng từ các lô thật. AI chuyển sang so khớp sản phẩm tương đồng, gộp nhiều trường hợp và phát hiện số liệu bất thường.
- **Phép tính tiền vẫn dùng công thức.** AI và thư viện chỉ cung cấp đầu vào: kích thước thùng, số cái mỗi thùng, cân nặng.

Mức can thiệp phù hợp: **Workflow có các bước AI + vòng lặp dữ liệu** (không phải Agent tự quyết).

| Việc | Mức phù hợp | Lý do |
|---|---|---|
| Tính thể tích, cân nặng quy đổi, số thùng | **Rule / thuật toán** | Cần đúng 100%, có công thức rõ. AI dễ tính sai số |
| Chọn hình thức vận chuyển | **Rule** + AI giải thích | Ngưỡng rõ ràng (cân nặng, CBM, thời gian); AI chỉ diễn giải cho người bán dễ hiểu |
| Điền thông tin sản phẩm từ ảnh hoặc mô tả | **AI** (người xác nhận) | Hộ kinh doanh ngại nhập form; AI đoán chất liệu, dễ vỡ, gợi ý cách đóng gói |
| Chatbot hỏi bù thông tin thiếu | **AI** | Hội thoại tự nhiên thay cho form dài |
| Đọc báo giá NCC (tin nhắn, ảnh, PDF) thành bảng | **AI** | Đây là chỗ AI tạo giá trị lớn nhất: mỗi NCC báo một kiểu |
| Gợi ý mã HS, giấy tờ hải quan | **AI gợi ý + người duyệt** | Sai thì bị phạt hoặc bị giữ hàng, nên không để AI tự quyết |
| Soạn báo giá tiếng Anh cho khách | **AI** | Tiết kiệm thời gian; người bán sửa trước khi gửi |
| Chốt giá, chọn NCC, đặt lịch | **Con người** | Trách nhiệm tiền bạc thuộc về người bán |

### Ví dụ phần không cần AI: tính cân nặng quy đổi

```text
Thùng 50 × 40 × 40 cm, nặng thật 8 kg
- Chuyển phát nhanh (hệ số 5000): 50×40×40 / 5000 = 16 kg  → tính tiền theo 16 kg
- Đường biển LCL: 0,08 CBM                                    → tính theo CBM (có mức tối thiểu)
Lấy giá trị lớn hơn giữa cân nặng thật và cân nặng quy đổi.
```

Hàng thủ công thường **nhẹ nhưng cồng kềnh** (giỏ mây, đèn tre), nên cân nặng quy đổi gần như luôn lớn hơn cân nặng thật. Đây là lý do người bán hay báo giá thiếu.

### Rủi ro khi dùng AI và cách chặn

- **AI tính số sai** → không cho AI tính tiền; mọi con số lấy từ công thức.
- **AI đọc sai báo giá** (nhầm USD/VND, nhầm kg/CBM) → hiện bản gốc bên cạnh, NCC hoặc người bán bấm xác nhận.
- **AI bịa mã HS hoặc quy định** → ghi rõ "gợi ý, cần NCC hoặc đại lý hải quan xác nhận"; quy định lấy từ danh sách có nguồn, cập nhật tay.

---

## 2b. Chiến lược dữ liệu: từ AI ước tính đến thư viện dùng chung

### Ý tưởng

- Một mẫu sản phẩm thủ công **không chỉ một hộ làm**. Ví dụ: bình gốm cao 30 cm, giỏ mây tròn 40 cm, đèn lồng tre có cả chục hộ và doanh nghiệp cùng làm.
- Vì vậy, kích thước và cách đóng gói đo được ở một hộ **dùng lại được cho hộ khác**.
- Thay vì mỗi hộ tự tính từ đầu trên một bảng tính riêng, mọi lô hàng thật đều góp vào **một thư viện chung**. Thư viện càng nhiều dữ liệu thì ước tính càng chính xác cho tất cả.

### Ba giai đoạn của dữ liệu

| Giai đoạn | Tình trạng dữ liệu | Hệ thống làm gì | Độ tin cậy hiển thị |
|---|---|---|---|
| **A. Khởi đầu** | Chưa có dữ liệu | AI phân tích ảnh, mô tả, kích thước sản phẩm, rồi ước tính số cái mỗi thùng, kích thước thùng, vật liệu chèn, cân nặng | "AI ước tính" (thấp), hiện khoảng giá rộng |
| **B. Tích luỹ** | Có vài lô thật | So ước tính với số NCC cân đo thật khi nhận hàng; AI học sai lệch và chỉnh lại | "Dựa trên 3 lô thật" (trung bình) |
| **C. Tái sử dụng** | Nhiều lô, nhiều doanh nghiệp | Sản phẩm mới được so khớp với mẫu tương đồng trong thư viện; dùng thẳng số đã kiểm chứng | "Đã kiểm chứng qua 12 lô" (cao), khoảng giá hẹp |

### Dữ liệu lấy từ đâu (theo độ tin cậy)

1. **NCC cân đo thật khi nhận hàng** (tin cậy cao nhất). NCC vốn phải cân đo mỗi lô để tính cước, nên chỉ cần ghi lại vào hệ thống, gần như không tốn thêm công.
2. **Hoá đơn cước thật** sau khi giao: phụ phí phát sinh, cân nặng tính tiền cuối cùng.
3. **Người bán tự đo** khi nhập sản phẩm.
4. **AI ước tính** từ ảnh và mô tả (thấp nhất, chỉ dùng khi chưa có nguồn khác).

Mỗi con số trong thư viện đều kèm **nguồn và số lô đã kiểm chứng**.

### AI phân tích nhiều trường hợp để ra số chính xác

- **So khớp sản phẩm tương đồng:** theo ảnh, chất liệu, kích thước, dáng (tròn, vuông, cao, dẹt), kể cả khi mỗi hộ đặt tên khác nhau.
- **Đóng gói hỗn hợp:** nhiều mẫu khác nhau trong cùng một đơn thì xếp thế nào cho ít thùng nhất, dựa trên các đơn tương tự trước đó.
- **Học hệ số thực tế:** hàng cồng kềnh bị tính theo thể tích cao hơn bao nhiêu; cách chèn nào ít vỡ; tuyến nào hay phát sinh phụ phí.
- **Phát hiện số bất thường:** nhập nhầm cm thành mm, cân nặng vô lý so với mẫu cùng loại.
- **Dùng khoảng thay vì một số:** hàng thủ công mỗi cái hơi khác nhau, nên thư viện lưu min–max và giá trị thường gặp.

### Quy tắc để dữ liệu dùng chung không gây hại

- **Chỉ chia sẻ thông số vật lý đã ẩn danh:** kích thước, cân nặng, cách đóng gói, kết quả lô (vỡ hay không, phụ phí).
- **Không chia sẻ:** tên hộ, giá bán, khách hàng, ảnh mẫu độc quyền.
- **Ngưỡng kiểm chứng:** cần ít nhất 3 lô thật từ ít nhất 2 doanh nghiệp thì một mẫu mới được gắn "đã kiểm chứng".
- **Số mới lệch nhiều so với thư viện** thì không tự gộp, chờ xác nhận.
- **Hộ đồng ý chia sẻ ẩn danh** để đổi lấy quyền dùng thư viện. Hộ không đồng ý vẫn dùng được nhưng chỉ có AI ước tính.

### Vì sao không chọn bảng tính thủ công

- Mỗi hộ phải tự đo, tự tính từ đầu. Kiến thức nằm trong file riêng của từng người, không ai dùng lại được.
- Không có số đối chiếu với lô thật, nên sai một lần là sai mãi.
- Thư viện dùng chung tạo **lợi thế càng dùng càng tốt**: đối thủ đến sau không có sẵn dữ liệu kích thước và đóng gói hàng thủ công thật.

---

## 3. Kế hoạch phát triển

| Giai đoạn | Thời gian (giả định) | Mục tiêu | Làm gì | Tiêu chí qua giai đoạn |
|---|---|---|---|---|
| **0. Khám phá** | 2 tuần | Xác nhận vấn đề có thật | Phỏng vấn 8–10 hộ kinh doanh và 4–5 NCC; thu 20 báo giá thật; đo thời gian báo giá hiện tại | ≥ 60% hộ nói báo giá ship là nút thắt; có ≥ 3 NCC chịu thử |
| **1. MVP dữ liệu + AI** | 4–6 tuần | Kiểm chứng AI ước tính đóng gói và bắt đầu tích luỹ dữ liệu | Web đơn giản: nhập ảnh, kích thước, số lượng; AI ước tính đóng gói (giai đoạn A); NCC đối tác ghi số cân đo thật mỗi lô; người vận hành vẫn gửi yêu cầu tới NCC thay hộ | Sai số ước tính cân nặng tính cước được đo; thời gian báo giá giảm ≥ 50%; mỗi nhóm hàng chính có ≥ 3 lô thật |
| **2. Web + chatbot** | 6–8 tuần | Tự động phần lặp lại | Kho sản phẩm, tính đóng gói, chatbot gom thông tin, cổng NCC trả lời, AI đọc báo giá, bảng so sánh riêng | 20 hộ dùng thường xuyên; NCC trả lời trung bình dưới 4 giờ |
| **3. Mở rộng** | Sau 3 tháng | Tạo doanh thu, giữ chân hai bên | Bảng giá riêng của NCC để tự báo giá, danh sách giấy tờ theo ngành hàng, đánh giá sau giao hàng, thu phí | Có doanh thu; tỷ lệ báo giá lệch hoá đơn dưới 10% |

### Công nghệ chi phí thấp (gợi ý)

- Giao diện web và API: Cloudflare Pages / Workers (miễn phí ở quy mô nhỏ).
- Dữ liệu: cơ sở dữ liệu ngay từ đầu (D1 / Postgres) để lưu thư viện dùng chung, kèm lưu ảnh và chỉ mục tìm sản phẩm tương đồng.
- AI: một mô hình đa phương thức qua API, chỉ gọi ở các bước đọc báo giá, điền từ ảnh và soạn văn bản. Chi phí theo lượt, rất thấp ở quy mô vài trăm yêu cầu mỗi tháng.
- Kênh liên lạc: tích hợp Zalo / Telegram cho NCC, vì họ đã quen nhắn tin.

### Thu thập dữ liệu từ hộ kinh doanh

Nguyên tắc: **hộ kinh doanh nhập dữ liệu vì được lợi ngay**, không phải vì nền tảng cần dữ liệu.

- **Công cụ miễn phí là "mồi":** kho sản phẩm, tính đóng gói, mẫu báo giá tiếng Anh. Hộ nhập kích thước sản phẩm để tự dùng, hệ thống có dữ liệu.
- **Nhập dễ:** chụp ảnh + gửi kích thước qua chatbot hoặc Zalo, AI điền sẵn, người bán chỉ xác nhận.
- **Ưu đãi lô đầu:** NCC đối tác giảm phí lô đầu cho hộ nhập đủ thông tin sản phẩm. NCC chi khoản này như chi phí tìm khách.
- **Đi qua kênh có sẵn:** hiệp hội làng nghề, chương trình xúc tiến xuất khẩu, nhóm và khoá học bán hàng Etsy hoặc Amazon.
- **Dữ liệu từ lô thật:** sau mỗi lô, lưu kích thước thùng thật và hoá đơn thật, dùng để ước tính lần sau chính xác hơn.
- **Cam kết quyền riêng tư:** dữ liệu sản phẩm và giá thuộc về hộ; không bán dữ liệu; NCC chỉ thấy yêu cầu được gửi cho mình.

### Chi phí vận hành (giả định, giai đoạn MVP)

- Hosting và cơ sở dữ liệu: gần như 0 đồng nếu dùng gói miễn phí.
- AI: trả theo lượt gọi, chỉ dùng ở bước đọc báo giá, điền từ ảnh và soạn văn bản. Ở vài trăm yêu cầu mỗi tháng thì chi phí nhỏ.
- **Người vận hành là chi phí lớn nhất** ở giai đoạn làm tay: gọi NCC, kiểm tra báo giá, hỗ trợ hộ kinh doanh.
- Tên miền, Zalo OA / Telegram bot: chi phí thấp.

### Thu tiền từ đâu (thứ tự ưu tiên, giả thuyết cần kiểm chứng)

1. **NCC trả phí theo lô chốt thành công** (nguồn thu chính). Ví dụ một phần trăm nhỏ trên cước hoặc phí cố định mỗi lô. NCC chỉ trả khi có khách thật, nên dễ chấp nhận nhất.
2. **Gói thuê bao cho NCC** (giai đoạn sau): cổng nhận yêu cầu, bảng giá riêng để hệ thống tự báo giá thay họ, thống kê khách hàng.
3. **Gói Pro cho hộ kinh doanh:** báo giá tiếng Anh không giới hạn, xuất invoice và packing list, nhiều người dùng chung, lưu lịch sử báo giá.
4. **Hoa hồng dịch vụ cộng thêm:** làm C/O, hun trùng, bảo hiểm hàng hoá, đóng gói chuyên nghiệp qua đối tác.
5. **Tài trợ hoặc hợp tác:** chương trình hỗ trợ doanh nghiệp nhỏ xuất khẩu, hiệp hội ngành hàng.

**Không thu:**
- phí xem báo giá;
- phí đăng ký ban đầu với hộ kinh doanh;
- tiền bán dữ liệu.

Mỗi khoản trên đều làm giảm số người tham gia ở giai đoạn đầu.

---

## 4. Rủi ro của dự án

| # | Rủi ro | Mức | Cách giảm |
|---:|---|---|---|
| R1 | **NCC không tham gia** vì sợ bị so giá, sợ mất khách quen | Cao | Báo giá riêng tư, không xếp hạng chỉ theo giá, phí theo lô chốt; bắt đầu với 3–5 NCC quen, làm tay trước |
| R2 | **Bài toán con gà – quả trứng:** ít NCC thì hộ không dùng, ít hộ thì NCC không vào | Cao | Chỉ làm một tuyến hẹp (Việt Nam → Mỹ, hàng thủ công nhỏ); người vận hành làm tay ở giai đoạn đầu |
| R3 | **Báo giá ước tính sai** do kích thước nhập sai hoặc phụ phí phát sinh, khiến khách mất lòng tin | Cao | Luôn ghi "ước tính", hiện khoảng giá; giá chốt là của NCC; theo dõi độ lệch so với hoá đơn |
| R4 | **Chính sách thuế và hải quan Mỹ thay đổi nhanh** (thuế nhập khẩu, quy định miễn thuế hàng giá trị nhỏ, khai báo hàng gỗ / thực vật) | Cao | Không tự tính thuế ở MVP; dẫn nguồn chính thức, ghi ngày cập nhật; để NCC xác nhận |
| R5 | **Hai bên gặp nhau rồi giao dịch ngoài nền tảng** | Trung bình | Giá trị nằm ở công cụ (kho sản phẩm, đóng gói, giấy tờ, soạn báo giá) chứ không chỉ ở việc kết nối |
| R6 | **AI đọc sai hoặc bịa thông tin** | Trung bình | AI không tính tiền; luôn có bước xác nhận; hiện bản gốc |
| R7 | **Hộ kinh doanh ngại nhập dữ liệu** | Trung bình | Nhập bằng ảnh + chatbot; chỉ bắt buộc vài trường cốt lõi |
| R8 | **Đã có đối thủ** (nền tảng so giá chuyển phát quốc tế, công ty logistics lớn) | Trung bình | Tập trung chỗ họ bỏ trống: NCC nhỏ báo giá thủ công, hàng cồng kềnh, giấy tờ hàng thủ công |
| R9 | **Trách nhiệm pháp lý** khi hàng bị giữ hoặc hỏng | Trung bình | Nền tảng là bên kết nối; điều khoản rõ; trách nhiệm vận chuyển thuộc NCC |
| R10 | **Dữ liệu sai lan sang nhiều doanh nghiệp** khi dùng chung | Cao | Ngưỡng ≥ 3 lô từ ≥ 2 doanh nghiệp; ưu tiên số NCC cân thật; số lệch nhiều phải chờ duyệt |
| R11 | **Hộ ngại chia sẻ** vì sợ lộ mẫu mã hoặc giá | Trung bình | Chỉ chia sẻ thông số vật lý ẩn danh; không chia sẻ ảnh, giá, khách; hộ tự chọn đồng ý |
| R12 | **NCC không ghi số cân đo thật** | Trung bình | Nhập nhanh qua Zalo / ảnh phiếu cân; gắn với phí theo lô (ghi số mới tính là lô hợp lệ) |

---

## 5. Đánh giá bài toán

### So sánh với sản phẩm trên thị trường

Các sản phẩm hiện có (tra cứu 11/2026, chủ yếu từ trang giới thiệu của chính công ty, cần kiểm tra lại):

- **Easyship**: so sánh giá chuyển phát nhanh của nhiều hãng cho từng kiện.
  - Thiếu: tự tính đóng gói nhiều mẫu, forwarder nhỏ Việt Nam, giấy tờ hàng thủ công.
- **Flexport, Shipa Freight, FreightAmigo**: báo giá online đường biển ghép hàng (LCL) và hàng không, từ cảng Việt Nam đi Mỹ.
  - Thiếu: phù hợp lô lớn (Flexport lấy mốc 5 CBM / 750 kg), người dùng phải tự biết CBM, giao diện tiếng Anh.
- **Ship4wd**: nhắm vào doanh nghiệp nhỏ, khoá giá và trả trước phí thông quan trên một nền tảng.
  - Thiếu: vẫn là hàng đường biển, không hỗ trợ tính đóng gói hàng thủ công.
- **Boxme Global**: fulfillment xuyên biên giới cho người bán online, tích hợp nhiều hãng vận chuyển.
  - Thiếu: hướng tới hàng thương mại điện tử chuẩn; tuyến Mỹ từng đi qua kho ở Trung Quốc (tài liệu cũ).
- **Etsy + Asendia**: kênh gửi hàng từ Việt Nam cho người bán Etsy.
  - Thiếu: chỉ cho đơn trên sàn; nhãn gửi hàng của chính Etsy không mở cho người bán Việt Nam.
- **Forwarder Việt Nam tự báo giá**: lo trọn gói, kể cả giấy tờ.
  - Thiếu: báo giá qua Zalo hoặc điện thoại, chậm, mỗi nơi một kiểu. Đây là chỗ đề tài muốn giải.

Điểm khác của **ShipQuote Craft**:

- Tính đóng gói nhiều mẫu, nhiều kích thước từ kho sản phẩm. Các sản phẩm trên chưa làm việc này.
- Kết nối forwarder **nhỏ trong nước** đang báo giá tay, thay vì chỉ hãng lớn.
- Báo giá **riêng tư**, không phải chợ so giá công khai, nên NCC chịu tham gia.
- AI đọc báo giá lộn xộn (tin nhắn, ảnh, PDF) về một bảng chung.
- Danh sách giấy tờ riêng cho hàng thủ công: hun trùng, C/O, khai báo hàng gỗ và thực vật.
- Giao diện tiếng Việt, nhập bằng ảnh hoặc Zalo, miễn phí cho hộ kinh doanh.

Nơi ShipQuote Craft **không nên cạnh tranh**:

- Không cạnh tranh giá chuyển phát nhanh kiện nhỏ với Easyship. Có thể hiện giá Easyship làm giá tham chiếu.
- Không cạnh tranh lô lớn nguyên container với Flexport và các nền tảng tương tự.

### Chấm nhanh (thang 1–5, chấm theo hiểu biết hiện tại, cần kiểm chứng)

| Tiêu chí | Điểm | Nhận xét |
|---|---:|---|
| Pain có thật và lặp lại | 4 | Mỗi đơn mới là một lần hỏi giá; hàng nhiều mẫu thì càng khó |
| Tần suất | 3 | Tuỳ hộ: vài lần mỗi tuần đến vài lần mỗi tháng **(giả định)** |
| Sẵn sàng trả tiền (hộ kinh doanh) | 2 | Hộ nhỏ nhạy cảm chi phí; nên thu phí từ phía NCC |
| Sẵn sàng tham gia (NCC) | 2–3 | Rủi ro lớn nhất; phụ thuộc thiết kế riêng tư |
| Khả thi kỹ thuật | 4 | Lõi là công thức và quy trình; AI chỉ ở vài bước |
| Mức phù hợp với AI | 3 | AI giúp nhiều ở đọc báo giá và nhập liệu, không phải lõi |
| Khác biệt so với giải pháp có sẵn | 3 | Khác biệt nằm ở NCC nhỏ + hàng thủ công + giấy tờ, không ở việc so giá |

### Điểm mạnh

- Vấn đề cụ thể, người thật đang làm tay mỗi ngày qua Zalo / Facebook.
- Đo được: thời gian báo giá, số tin nhắn, độ lệch giá.
- Dữ liệu dùng chung càng dùng càng chính xác. Đây là lợi thế đối thủ đến sau khó có.
- MVP rẻ: AI theo lượt + NCC ghi số cân đo vốn đã phải làm.

### Điểm yếu, điều còn chưa chắc

- Chưa có số liệu thật: hộ mất bao lâu cho một lần báo giá? Mất bao nhiêu đơn vì báo chậm?
- Chưa biết NCC nhỏ có chịu trả lời qua một cổng mới không, hay chỉ muốn Zalo.
- Hộ kinh doanh có thực sự có đơn từ Mỹ đều đặn không, hay phần lớn bán qua sàn (Etsy, Amazon) đã có sẵn dịch vụ ship?
- "Cần đủ số lượng mới tính được đóng gói": cần làm rõ hộ có biết kích thước đóng gói chuẩn từng mẫu chưa, hay phải đo lại từ đầu.

### Success metric (baseline → target, cần đo baseline ở Giai đoạn 0)

| Chỉ số | Baseline | Target sau MVP |
|---|---|---|
| Thời gian từ lúc khách hỏi đến lúc báo được giá ship | đo thật (giả định 1–3 ngày) | dưới 4 giờ |
| Số tin nhắn qua lại với NCC cho mỗi lần báo giá | đo thật | giảm ≥ 50% |
| Độ lệch giữa giá ship đã báo và hoá đơn thật | đo thật | dưới 10% |
| Tỷ lệ yêu cầu báo giá chốt thành lô hàng | đo thật | ≥ 30% |

### Phương án không dùng AI (để so sánh)

Một **bảng tính mẫu** cho mỗi hộ: tab sản phẩm, tab tính thùng và cân nặng quy đổi, tab mẫu tin nhắn yêu cầu báo giá.

- Ưu điểm: rẻ, làm được ngay.
- **Không chọn**, vì mỗi hộ phải tự đo và tính từ đầu, dữ liệu nằm rời trong file riêng, không đối chiếu được với lô thật và không dùng lại được cho doanh nghiệp khác.
- Phương án này chỉ dùng làm **mốc so sánh**: đo xem AI ước tính + thư viện dùng chung có nhanh hơn và chính xác hơn bảng tính tự làm không.

### Chỉ số riêng cho chiến lược dữ liệu

| Chỉ số | Ý nghĩa |
|---|---|
| Sai số cân nặng tính cước (ước tính so với NCC cân thật) | Giai đoạn A đo baseline; mục tiêu giảm dần khi thư viện lớn lên |
| Tỷ lệ sản phẩm mới tìm được mẫu tương đồng trong thư viện | Cho biết dữ liệu đã đủ để tái sử dụng chưa |
| Số mẫu "đã kiểm chứng" theo nhóm hàng | Độ phủ của thư viện |
| Tỷ lệ lô có NCC ghi số cân đo thật | Cho biết vòng lặp dữ liệu có chạy không |

### Kết luận

Bài toán **đáng làm nếu thu hẹp phạm vi**: một tuyến (Việt Nam → Mỹ), một nhóm hàng (thủ công nhỏ, cồng kềnh), vài NCC đầu tiên. Rủi ro lớn nhất không phải kỹ thuật hay AI, mà là **phía NCC có tham gia hay không**. Vì vậy câu hỏi cần trả lời đầu tiên trong phỏng vấn là: *"Nếu nhận được yêu cầu đã đủ thông tin, có giới hạn số người cùng báo giá và đối thủ không thấy giá của anh/chị, anh/chị có trả lời qua kênh này không?"*

### Câu hỏi phỏng vấn gợi ý

**Hộ kinh doanh**
1. Lần gần nhất khách nước ngoài hỏi giá, từ lúc hỏi đến lúc anh/chị báo được giá mất bao lâu?
2. Anh/chị đã hỏi mấy NCC vận chuyển? Nhắn qua lại khoảng bao nhiêu tin?
3. Đã bao giờ báo giá ship thiếu, phải bù tiền hoặc báo lại cho khách chưa?
4. Đã từng mất đơn vì báo giá chậm chưa? Bao nhiêu lần trong 3 tháng gần đây?
5. Anh/chị có sẵn kích thước đóng gói của từng mẫu không?

**NCC vận chuyển**
1. Một ngày anh/chị nhận bao nhiêu yêu cầu báo giá? Bao nhiêu phần trăm chốt được?
2. Mất bao lâu để hỏi đủ thông tin trước khi báo được giá?
3. Anh/chị lo điều gì nếu báo giá qua một nền tảng chung?
4. Anh/chị chấp nhận trả phí theo hình thức nào: theo lô chốt, theo tháng, hay không trả?
