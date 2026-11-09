# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: 3TDL
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi khách Mỹ hỏi mua đơn hàng gồm nhiều mẫu thủ công mỹ nghệ, hộ kinh doanh mất 1–3 ngày tự ước tính đóng gói (số thùng, cân nặng quy đổi/CBM), nhắn Zalo hỏi từng nhà cung cấp vận chuyển (NCC) và tự đối chiếu các báo giá/giấy tờ hải quan không đồng nhất trước khi báo lại cho khách.
- Quyết định cuối: **Not Yet** (Thực hiện GĐ 0 trong 2 tuần để kiểm chứng 8–10 hộ kinh doanh & 3–5 NCC trước khi triển khai MVP GĐ 1 trong phạm vi hẹp: 1 tuyến Việt Nam → Mỹ, 1–2 nhóm hàng thủ công).

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Nguyễn Mạnh Tường | Khi khách Mỹ hỏi mua sỉ/lẻ nhiều mẫu hàng thủ công (gốm, mây tre), tôi muốn biết nhanh cách đóng thùng, cước ship và giấy tờ cần thiết, để báo giá trong vài giờ thay vì chờ 1–3 ngày | Hộ kinh doanh hàng thủ công bán sang Mỹ | Tự ước tính số thùng/CBM dễ sai + nhắn Zalo hỏi 3–5 NCC rồi tự quy đổi bảng giá lộn xộn | "NCC nhỏ có chịu đưa bảng giá lên hệ thống không hay sợ bị lộ giá và so giá?" (Mai Lâm Tấn Đạt) |
| 2 | Phạm Duy Đức | Khi xuất hàng thủ công (gỗ, mây tre, gốm) đi quốc tế, tôi muốn biết chính xác lô hàng cần giấy tờ gì (C/O, hun trùng, khai báo gỗ/mây tre), để không bị hải quan giữ hàng | Hộ kinh doanh xuất khẩu nhỏ | Thông tin quy định rải rác, hỏi mỗi forwarder nói một kiểu, không rõ bên nào lo trọn gói | "Quy định hải quan Mỹ thay đổi liên tục, nếu AI tư vấn sai thì ai chịu trách nhiệm?" (Nguyễn Mạnh Tường) |
| 3 | Nguyễn Trần Tú Trân | Khi khách nước ngoài nhắn hỏi giá sản phẩm kèm phí ship sang Mỹ, tôi muốn gom báo giá từ các bên ship và soạn nhanh báo giá tiếng Anh chuẩn, để tăng tỷ lệ chốt đơn | Chủ xưởng / hộ làm hàng thủ công | Mỗi NCC báo một kiểu (kg, CBM, có/chưa có phụ phí) và hộ không rành thuật ngữ tiếng Anh | "Đây là bước nối tiếp của bài toán đóng gói và hỏi giá NCC, có nên gộp chung với #1 và #2 không?" (Mai Lâm Tấn Đạt) |
| 4 | Mai Lâm Tấn Đạt | Khi đến kỳ báo cáo trạng thái dự án ngày/tuần, tôi muốn tổng hợp dữ liệu từ task board, ghi chú, tin nhắn nhóm và số liệu tiến độ thành status report chuẩn, để cập nhật nhanh cho stakeholder mà không sót blocker | PM, Team Lead, thành viên dự án | Đọc lại nhiều nguồn rời rạc và viết phần tóm tắt/blocker (mất 30–60 phút/lần) | "Dùng template cố định hoặc công cụ có sẵn trong Jira/Notion đã đủ giải quyết 80% chưa?" (Lục Anh Tuấn) |
| 5 | Mai Lâm Tấn Đạt | Khi nhận đề tài thuyết trình nhóm có deadline và giới hạn số slide, tôi muốn chuyển đề bài và tài liệu thành dàn ý, nội dung slide theo vai trò, kịch bản nói và checklist, để nhóm làm đồng bộ | Sinh viên / thành viên nhóm dự án | Đọc tài liệu tham khảo, chia việc và ghép nội dung các thành viên (2–4 giờ/đợt) | "Làm sao đo lường định lượng được chất lượng một bài slide 'đồng bộ' trong phạm vi buổi lab?" (Nguyễn Trần Tú Trân) |
| 6 | Mai Lâm Tấn Đạt | Khi cuối tuần cần chuẩn bị bữa ăn cho các ngày bận (Meal Prep), tôi muốn có kế hoạch batch cooking, định lượng nguyên liệu, lịch nấu và cách chia hộp/nhãn ngày ăn, để tránh ăn nhanh không healthy | Người đi làm / sinh viên bận rộn | Tính khẩu phần, chọn anchor meals và xếp lịch nấu mất 1–2 giờ mỗi cuối tuần | "Nếu chỉ xoay quanh vài món quen thuộc thì dùng ghi chú cố định có nhanh hơn nhập vào AI không?" (Nguyễn Thuỳ Lam) |
| 7 | Nguyễn Thuỳ Lam | Khi mỗi tối cần quyết định ngày mai ăn gì (Daily Meal Planner) theo mục tiêu dinh dưỡng, ngân sách, thời gian nấu và nguyên liệu sẵn có, tôi muốn có sẵn thực đơn sáng–trưa–tối kèm calo/macro, để không gọi đồ ngoài | Cá nhân kiểm soát cân nặng / sức khỏe | Lọc món theo nhiều ràng buộc (dị ứng, tồn kho tủ lạnh, thời gian) mất 15–30 phút mỗi tối | "Người dùng có kiên nhẫn nhập lại nguyên liệu tồn trong tủ lạnh mỗi tối không?" (Phạm Duy Đức) |
| 8 | Lục Anh Tuấn | Khi đã có thực đơn tuần (Smart Grocery List), tôi muốn gộp nguyên liệu trùng, trừ tồn kho và phân nhóm theo khu vực cửa hàng kèm ước lượng chi phí, để đi siêu thị nhanh và không vượt ngân sách | Người nội trợ / người tự nấu ăn theo tuần | Đối chiếu thực đơn với tủ lạnh mất 20–30 phút/lần, dễ mua thừa hoặc quên đồ | "Tần suất đi siêu thị chỉ 1–2 lần/tuần thì mức độ đau (pain) có đủ lớn để người dùng đổi công cụ không?" (Nguyễn Mạnh Tường) |
| 9 | Lục Anh Tuấn | Khi nhận nhiều phản hồi/tin nhắn hỏi hàng từ khách trên nhiều kênh, tôi muốn trích xuất nhanh yêu cầu chính (mẫu mã, số lượng, điểm giao), để không bỏ sót thông tin khi báo giá | Người bán hàng nhỏ / CSKH | Phải lội lại lịch sử chat dài để tìm kích thước và yêu cầu riêng của khách | "Có thể tích hợp bước hỏi bù thông tin thiếu này thành một bước trong luồng báo giá vận chuyển không?" (Nguyễn Thuỳ Lam) |
| 10 | Nguyễn Thuỳ Lam | Khi nhiều hộ cùng làm các dòng hàng thủ công tương tự (bình gốm 30cm, giỏ mây 40cm), tôi muốn tra cứu quy cách đóng thùng đã kiểm chứng, để không phải tự đo đạc và thử sai từ đầu | Hộ kinh doanh làng nghề / thủ công | Dữ liệu đóng gói nằm rời rạc ở từng hộ, mỗi lần có mẫu mới lại phải tự ước lượng | "Hộ kinh doanh có sợ lộ mẫu mã độc quyền hay giá bán khi chia sẻ dữ liệu đóng gói không?" (Phạm Duy Đức) |
| 11 | Phạm Duy Đức | Khi nhận yêu cầu hỏi giá vận chuyển từ hộ kinh doanh nhỏ, tôi muốn nhận đủ thông tin (số thùng, CBM, loại hàng, địa chỉ Mỹ) ngay từ đầu, để báo giá nhanh mà không tốn công hỏi đi hỏi lại | Nhà cung cấp vận chuyển (Forwarder nhỏ) | Tốn nhiều thời gian tư vấn qua Zalo cho những khách hỏi thiếu thông tin rồi không chốt | "NCC có chịu mở app/web mới để trả lời báo giá hay vẫn chỉ muốn dùng Zalo?" (Lục Anh Tuấn) |
| 12 | Nguyễn Trần Tú Trân | Khi sau mỗi lô hàng giao xong, hóa đơn cước thực tế bị lệch so với giá ước tính ban đầu, tôi muốn đối chiếu lại số cân đo thật của NCC, để các đơn sau báo giá chính xác hơn | Hộ kinh doanh & Người vận hành | Không lưu lại lịch sử kích thước thùng và hóa đơn thật của các lô trước để rút kinh nghiệm | "Làm sao khuyến khích NCC hoặc hộ kinh doanh ghi lại số cân đo thật sau khi giao?" (Mai Lâm Tấn Đạt) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| **A — Báo giá, đóng gói & vận chuyển hàng thủ công xuất đi Mỹ** | #1, #2, #3, #9, #10, #11, #12 | Hộ kinh doanh hàng thủ công và NCC vận chuyển nhỏ mất nhiều thời gian ước tính đóng gói (số thùng, CBM), nhắn hỏi qua lại trên Zalo, chuẩn hóa báo giá lộn xộn và kiểm tra giấy tờ hải quan cho từng đơn hàng đi Mỹ |
| **B — Tổng hợp tiến độ & phối hợp công việc nhóm** | #4, #5 | Đọc, phân loại và tổng hợp thông tin từ nhiều nguồn rời rạc (task board, chat, tài liệu tham khảo) thành báo cáo trạng thái hoặc nội dung thuyết trình theo template |
| **C — Lên kế hoạch bữa ăn & mua sắm thực phẩm cá nhân** | #6, #7, #8 | Lập thực đơn, tính dinh dưỡng (calo/macro), lên lịch sơ chế (meal prep) và gộp danh sách mua sắm dựa trên ngân sách và nguyên liệu tồn kho |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian từ lúc khách Mỹ hỏi mua đến lúc hộ kinh doanh báo được giá ship chính xác (từ 1–3 ngày xuống dưới 4 giờ, độ lệch giá so với hóa đơn thật dưới 10%)
├── Opportunity A (Đóng gói & CBM): Hàng thủ công nhẹ nhưng cồng kềnh, bị tính theo cân nặng quy đổi (thể tích/CBM); hộ kinh doanh phải tự đo, tự đoán xếp được mấy thùng khi khách mua gộp nhiều mẫu nên rất dễ báo giá thiếu.
├── Opportunity B (Thu thập & so sánh báo giá): Hộ kinh doanh phải nhắn Zalo/Facebook lặp lại cho 3–5 NCC vận chuyển, trả lời các câu hỏi bổ sung rời rạc, chờ lâu và tự quy đổi các báo giá khác chuẩn (kg, CBM, đã có hoặc chưa có phụ phí) để so sánh; trong khi phía NCC nhỏ lại tốn thời gian tư vấn các yêu cầu thiếu thông tin và ngại bị so giá công khai.
└── Opportunity C (Giấy tờ hải quan & báo giá tiếng Anh): Hộ kinh doanh không rõ lô hàng (gốm, gỗ, mây tre) cần giấy tờ gì khi vào Mỹ (invoice, packing list, C/O, hun trùng, khai báo hàng gỗ/mây tre) và NCC nào hỗ trợ, đồng thời mất thời gian ghép giá hàng và giá ship thành bản báo giá tiếng Anh cho khách.
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- *"Hộ kinh doanh thiếu công cụ AI để chọn phương án vận chuyển"* ← Solution đội lốt problem (nhảy thẳng vào "công cụ AI"), đã gạch bỏ và tách thành 3 opportunity cụ thể ở trên.
- *"Sàn/chợ so sánh bảng giá công khai giữa các forwarder"* ← Solution, đồng thời mâu thuẫn trực tiếp với pain của NCC nhỏ (sợ lộ bảng giá và bị ép giá công khai).
- *"Chatbot AI tự động tính thuế hải quan Mỹ và tự chốt đơn với khách"* ← Solution quá rủi ro (quy định thuế Mỹ thay đổi nhanh, tính sai gây thiệt hại tài chính trực tiếp).

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **Cluster A: Báo giá vận chuyển & đóng gói cho hộ làm hàng thủ công bán sang Mỹ (Báo Giá Liền Tay)** | 5 | 5 | 4 | 5 | 4 | 5 | 4 | **32** |
| **Cluster B: Soạn báo cáo trạng thái dự án hằng ngày/tuần** | 5 | 5 | 4 | 4 | 5 | 4 | 4 | **31** |
| **Cluster C: Trợ lý thực đơn & danh sách mua sắm tuần (Meal Prep / Grocery List)** | 4 | 4 | 3 | 3 | 5 | 3 | 5 | **27** |

**Candidate được chọn:** Báo giá vận chuyển, ước tính đóng gói và chuẩn hóa báo giá NCC cho hộ kinh doanh hàng thủ công bán sang Mỹ (**Báo Giá Liền Tay** — Cluster A).

**Vì sao chọn:**
- Bài toán có **Actor hai phía rất rõ** (Hộ kinh doanh hàng thủ công xuất đi Mỹ & Nhà cung cấp vận chuyển/forwarder nhỏ) cùng quy trình 6 bước thủ công đang diễn ra mỗi ngày qua Zalo.
- Cho phép **phân định cực kỳ rạch ròi giữa Rule, AI và Con người**: phép tính số thùng, CBM, cân nặng quy đổi và tiền cước dùng **Rule (công thức)**; việc ước tính đóng gói khi chưa có dữ liệu, hỏi bù thông tin, đọc báo giá lộn xộn (tin nhắn, ảnh, PDF) về một bảng chung và soạn nháp tiếng Anh dùng **AI (Workflow)**; việc xác nhận giá và chốt NCC do **Con người** quyết định.
- Có lợi thế **vòng lặp dữ liệu (Data Flywheel)**: thông số đóng gói và cân đo thật từ một hộ có thể ẩn danh để tái sử dụng cho các hộ khác làm cùng dòng sản phẩm (bình gốm 30cm, giỏ mây 40cm, đèn lồng tre...).

**Vì sao loại các candidate còn lại:**
- *Cluster B (Báo cáo trạng thái dự án):* Quy trình rõ nhưng thị trường đã bão hòa công cụ giải quyết trực tiếp trong hệ sinh thái làm việc (Atlassian Rovo, Slack AI, Notion AI, n8n), ít khoảng trống khác biệt.
- *Cluster C (Meal Prep / Smart Grocery List):* Phù hợp quy mô cá nhân nhưng impact kinh tế thấp, rào cản lớn ở thói quen người dùng (ngại cập nhật tồn kho tủ lạnh mỗi ngày) và phần lớn giải quyết được bằng công thức/rule lọc cơ bản.

**Xử lý bất đồng (nếu có):**
- Một số thành viên lo ngại bài toán logistics quốc tế quá rộng, vướng rào cản NCC không chịu công khai giá và rủi ro pháp lý/thuế hải quan Mỹ. Nhóm đã giải quyết bằng cách **thu hẹp phạm vi triệt để**: (1) Chỉ tập trung 1 tuyến **Việt Nam → Mỹ** cho ngành **hàng thủ công cồng kềnh**; (2) Thiết kế **báo giá riêng tư** (mỗi yêu cầu chỉ gửi 3–5 NCC, không có bảng giá công khai); (3) **Không tự tính thuế hải quan ở MVP** mà chỉ gợi ý danh mục giấy tờ kèm nguồn chính thức và yêu cầu NCC xác nhận.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Hộ kinh doanh hàng thủ công mất 1–3 ngày nhắn hỏi nhiều nơi mới báo được giá ship đi Mỹ, làm chậm phản hồi và mất đơn của khách | Value | 5 | 2 | Kiểm chứng ngay (GĐ 0) |
| 2 | NCC vận chuyển nhỏ đồng ý nhận yêu cầu chuẩn và gửi báo giá nếu báo giá được giữ riêng tư (không bị so giá công khai) và chỉ trả phí khi chốt được lô hàng | Viability | 5 | 2 | Kiểm chứng ngay (GĐ 0) |
| 3 | Hộ kinh doanh chưa có sẵn kích thước đóng gói chuẩn khi khách mua gộp nhiều mẫu, và sẵn sàng nhập qua ảnh/Zalo/chatbot để nhận ước tính ban đầu | Usability | 4 | 2 | Kiểm chứng ngay (GĐ 0) |
| 4 | Kích thước và cách đóng gói đo thật ở một hộ (do NCC cân đo khi nhận hàng) có thể ẩn danh và tái sử dụng chính xác cho hộ khác làm mẫu tương đồng | Feasibility | 4 | 3 | Kiểm chứng ở GĐ 1 |
| 5 | AI có thể trích xuất các báo giá dạng tin nhắn Zalo, ảnh chụp, file PDF của nhiều NCC về một bảng so sánh chuẩn (tổng chi phí, thời gian, giấy tờ) | Feasibility | 4 | 4 | — |
| 6 | Sự thay đổi nhanh của thuế và quy định hải quan Mỹ (C/O, hun trùng, khai báo gỗ/mây tre) không làm vỡ luồng báo giá nếu hệ thống chỉ gợi ý danh mục giấy tờ và để NCC xác nhận | Viability | 5 | 2 | Kiểm chứng ngay (GĐ 0) |

Giả định nhóm kiểm chứng trong buổi này và GĐ 0:
- **Ưu tiên số 1:** Giả định #1 (Nút thắt thời gian & độ lệch báo giá phía hộ kinh doanh), Giả định #2 (Sự tham gia của NCC vận chuyển nhỏ khi báo giá riêng tư) và Giả định #3 (Thực trạng tự đoán số thùng/CBM khi khách Mỹ hỏi đơn gộp nhiều mẫu).

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn tình huống thực tế (theo nguyên tắc *The Mom Test*) + Phân tích luồng chat báo giá qua Zalo của hộ làm hàng thủ công và forwarder nhỏ + Thiết kế cổng kiểm chứng định lượng GĐ 0.

Interview snapshot #1 (Phía hộ kinh doanh hàng thủ công):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Chủ hộ kinh doanh đồ gốm & mây tre đan bán cho khách lẻ/sỉ nhỏ tại Mỹ (qua kênh trực tiếp, Facebook, Etsy) |
| Câu nói đáng nhớ nhất (nguyên văn) | *"Khách Mỹ hỏi '50 bình gốm mẫu A và 20 giỏ mây mẫu B, giao tới Texas giá bao nhiêu?', mình phải tự nhẩm xem xếp được mấy thùng rồi nhắn Zalo cho 3–5 bên vận chuyển, mỗi nơi hỏi thêm một kiểu rồi báo một kiểu, chờ gom đủ để so cũng mất cả ngày đến vài ngày."* |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Khách hỏi mua đơn gộp nhiều mẫu gốm và giỏ mây; vì hàng thủ công nhẹ nhưng cồng kềnh nên khi gửi thật bị tính theo cân nặng quy đổi (thể tích/CBM) cao hơn hẳn cân nặng thật, cộng thêm phí hun trùng cho hàng mây tre khiến giá ship đội lên so với ước tính ban đầu. |
| Hiện đang xử lý bằng cách nào (workaround)? | Tự đo và đoán số thùng theo cảm tính; nhắn Zalo/Facebook riêng cho 3–5 NCC quen; gửi lại cùng một bộ ảnh, kích thước, số lượng cho từng nơi; tự quy đổi các báo giá (nơi tính theo kg, nơi tính theo CBM, nơi chưa gồm phụ phí) rồi tự viết báo giá tiếng Anh gửi khách. |
| Mất bao lâu, bao lần? | Mất khoảng 45–90 phút thao tác nhắn tin/quy đổi cho mỗi đơn hỏi giá và phải chờ 1–3 ngày để nhận đủ phản hồi từ các NCC. |
| Insight / opportunity rút ra | Pain không chỉ nằm ở việc "tìm NCC", mà nằm ở **3 điểm nghẽn liên tiếp**: (1) Tính đóng gói & cân quy đổi (CBM) khi gộp nhiều mẫu cồng kềnh; (2) Nhắn lặp lại và đọc báo giá không cùng chuẩn; (3) Không nắm rõ giấy tờ hải quan (invoice, packing list, C/O, hun trùng, khai báo gỗ/mây tre) bên nào lo. |

Interview snapshot #2 (Phía nhà cung cấp vận chuyển / Forwarder nhỏ):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Nhân viên sale / điều phối báo giá tại đơn vị forwarder nhỏ chuyên tuyến Việt Nam – Mỹ |
| Câu nói đáng nhớ nhất (nguyên văn) | *"Khách nhắn hỏi giá toàn gửi mỗi cái ảnh sản phẩm với số lượng, không có kích thước thùng hay mã vùng bên Mỹ, tụi mình phải hỏi đi hỏi lại rất mất thời gian mà nhiều khi tư vấn xong khách im luôn; còn bảo công khai bảng giá lên web thì bên mình không làm đâu vì dễ bị ép giá."* |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Nhận tin nhắn hỏi giá lô đèn lồng tre và bình gốm đi Mỹ qua Zalo nhưng khách chỉ báo cân nặng sản phẩm, không tính vật liệu chèn chống vỡ và kích thước thùng carton; phải nhắn hỏi lại 4–5 lượt về chất liệu gỗ/tre và hình thức giao tận nhà (door-to-door). |
| Hiện đang xử lý bằng cách nào (workaround)? | Hỏi thủ công từng câu qua Zalo, tự ước lượng hoặc yêu cầu khách đóng thùng thử rồi mới tra bảng giá nội bộ và gửi báo giá qua tin nhắn/ảnh chụp/PDF. |
| Mất bao lâu, bao lần? | 15–30 phút tư vấn/khách; ngày nào cũng gặp các yêu cầu thiếu thông tin đóng gói cơ bản. |
| Insight / opportunity rút ra | Phía NCC **chỉ tham gia khi họ cũng được lợi**: (1) Nhận yêu cầu đã đủ thông tin (số thùng, cân nặng quy đổi, loại hàng, điểm đến); (2) Bớt thời gian tư vấn khách không chốt; (3) Có khách mới nhưng **không phải công khai bảng giá**; (4) Chỉ trả phí khi chốt được lô hàng. |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Thảo luận & phỏng vấn tình huống thực tế (Hộ KD + Forwarder) | 2 nhóm actor chính (kèm kế hoạch GĐ 0: 8–10 hộ, 4–5 NCC, 20 báo giá thật) | Xác nhận quy trình 6 bước thủ công qua Zalo; xác nhận nỗi đau tính sai cân nặng thể tích (CBM) của hàng thủ công cồng kềnh và sự lộn xộn của báo giá/giấy tờ. | (1) Hộ kinh doanh rất ít sẵn sàng trả phí cố định (điểm 2/5); (2) NCC nhỏ từ chối mô hình chợ so giá công khai và ngại nhập liệu phức tạp (điểm 2,5/5). |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**
1. **Đổi mô hình từ "Chợ so giá công khai" sang "Báo giá riêng tư (Private RFQ)":** Không công khai bảng giá của NCC; mỗi yêu cầu chuẩn chỉ gửi tới 3–5 NCC phù hợp và bảng so sánh chỉ hiển thị riêng cho hộ kinh doanh đã hỏi; xếp hạng NCC theo tổng điểm (giá, thời gian, giấy tờ, độ chính xác, tốc độ phản hồi) chứ không chỉ theo giá rẻ nhất.
2. **Đổi mô hình doanh thu (Miễn phí cho hộ kinh doanh):** Cung cấp miễn phí kho sản phẩm, công cụ tính đóng gói và mẫu báo giá tiếng Anh làm "mồi" thu hút hộ kinh doanh; nguồn thu chính lấy từ phí hoa hồng theo lô chốt thành công phía NCC.
3. **Bổ sung chiến lược dữ liệu 3 giai đoạn (Khởi đầu → Tích lũy → Tái sử dụng):** Vì hộ kinh doanh chưa có kích thước đóng gói chuẩn, giai đoạn đầu dùng AI ước tính từ ảnh/mô tả (hiển thị khoảng giá rộng); khi giao hàng, lấy **số cân đo thật của NCC** (vốn NCC bắt buộc phải cân để tính cước) đưa vào **thư viện dùng chung ẩn danh** để tái sử dụng cho các hộ khác khi đạt ngưỡng $\ge 3$ lô thật từ $\ge 2$ doanh nghiệp.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **Easyship** | https://www.easyship.com | Bước so giá chuyển phát nhanh quốc tế (DHL, FedEx, UPS...) cho từng kiện hàng nhỏ lẻ | So giá tự động nhiều hãng chuyển phát nhanh lớn, ước tính sẵn thuế và phí cho kiện hàng tiêu chuẩn | Không tính đóng gói khi gộp nhiều mẫu thủ công khác kích cỡ; không kết nối được các forwarder nhỏ tại Việt Nam; thiếu danh mục giấy tờ đặc thù hàng thủ công | **Không cạnh tranh** trực tiếp ở mảng chuyển phát nhanh kiện nhỏ với Easyship; có thể hiển thị giá này làm mốc tham chiếu |
| **Flexport · Shipa Freight · FreightAmigo** | https://www.flexport.com · https://www.shipafreight.com · https://www.freightamigo.com | Bước báo giá online đường biển ghép hàng (LCL) và hàng không (Air Freight) | Quy trình số hóa bài bản cho xuất nhập khẩu, quản lý chứng từ và lịch tàu minh bạch | Chỉ hợp với lô hàng lớn (thường từ mốc ~5 CBM / 750 kg trở lên); bắt buộc người bán phải **tự biết trước số CBM**; giao diện tiếng Anh phức tạp với hộ nhỏ | **Không cạnh tranh** ở mảng lô lớn nguyên container; cần giải bài toán **tính ra số thùng & CBM trước** cho các lô sỉ nhỏ của hộ thủ công |
| **Ship4wd** | https://ship4wd.com | Bước đặt chỗ và khóa giá vận chuyển cho doanh nghiệp nhỏ (SMB), hỗ trợ trả trước phí thông quan | Hướng tới SMB, cho phép khóa giá và có tùy chọn dịch vụ thông quan rõ ràng | Chủ yếu tập trung đường biển, không giải bài toán ước tính đóng gói hàng thủ công cồng kềnh hay kết nối các tuyến gom hàng linh hoạt từ VN | Học cách minh bạch hóa các khoản "đã bao gồm / chưa bao gồm thông quan & phụ phí" trên bảng so sánh |
| **Boxme Global** | https://boxme.asia | Bước fulfillment xuyên biên giới và kết nối nhiều hãng vận chuyển cho TMĐT | Hạ tầng kho bãi và tích hợp đơn hàng tự động cho người bán TMĐT Đông Nam Á | Thiết kế cho hàng TMĐT đóng gói sẵn theo SKU chuẩn; một số tuyến đi Mỹ trước đây phải trung chuyển qua kho Trung Quốc, chưa tối ưu cho lô hàng thủ công đóng thùng theo đơn | Tập trung vào ngách hàng thủ công mỹ nghệ đóng ghép thùng linh hoạt và đi trực tiếp qua các forwarder tuyến VN → Mỹ |
| **Etsy + Asendia** | https://www.etsy.com | Bước gửi hàng quốc tế từ Việt Nam cho người bán trên sàn Etsy | Gắn liền với đơn hàng phát sinh nội sàn Etsy | Chỉ áp dụng cho đơn lẻ trên sàn; tính năng mua nhãn vận chuyển (Etsy Shipping Labels) không mở đầy đủ cho người bán tại Việt Nam | Giải quyết bài toán cho các đơn khách Mỹ hỏi mua trực tiếp (qua mạng xã hội, web riêng, hội chợ hoặc đơn sỉ nhỏ nhiều mẫu) |
| **Forwarder Việt Nam truyền thống (qua Zalo)** | Thực tế thị trường vận chuyển VN – Mỹ | Bước tư vấn đóng gói, lo trọn gói vận chuyển và giấy tờ (C/O, hun trùng, thông quan) | Linh hoạt, hỗ trợ tiếng Việt, nhận làm trọn gói kể cả giấy tờ khó cho hộ nhỏ | Báo giá thủ công qua Zalo rất chậm (1–3 ngày), mỗi nơi tính một kiểu (kg, CBM, thiếu/đủ phụ phí), hộ phải nhắn hỏi lại nhiều nơi | **Đúng khoảng trống nhóm giải quyết:** Không thay thế forwarder Việt Nam mà số hóa luồng gửi yêu cầu chuẩn và chuẩn hóa bảng báo giá cho họ |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ quy trình hiện tại (khi khách Mỹ hỏi: *"50 bình gốm mẫu A và 20 giỏ mây mẫu B, giao tới Texas giá bao nhiêu?"*):

```text
HIỆN TẠI — 6 bước, tổng thời gian chờ 1–3 ngày (45–90 phút thao tác tay), 6/6 bước thủ công

[1 Tự đo, tự đoán xếp được mấy thùng: 15–20'] ← BOTTLENECK 1 (Dễ tính sai cân nặng quy đổi/CBM)
  → [2 Nhắn Zalo / Facebook cho 3–5 NCC vận chuyển: 10']
  → [3 Gửi lại ảnh, kích thước, số lượng cho từng nơi: 15']
  → [4 Trả lời câu hỏi bổ sung (hàng gỗ? hun trùng? giao tận nhà?): 15–20']
  → [5 Chờ báo giá, mỗi nơi tính một kiểu (kg, CBM, có/chưa có phụ phí): 1–3 ngày]
  → [6 Tự quy đổi, so sánh rồi mới báo giá tiếng Anh cho khách: 20–30'] ← BOTTLENECK 2 (Dễ sót phụ phí & giấy tờ)
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Hộ kinh doanh | Câu hỏi mua hàng của khách Mỹ (mẫu mã, số lượng, bang nhận hàng) | Ước tính nhẩm số thùng, kích thước thùng và cân nặng | 15–20 phút/đơn | Hàng thủ công nhẹ nhưng cồng kềnh, rất dễ quên tính vật liệu chèn và cân nặng quy đổi (thể tích) |
| 2 | Hộ kinh doanh | Danh sách 3–5 NCC vận chuyển quen trên Zalo / Facebook | Tin nhắn liên hệ hỏi giá từng nơi | 10 phút/đơn | Phải mở từng cuộc trò chuyện riêng lẻ |
| 3 | Hộ kinh doanh | Ảnh sản phẩm, kích thước, số lượng, địa chỉ giao tại Mỹ | Cùng một bộ thông tin gửi lặp lại cho 3–5 nơi | 15 phút/đơn | Thao tác copy-paste thủ công, dễ gửi thiếu thông tin |
| 4 | Hộ KD & NCC | Câu hỏi hỏi lại từ từng NCC (hàng gỗ? cần hun trùng? giao tận nhà?) | Tin nhắn trả lời bổ sung cho từng nơi | 15–20 phút (rải rác trong ngày) | Mỗi NCC hỏi thêm một kiểu, hộ không biết trước danh mục giấy tờ cần khai báo |
| 5 | NCC vận chuyển | Thông tin lô hàng sau khi hỏi đủ | Báo giá gửi qua tin nhắn Zalo, ảnh chụp hoặc file PDF | Chờ 4 giờ – 3 ngày | Đơn vị tính không đồng nhất (kg, CBM, đã gồm hoặc chưa gồm phụ phí/thông quan) |
| 6 | Hộ kinh doanh | 3–5 báo giá rời rạc từ các NCC | Bảng tính nhẩm so sánh + báo giá tiếng Anh gửi khách Mỹ | 20–30 phút/đơn | Tự quy đổi dễ nhầm, dễ báo thiếu phí hoặc phản hồi quá trễ làm mất khách |

**Bottleneck chính:**
1. **Bước 1 (Tự đoán đóng gói & CBM):** Hộ kinh doanh không có công cụ và dữ liệu chuẩn để tính số thùng và cân nặng quy đổi khi ghép nhiều mẫu hàng thủ công cồng kềnh.
2. **Bước 5–6 (Nhắn lặp lại & tự quy đổi báo giá lộn xộn):** Phải chờ và đọc hiểu các báo giá phi cấu trúc (kg vs CBM, ẩn phụ phí và giấy tờ hải quan) từ 3–5 NCC khác nhau trước khi báo được cho khách.

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
TƯƠNG LAI (BÁO GIÁ LIỀN TAY) — 6 bước, có giá ước tính trong vài phút & báo giá NCC dưới 4 giờ

[Bước 1: Chọn mẫu & số lượng trong kho sản phẩm (2')]
  ├── AI ước tính đóng gói từ ảnh/mô tả (GĐ A: Khởi đầu — chưa có dữ liệu, hiện khoảng giá rộng)
  └── AI so khớp với mẫu tương đồng trong thư viện chung (GĐ C: Tái sử dụng — khi đã có ≥ 3 lô thật từ ≥ 2 DN)
        ↓
[Bước 2: Tính số thùng, cân nặng thật & quy đổi, CBM + Gợi ý hình thức vận chuyển (<1')]
  ├── RULE (Công thức cố định): Tính số thùng, cân nặng quy đổi, CBM, khoảng giá tham chiếu
  └── RULE + AI giải thích: Gợi ý Chuyển phát nhanh / Hàng không / Đường biển gom hàng
        ↓
[Bước 3: Hỏi bù thông tin thiếu & Gửi yêu cầu báo giá chuẩn tới 3–5 NCC phù hợp (2')]
  └── AI Chatbot: Kiểm tra đủ trường bắt buộc (chất liệu gỗ/mây tre, điểm đến, hình thức giao) và phát RFQ chuẩn
      (Lưu ý: Ở GĐ 1 MVP, người vận hành vẫn gửi yêu cầu tới NCC thay hộ kinh doanh)
        ↓
[Bước 4: Đọc các báo giá của NCC về một bảng so sánh riêng tư (2')]
  ├── AI trích xuất: Đọc tin nhắn Zalo, ảnh, PDF của từng NCC về cùng chuẩn (tổng chi phí, thời gian, giấy tờ)
  └── CON NGƯỜI xác nhận: Kiểm tra số liệu AI trích xuất đối chiếu với bản báo giá gốc
        ↓
[Bước 5: Gợi ý giấy tờ hải quan & Soạn nháp báo giá tiếng Anh cho khách Mỹ (2')]
  ├── AI gợi ý + CON NGƯỜI duyệt: Danh sách giấy tờ theo loại hàng (invoice, packing list, C/O, hun trùng...) & NCC nào hỗ trợ
  └── AI soạn + CON NGƯỜI (Người bán) sửa: Ghép giá hàng và giá ship thành bản báo giá tiếng Anh
        ↓
[Bước 6: Chốt giá, chọn NCC & Gửi báo giá cho khách + Cập nhật số cân đo thật (2')]
  ├── CON NGƯỜI quyết định cuối cùng: Chọn NCC và gửi báo giá cho khách Mỹ
  └── VÒNG LẶP DỮ LIỆU (Rule + Con người): Khi giao hàng, NCC ghi số cân đo thật → cập nhật thư viện dùng chung

──────────────────────────────────────────────────────────────────────────────
BOUNDARY (Ranh giới an toàn):
1. AI KHÔNG tự tính tiền: Mọi phép tính số thùng, CBM, cân nặng quy đổi và tổng tiền bắt buộc chạy bằng Công thức (Rule).
2. AI KHÔNG tự tính thuế nhập khẩu Mỹ ở MVP (do quy định thay đổi nhanh); chỉ dẫn nguồn chính thức kèm ngày cập nhật và để NCC xác nhận.
3. AI KHÔNG tự chốt NCC và KHÔNG tự gửi báo giá cho khách Mỹ.
4. Báo giá của NCC hoàn toàn riêng tư (chỉ hiện cho người hỏi), không lập bảng giá công khai.
5. Thư viện dùng chung chỉ chia sẻ thông số vật lý đã ẩn danh khi hộ đồng ý; chỉ gắn nhãn "Đã kiểm chứng" khi có ≥ 3 lô thật từ ≥ 2 doanh nghiệp; số lệch nhiều phải chờ người duyệt, không tự gộp.

PHƯƠNG ÁN QUAY VỀ (Fallback khi AI sai hoặc thiếu dữ liệu):
1. Khi sản phẩm mới chưa có dữ liệu trong thư viện: Hệ thống gắn nhãn "Độ tin cậy thấp · khoảng giá rộng", cho phép người bán tự nhập kích thước thùng hoặc chờ số cân đo thật từ NCC.
2. Khi AI đọc báo giá NCC (ảnh/PDF/tin nhắn) không chắc chắn hoặc thiếu thông tin phụ phí: Hiển thị nguyên văn báo giá gốc ngay cạnh bảng so sánh và đánh dấu cảnh báo để người bán/người vận hành tự nhập hoặc hỏi lại NCC.
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 6 bước thủ công rời rạc | 6 bước liền mạch (nhập 1 lần, dùng lại cho mọi đơn) | Loại bỏ hoàn toàn việc gửi lại thông tin cho từng NCC |
| Tổng thời gian có báo giá | 1–3 ngày chờ (45–90' thao tác tay) | Giá ước tính: **vài phút**; Báo giá thật từ NCC: **dưới 4 giờ** (~10' thao tác) | Số tin nhắn qua lại với NCC giảm $\ge 50\%$ |
| Số bước thủ công | 6/6 bước | 2/6 bước chính (Xác nhận báo giá/giấy tờ & Chốt chọn NCC) | Con người vẫn giữ 100% quyền duyệt tiền và chốt đơn |
| Bottleneck chính | Tự đoán số thùng/CBM & tự quy đổi 3–5 báo giá khác chuẩn | Chờ NCC phản hồi báo giá (đã rút ngắn còn < 4 giờ nhờ yêu cầu đủ thông tin ngay từ đầu) | Độ lệch giá ship đã báo so với hóa đơn thật giảm xuống **< 10%** |
| Rủi ro mới phát sinh | — | (1) AI ước tính đóng gói sai lúc đầu chưa có dữ liệu; (2) AI đọc sót phụ phí từ ảnh/PDF của NCC; (3) Dữ liệu sai lan sang thư viện chung | Giảm thiểu bằng: Công thức tính tiền + Hiện bản gốc báo giá + Ngưỡng kiểm chứng $\ge 3$ lô thật từ $\ge 2$ DN + Ưu tiên số cân đo thật của NCC |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Hộ kinh doanh hàng thủ công mỹ nghệ tại Việt Nam bán hàng cho khách tại Mỹ |
| **Quy trình** | Khi khách Mỹ hỏi mua nhiều mẫu sản phẩm: Tự đo và đoán số thùng → Nhắn Zalo/FB cho 3–5 NCC vận chuyển → Gửi lại ảnh, kích thước, số lượng cho từng nơi → Trả lời câu hỏi bổ sung (gỗ, hun trùng, giao tận nhà) → Chờ báo giá (mỗi nơi tính theo kg/CBM/phụ phí khác nhau) → Tự quy đổi, so sánh rồi mới báo cho khách |
| **Bottleneck** | Tự ước tính đóng gói (số thùng, cân nặng quy đổi/CBM) dễ sai và phải nhắn tin lặp lại, chờ đợi rồi tự quy đổi các báo giá không đồng nhất từ 3–5 NCC |
| **Impact** | Mất 1–3 ngày mới báo được giá ship cho khách Mỹ, dễ báo giá thiếu cước (do hàng nhẹ nhưng cồng kềnh bị tính cân thể tích hoặc sót phí giấy tờ hải quan), làm giảm tỷ lệ chốt đơn hoặc ăn vào lợi nhuận |
| **Success Metric** (baseline → target, cách đo) | Thời gian từ lúc khách hỏi đến lúc báo được giá ship giảm từ 1–3 ngày xuống **dưới 4 giờ** (có giá ước tính trong vài phút); đo qua 20 báo giá thật thu thập ở GĐ 0 và thử nghiệm ở GĐ 1 |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI không tự chốt NCC, không tự gửi báo giá cho khách, không tự tính tiền ngoài công thức; người bán phải kiểm tra bảng so sánh báo giá và duyệt bản nháp tiếng Anh trước khi gửi |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- **Phản biện 1 (Về phía cung của thị trường):** *"Problem Statement v0 mới chỉ nhìn từ phía hộ kinh doanh. Nếu các NCC vận chuyển nhỏ sợ bị so giá công khai và không chịu tham gia thì hệ thống không có báo giá thật."* → **Đồng ý hoàn toàn.** Ở v1, nhóm bổ sung cơ chế **báo giá riêng tư** (không công khai bảng giá, chỉ gửi 3–5 NCC, xếp hạng theo tổng điểm chứ không chỉ theo giá) và làm rõ giá trị cho phía NCC.
- **Phản biện 2 (Về độ tin cậy của ước tính đóng gói):** *"Hàng thủ công mỗi cái một kiểu, nếu AI chỉ nhìn ảnh để đoán số thùng thì sai số rất lớn."* → **Đồng ý.** Nhóm bổ sung chiến lược **Thư viện đóng gói dùng chung 3 giai đoạn (A: Khởi đầu → B: Tích lũy → C: Tái sử dụng)** dựa trên **số cân đo thật của NCC khi nhận hàng**, và quy định chỉ dùng số tự động khi đã kiểm chứng qua $\ge 3$ lô thật từ $\ge 2$ doanh nghiệp.
- **Phản biện 3 (Về Success Metric):** *"Chỉ đo thời gian báo giá dưới 4 giờ là chưa đủ; nếu báo nhanh nhưng lệch xa hóa đơn thực tế hoặc vẫn phải nhắn tin hỏi lại nhiều lần thì không giải quyết được gốc vấn đề."* → **Đồng ý.** Ở v1, nhóm mở rộng thành bộ **4 chỉ số thành công**: thời gian báo giá (< 4 giờ), số tin nhắn với NCC (giảm $\ge 50\%$), độ lệch giá so với hóa đơn thật (< 10%) và tỷ lệ yêu cầu chốt thành lô hàng ($\ge 30\%$).

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **Độ mơ hồ Cao × Độ phức tạp Trung bình–Cao** (đối với khâu ước tính đóng gói từ ảnh/mô tả tự do, chuẩn hóa báo giá lộn xộn từ Zalo/ảnh/PDF và gom dữ liệu nhiều doanh nghiệp), kết hợp với **Độ mơ hồ Thấp** (đối với khâu tính số thùng, CBM, cân nặng quy đổi và tổng chi phí).

Vì sao:
- **Độ mơ hồ cao ở đầu vào & đầu ra ngôn ngữ/hình ảnh:** Mỗi hộ đặt tên sản phẩm khác nhau, hình dáng hàng thủ công đa dạng (bình gốm, giỏ mây, đèn lồng tre), và mỗi NCC trả lời báo giá một kiểu qua tin nhắn Zalo, ảnh chụp hoặc PDF. Các tác vụ này không thể viết if/else cứng mà cần AI ước tính, trích xuất và so khớp.
- **Độ phức tạp quy trình gồm 6 bước nối tiếp nhưng thứ tự cố định:** Luồng đi từ *Kho sản phẩm → Tính đóng gói → Tạo yêu cầu chuẩn → Đọc báo giá NCC → Kiểm tra giấy tờ & soạn báo giá tiếng Anh → Chốt đơn & cập nhật số cân thật*. Vì các bước đã định sẵn rõ ràng và phép tính tiền đòi hỏi độ chính xác toán học tuyệt đối (dùng **Rule**), mức can thiệp phù hợp nhất là **Workflow có bước AI + vòng lặp dữ liệu**, tuyệt đối không dùng Agent tự quyết.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Lập bảng tính thủ công (Excel/Google Sheets) + mẫu câu hỏi chuẩn trên Zalo cho từng hộ tự đo và tự nhập | Hộ chỉ bán vài mẫu cố định đã biết sẵn quy cách đóng thùng và chỉ gửi qua 1 NCC quen duy nhất | Mỗi hộ phải tự tính từ đầu, dữ liệu nằm rời rạc, không đối chiếu được với lô thật, không tái sử dụng chéo giữa các hộ được | Không chọn (chỉ dùng bảng tính làm mốc so sánh độ chính xác) |
| **Rule** | Dùng công thức cố định tính số thùng, cân nặng thật và cân nặng quy đổi (CBM), cộng tổng phí và gợi ý hình thức vận chuyển (Express / Air / Đường biển gom hàng) theo ngưỡng | Khi đầu vào kích thước thùng đã có sẵn chuẩn xác và các NCC chịu nhập báo giá vào biểu mẫu cố định | Không ước tính được cách đóng gói khi chưa có dữ liệu; không đọc được báo giá dạng tin nhắn/ảnh/PDF tự do của NCC; không gộp được sản phẩm tương đồng khác tên | **Chọn cho bước tính đóng gói (CBM/cân quy đổi) và phép tính tiền** |
| **Workflow** | Các bước định sẵn: **AI** ước tính đóng gói lúc đầu & so khớp thư viện về sau → **Rule (Công thức)** tính thùng/CBM → **AI Chatbot** hỏi bù thông tin thiếu → **AI** trích xuất báo giá Zalo/ảnh/PDF về bảng so sánh + gợi ý giấy tờ + soạn nháp tiếng Anh → **Con người** xác nhận và chốt NCC | Khi quy trình 6 bước đã rõ ràng nhưng cần AI cầu nối ở các bước xử lý ảnh/văn bản phi cấu trúc và tích lũy thư viện dùng chung qua nhiều lô thật | AI ước tính lệch ở giai đoạn chưa có dữ liệu hoặc đọc nhầm trường trong ảnh báo giá của NCC | **Chọn (Workflow có bước AI + vòng lặp dữ liệu)** |
| **Agent** | AI tự động liên hệ thương lượng giá với các NCC, tự tra cứu và tính thuế hải quan Mỹ, tự chọn NCC và gửi báo giá chốt đơn trực tiếp cho khách Mỹ | Khi toàn bộ NCC số hóa API, quy định hải quan cố định và người bán ủy quyền hoàn toàn quyết định tài chính | Rủi ro cực cao: tính sai giá/thuế gây lỗ nặng, lộ thông tin giữa các NCC, mất kiểm soát chất lượng dịch vụ | **Không chọn** |

**Mức chọn:** **Workflow có bước AI + vòng lặp dữ liệu** (kết hợp chặt chẽ giữa **Rule công thức**, **AI xử lý phi cấu trúc** và **Con người phê duyệt**).

**Vì sao không chọn mức đơn giản hơn:**
- Nếu chỉ dùng **No AI (bảng tính thủ công cho từng hộ)** hoặc **Rule thuần**: Khi khách Mỹ hỏi đơn gộp nhiều mẫu mới, hộ kinh doanh vẫn bị kẹt ở bước chưa có thông số đóng gói chuẩn, dữ liệu của hộ này không giúp ích được cho hộ khác làm cùng loại sản phẩm (bình gốm 30cm, giỏ mây 40cm), và người bán vẫn phải tự đọc/gõ lại từng tin nhắn hay ảnh báo giá lộn xộn từ 3–5 forwarder trên Zalo. AI đóng vai trò quyết định ở **giai đoạn khởi đầu chưa có dữ liệu** (ước tính từ ảnh/mô tả) và **giai đoạn tái sử dụng** (so khớp sản phẩm tương đồng dù khác tên gọi, phát hiện số đo bất thường như nhầm cm với mm, và trích xuất báo giá đa định dạng).

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | 1. Ước tính thông số đóng gói ban đầu (số cái/thùng, kích thước thùng, vật liệu chèn, cân nặng) từ ảnh/mô tả khi chưa có dữ liệu, hoặc so khớp với mẫu tương đồng đã kiểm chứng trong thư viện chung.<br>2. Phát hiện thông tin còn thiếu để hỏi bù và phát hiện số đo bất thường (VD: nhầm cm và mm).<br>3. Trích xuất báo giá từ tin nhắn, ảnh, PDF của 3–5 NCC thành một bảng so sánh chuẩn.<br>4. Gợi ý danh sách giấy tờ hải quan theo loại hàng và soạn bản nháp báo giá tiếng Anh gửi khách Mỹ. |
| **Judgment** — con người cân nhắc, quyết định gì? | 1. Hộ kinh doanh (và người vận hành ở GĐ 1) kiểm tra thông số đóng gói, xác nhận các khoản phí/phụ phí AI trích xuất từ báo giá gốc của NCC.<br>2. Duyệt danh mục giấy tờ hải quan và chỉnh sửa bản nháp báo giá tiếng Anh.<br>3. Cân nhắc giữa giá cước, thời gian giao, khả năng hỗ trợ giấy tờ và độ uy tín để chọn NCC phù hợp nhất. |
| **Action** — hành động cuối cùng là gì, ai làm? | Hộ kinh doanh chốt chọn NCC vận chuyển và gửi báo giá chính thức cho khách Mỹ; khi nhận hàng thật, NCC cân đo thực tế và ghi nhận số liệu vào hệ thống. |
| **Outcome** — đo kết quả bằng gì? | 1. Thời gian từ lúc khách hỏi đến lúc báo được giá ship: **dưới 4 giờ**.<br>2. Số tin nhắn với NCC cho mỗi lần báo giá: **giảm $\ge 50\%$**.<br>3. Độ lệch giá ship đã báo so với hóa đơn thật: **dưới 10%**.<br>4. Tỷ lệ yêu cầu chốt thành lô hàng: **$\ge 30\%$**. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | - **Từ hộ kinh doanh (có sẵn):** Ảnh sản phẩm, kích thước, cân nặng, chất liệu, số lượng từng mẫu, điểm đến tại Mỹ.<br>- **Từ NCC (có khi phản hồi):** Tin nhắn Zalo, ảnh chụp bảng giá hoặc file PDF báo giá.<br>- **Từ thư viện dùng chung (tích lũy dần):** Số cân đo thật của NCC khi nhận hàng và hóa đơn cước thật của các lô hàng trước. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | 1. **Số NCC cân đo thật khi nhận hàng** và **hóa đơn cước thật sau khi giao**: đối chiếu với ước tính ban đầu để AI học sai lệch (hệ số cồng kềnh, cách chèn chống vỡ, tuyến hay phát sinh phụ phí) và nâng mức tin cậy từ *Khởi đầu (A)* → *Tích lũy (B — dựa trên 3 lô thật)* → *Tái sử dụng (C — đã kiểm chứng qua $\ge 3$ lô từ $\ge 2$ DN)*.<br>2. Các chỉnh sửa của người dùng trên bảng trích xuất báo giá NCC và bản nháp tiếng Anh. |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
  - **Được hỗ trợ (Augment).** Bằng chứng từ phân tích hai phía thị trường: (1) Cước vận chuyển quốc tế và giấy tờ hải quan (hun trùng, C/O, khai báo hàng gỗ/mây tre) ảnh hưởng trực tiếp tới biên lợi nhuận và rủi ro bị giữ hàng tại Mỹ, nên hộ kinh doanh cần hệ thống tính nháp và gom bảng so sánh chuẩn nhưng phải tự duyệt giá trước khi gửi khách; (2) Phía NCC vận chuyển nhỏ không muốn công khai bảng giá tự động mà chỉ báo giá riêng tư cho từng yêu cầu cụ thể.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:
  - **Bỏ sót (False Negative) tệ hơn rất nhiều so với báo nhầm.** Nếu hệ thống bỏ sót cân nặng thể tích (tính theo cân thật thay vì CBM cho hàng nhẹ nhưng cồng kềnh), bỏ sót phụ phí trong báo giá của NCC, hoặc bỏ sót giấy tờ bắt buộc (như hun trùng/khai báo gỗ mây tre), hộ kinh doanh sẽ báo giá hớ cho khách Mỹ (chịu lỗ tiền ship) hoặc bị hải quan giữ hàng.
  - **Cách thiết kế xử lý:**
    1. Không để AI tự tính tiền; dùng công thức (Rule) luôn tính cả cân nặng thật lẫn cân nặng quy đổi (CBM) và lấy mức cao hơn theo chuẩn vận chuyển.
    2. Khi mẫu sản phẩm chưa đủ dữ liệu kiểm chứng, luôn hiển thị nhãn *"Độ tin cậy thấp · khoảng giá rộng (min–max)"* thay vì một con số đơn lẻ.
    3. Trên bảng so sánh báo giá NCC, luôn hiển thị kèm bản gốc (tin nhắn/ảnh/PDF) và buộc người dùng xác nhận các khoản phụ phí/giấy tờ trước khi xuất báo giá cho khách.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | **Phía cầu:** Hộ kinh doanh hàng thủ công mỹ nghệ tại Việt Nam bán đơn gộp/sỉ nhỏ sang Mỹ.<br>**Phía cung:** Nhà cung cấp vận chuyển (forwarder nhỏ) chuyên tuyến Việt Nam → Mỹ đang báo giá thủ công. |
| **Quy trình** | Nhập/chọn mẫu và số lượng từ kho sản phẩm → Tính số thùng, cân nặng quy đổi (CBM) và gợi ý hình thức vận chuyển → Chatbot hỏi bù thông tin thiếu & gửi yêu cầu chuẩn tới 3–5 NCC phù hợp → Trích xuất báo giá của các NCC về một bảng so sánh riêng tư → Kiểm tra giấy tờ hải quan, xuất báo giá tiếng Anh cho khách Mỹ → Chốt NCC và ghi nhận số cân đo thật sau mỗi lô vào thư viện dùng chung. |
| **Bottleneck** | (1) Ước tính quy cách đóng gói và cân nặng quy đổi (CBM) khi khách mua gộp nhiều mẫu hàng thủ công cồng kềnh; (2) Nhắn hỏi lặp lại và chuẩn hóa các báo giá phi cấu trúc (tin nhắn, ảnh, PDF) từ nhiều NCC. |
| **Impact** | Mất 1–3 ngày chờ báo giá, tốn nhiều tin nhắn qua lại với từng NCC, dễ báo thiếu phí vận chuyển (do lệch CBM hoặc phụ phí) và rủi ro vướng giấy tờ hải quan khi vào Mỹ. |
| **Success Metric** (baseline → target, cách đo) | 1. **Thời gian từ lúc khách hỏi đến lúc báo được giá ship:** từ 1–3 ngày (đo ở GĐ 0) xuống **dưới 4 giờ** (giá ước tính có trong vài phút).<br>2. **Số tin nhắn với NCC cho mỗi lần báo giá:** **giảm $\ge 50\%$** so với baseline GĐ 0.<br>3. **Độ lệch giá ship đã báo so với hóa đơn thật:** **dưới 10%**.<br>4. **Tỷ lệ yêu cầu chốt thành lô hàng:** **$\ge 30\%$**. |
| **Boundary** | - AI không tự tính tiền (phép tính đóng gói/CBM/cước dùng công thức Rule).<br>- Không tự tính thuế hải quan Mỹ ở MVP (chỉ dẫn nguồn chính thức kèm ngày cập nhật và để NCC xác nhận).<br>- Không công khai bảng giá NCC; mỗi yêu cầu chỉ gửi 3–5 NCC.<br>- Chỉ chia sẻ thông số vật lý đã ẩn danh vào thư viện chung khi hộ đồng ý và chỉ gắn nhãn *"Đã kiểm chứng"* khi có $\ge 3$ lô thật từ $\ge 2$ doanh nghiệp; số lệch nhiều phải chờ người duyệt. |
| **AI intervention point** | 1. **Kho sản phẩm & thư viện chung:** AI ước tính đóng gói lúc đầu từ ảnh/mô tả; AI so khớp mẫu tương đồng và phát hiện số đo bất thường (cm vs mm) về sau.<br>2. **Yêu cầu báo giá chuẩn (RFQ):** Chatbot AI hỏi bù thông tin thiếu.<br>3. **Đọc báo giá NCC:** AI trích xuất tin nhắn, ảnh, PDF thành bảng so sánh.<br>4. **Giấy tờ & Báo giá khách Mỹ:** AI gợi ý danh mục giấy tờ theo loại hàng và soạn nháp báo giá tiếng Anh. |
| **Mức chọn** | **Workflow** (Workflow có bước AI + Công thức Rule + Vòng lặp dữ liệu thư viện chung) |
| **Rủi ro & người kiểm tra** | - **Rủi ro:** AI ước tính sai số thùng lúc đầu; AI đọc nhầm/bịa thông tin từ báo giá NCC; dữ liệu đóng gói sai lan sang doanh nghiệp khác.<br>- **Người kiểm tra:** Hộ kinh doanh (và người vận hành ở GĐ 1) xác nhận bảng trích xuất báo giá đối chiếu bản gốc và duyệt báo giá tiếng Anh; NCC đối tác cân đo thật khi nhận hàng để xác thực dữ liệu gốc. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| **Actor** | Chỉ nêu hộ kinh doanh hàng thủ công | Bổ sung **NCC vận chuyển nhỏ** làm actor phía cung và thu hẹp rõ tuyến **Việt Nam → Mỹ** | Phía NCC chỉ tham gia khi họ nhận được yêu cầu đủ thông tin và không bị công khai bảng giá; thu hẹp 1 tuyến để giải bài toán con gà – quả trứng |
| **Success Metric** | Chỉ đo thời gian có báo giá (< 4 giờ) | Bộ 4 chỉ số: Thời gian (< 4 giờ), Số tin nhắn (giảm $\ge 50\%$), Độ lệch hóa đơn thật (< 10%), Tỷ lệ chốt ($\ge 30\%$) | Đảm bảo báo giá không chỉ nhanh mà còn sát thực tế hóa đơn và tạo ra đơn hàng thật cho NCC |
| **Boundary & Chiến lược dữ liệu** | Chỉ giới hạn "AI không tự gửi báo giá" | Bổ sung quy tắc tách **Rule công thức tính tiền**, **không tự tính thuế Mỹ ở MVP**, và **quy tắc thư viện dùng chung** (ẩn danh, $\ge 3$ lô từ $\ge 2$ DN) | Ngăn rủi ro AI làm tròn/tính sai tiền, rủi ro pháp lý thuế quan Mỹ, và rủi ro dữ liệu sai của 1 hộ làm hỏng ước tính của toàn hệ thống |

**Tiêu chí đánh giá đầu ra của AI (4 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | **Ước tính & so khớp thông số đóng gói** | Nêu rõ khoảng min–max (số cái/thùng, kích thước thùng, vật liệu chèn), gắn đúng nhãn độ tin cậy (*Khởi đầu / Dựa trên N lô thật / Đã kiểm chứng*), phát hiện được lỗi đơn vị (cm vs mm) và giúp độ lệch báo giá tiến tới **< 10%** so với hóa đơn thật | Đưa ra một con số cứng không có khoảng dự phòng khi chưa có lô thật, hoặc tự gộp dữ liệu khi số đo lệch nhiều mà không chờ người duyệt |
| 2 | **Trích xuất báo giá của NCC sang bảng so sánh** | Mọi con số cước phí, đơn vị tính (kg, CBM), thời gian giao và trạng thái phụ phí/giấy tờ khớp 100% với tin nhắn/ảnh/PDF gốc của NCC; luôn hiển thị kèm bản gốc | AI tự tính toán lại tiền cước, tự suy diễn "đã bao gồm phụ phí" khi NCC không nêu, hoặc bỏ sót điều kiện trong báo giá gốc |
| 3 | **Gom đủ thông tin trong yêu cầu báo giá chuẩn (RFQ)** | Yêu cầu gửi tới 3–5 NCC có đầy đủ: danh sách mẫu, số thùng, cân nặng thật & quy đổi (CBM), chất liệu hàng (gỗ/mây tre/gốm), điểm đến tại Mỹ, nhu cầu giấy tờ/giao tận nhà | Thiếu trường thông tin cơ bản khiến NCC phải nhắn hỏi lại hộ kinh doanh như quy trình cũ |
| 4 | **Gợi ý giấy tờ hải quan & Soạn báo giá tiếng Anh** | Liệt kê đúng nhóm giấy tờ cần lưu ý theo chất liệu (invoice, packing list, C/O, hun trùng, khai báo gỗ/mây tre) kèm nguồn/ngày cập nhật; bản nháp tiếng Anh ghép đúng giá hàng + giá ship đã duyệt | Tự ý tính thuế nhập khẩu Mỹ khi chưa được xác nhận, hoặc bịa đặt cam kết pháp lý/thời gian thông quan không có trong báo giá của NCC |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | **Trung bình** | Pain báo giá chậm và tính thiếu cân nặng quy đổi (CBM) là có thật và lặp lại (điểm 4/5), nhưng tần suất đơn đi Mỹ ngoài sàn (3/5) và mức sẵn sàng trả tiền trực tiếp của hộ kinh doanh thấp (2/5). Đã giảm rủi ro bằng cách **miễn phí cho hộ kinh doanh** và dùng công cụ tính đóng gói/mẫu báo giá tiếng Anh làm "mồi". |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | **Trung bình** | Hộ kinh doanh ngại nhập dữ liệu dài và NCC quen dùng Zalo hơn mở cổng mới. Đã giảm rủi ro bằng cách cho phép nhập bằng ảnh/chatbot/Zalo, chỉ bắt buộc vài trường cốt lõi, nhập 1 lần dùng lại cho mọi đơn, và ở GĐ 1 có người vận hành hỗ trợ gửi yêu cầu. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | **Trung bình** | Khả thi kỹ thuật cao (4/5), chi phí hosting/database và AI theo lượt cho MVP rất thấp. Thách thức lớn nhất là **lúc đầu chưa có dữ liệu đóng gói thật** và nguy cơ **dữ liệu sai lan sang nhiều doanh nghiệp** (Mức Cao nếu không kiểm soát) → giải quyết bằng lộ trình tích lũy A→B→C, ưu tiên số cân đo thật của NCC và ngưỡng kiểm chứng $\ge 3$ lô thật từ $\ge 2$ doanh nghiệp. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | **Cao** | Ba rủi ro lớn nhất nằm ở mô hình thị trường và quy định: (1) **NCC không tham gia** vì sợ bị so giá, sợ mất khách quen (điểm sẵn sàng 2,5/5); (2) **Bài toán con gà – quả trứng** giữa số lượng hộ và số lượng NCC; (3) **Thuế và quy định hải quan Mỹ thay đổi nhanh**. |

### 8.2. Kết luận

**Quyết định:** **Not Yet** *(Cần hoàn tất GĐ 0 trong 2 tuần để kiểm chứng định lượng trước khi chuyển sang Go — Concierge MVP GĐ 1 trong phạm vi thu hẹp)*.

**Lý do:**
- Bài toán rất đáng làm **nếu thu hẹp phạm vi** (một tuyến Việt Nam → Mỹ, một nhóm hàng thủ công, vài NCC đầu tiên) vì giải quyết đúng khoảng trống mà các nền tảng quốc tế (Easyship, Flexport, Ship4wd) đang bỏ trống và tạo ra tài sản dữ liệu đóng gói dùng chung càng dùng càng chính xác.
- Tuy nhiên, theo nguyên tắc quản trị rủi ro: hiện tại các chỉ số baseline đang là ước lượng cần đo ở GĐ 0 và rủi ro **Viability (phía NCC có chịu tham gia hay không)** đang ở mức **Cao**. Vì vậy, nhóm chọn **Not Yet** ở thời điểm hiện tại để chạy GĐ 0 (2 tuần khám phá không cần code), nếu đạt tiêu chí qua cửa sẽ lập tức **Go** vào GĐ 1 (MVP dữ liệu + AI).

**Nếu Not Yet — cần kiểm chứng gì trước (GĐ 0 — 2 tuần: Khám phá):**
- Phỏng vấn trực tiếp **8–10 hộ kinh doanh hàng thủ công** và **4–5 NCC vận chuyển nhỏ** chuyên tuyến Mỹ.
- Thu thập **20 báo giá thật** và đo chính xác thời gian báo giá, số tin nhắn qua lại và độ lệch giữa giá báo với hóa đơn thực tế hiện tại.
- **Tiêu chí qua cửa (Gate GĐ 0 → Go GĐ 1):** $\ge 60\%$ hộ kinh doanh xác nhận đây là nút thắt lớn VÀ $\ge 3$ NCC vận chuyển đồng ý thử nghiệm nhận yêu cầu báo giá riêng tư.

**Nếu Go (sau khi qua cửa GĐ 0) — Pilot nhỏ nhất (GĐ 1 — 4–6 tuần: MVP dữ liệu + AI):**
- Thu hẹp phạm vi: **1 tuyến (Việt Nam → Mỹ)**, **1–2 nhóm hàng thủ công chính** (VD: gốm, mây tre đan), làm việc với **3–5 NCC đối tác quen**.
- Xây dựng trang web đơn giản nhập ảnh, kích thước, số lượng; dùng AI ước tính đóng gói + công thức (Rule) tính CBM/cân quy đổi.
- **Vận hành bán thủ công (Concierge MVP):** Người vận hành của nhóm nhận yêu cầu chuẩn và gửi tới 3–5 NCC qua Zalo thay cho hộ kinh doanh; sau đó dùng AI gom báo giá về bảng so sánh riêng tư.
- **Tích lũy thư viện:** NCC đối tác ghi lại số cân đo thật của mỗi lô hàng (qua Zalo / ảnh phiếu cân — điều kiện tính lô hợp lệ) để xây dựng thư viện dùng chung.
- **Tiêu chí qua cửa GĐ 1:** Đo được sai số ước tính đóng gói; thời gian báo giá giảm $\ge 50\%$; mỗi nhóm hàng chính tích lũy được $\ge 3$ lô hàng thật.

**Nếu No-Go — nên làm gì thay AI:**
- Nếu kết thúc GĐ 0 mà các NCC nhỏ từ chối tham gia (dưới 3 NCC) hoặc các hộ kinh doanh chỉ gửi kiện nhỏ lẻ qua sàn đã có sẵn dịch vụ ship: **Không xây dựng nền tảng kết nối hai đầu**. Thay vào đó, đóng gói công thức tính số thùng & cân nặng quy đổi (Rule) kèm checklist giấy tờ hải quan hàng thủ công và mẫu báo giá tiếng Anh thành một **web tool / bảng tính miễn phí** để hộ kinh doanh tự sử dụng.

**Ngưỡng dừng (Kill Criteria):**
- **Tại cổng GĐ 0 (sau 2 tuần):** Nếu **dưới 60% hộ kinh doanh** xác nhận đây là nút thắt hoặc **dưới 3 NCC** chịu thử nghiệm → **Dừng dự án (No-Go)**, chuyển sang phương án công cụ tính công thức miễn phí.
- **Tại cổng GĐ 1 (sau 4–6 tuần MVP):** Nếu thời gian báo giá **không giảm được $\ge 50\%$**, hoặc không thu thập được **$\ge 3$ lô cân đo thật** cho mỗi nhóm hàng chính → **Dừng lên GĐ 2 (Web + Chatbot tự động)**, giữ ở quy trình bán thủ công để tìm nguyên nhân.
- **Tại cổng GĐ 2–3:** Nếu có dưới 20 hộ dùng thường xuyên, thời gian NCC phản hồi trung bình **vượt quá 4 giờ**, hoặc độ lệch giá báo so với hóa đơn thật **vượt quá 10%** mà không cải thiện được qua thư viện chung → **Dừng mở rộng thu phí**.

---

## 9. Hạn chế và hướng tiếp theo

**Hạn chế hiện tại:**
- Các con số baseline (thời gian chờ 1–3 ngày, số lượng tin nhắn, độ lệch hóa đơn) và điểm chấm mức độ sẵn sàng của hộ kinh doanh (2/5) / NCC (2,5/5) mới dừng ở mức giả định và khảo sát định tính ban đầu, cần được đo đạc định lượng qua 20 báo giá thật ở GĐ 0.
- Ở giai đoạn đầu (GĐ 1), hệ thống chưa có dữ liệu đóng gói thực tế nên khoảng giá ước tính của AI còn rộng, và chi phí lớn nhất nằm ở công sức của **người vận hành** làm cầu nối gửi yêu cầu cho NCC.
- Chưa giải quyết bài toán tự động tính thuế nhập khẩu Mỹ ở MVP do chính sách thuế và hải quan Mỹ biến động nhanh.

**Hướng tiếp theo (Lộ trình 4 giai đoạn):**
- **GĐ 0 (2 tuần — Khám phá):** Phỏng vấn 8–10 hộ kinh doanh và 4–5 NCC; thu thập 20 báo giá thật; đo baseline thời gian và độ lệch giá.
- **GĐ 1 (4–6 tuần — MVP dữ liệu + AI):** Triển khai web đơn giản nhập ảnh/kích thước/số lượng + AI ước tính đóng gói + người vận hành điều phối báo giá với 3–5 NCC quen + thu thập số cân đo thật cho $\ge 3$ lô/nhóm hàng.
- **GĐ 2 (6–8 tuần — Web + Chatbot):** Hoàn thiện kho sản phẩm, chatbot tự động hỏi bù thông tin, cổng NCC trả lời báo giá (mục tiêu < 4 giờ), AI đọc báo giá đa định dạng về bảng so sánh riêng tư cho 20 hộ dùng thường xuyên; tiếp cận qua hiệp hội làng nghề, chương trình xúc tiến xuất khẩu, cộng đồng bán hàng Etsy.
- **GĐ 3 (Sau 3 tháng — Mở rộng & Thu phí):** NCC tự nhập bảng giá riêng để hệ thống báo giá tức thì; hoàn thiện danh sách giấy tờ theo ngành hàng; mở mô hình thu phí theo lô chốt thành công từ NCC, gói Pro cho hộ (invoice, packing list, báo giá tiếng Anh) và hoa hồng dịch vụ GTGT (C/O, hun trùng, bảo hiểm, đóng gói).

## 10. Tài liệu tham khảo

- Canvas phân tích đề tài nhóm 3TDL — *Báo Giá Liền Tay: báo giá vận chuyển trong vài phút cho hộ làm hàng thủ công bán sang Mỹ*: https://gemini.google.com/share/c8c627a09658
- Các nền tảng và dịch vụ vận chuyển quốc tế đối chiếu (tra cứu 11/2026):
  - Easyship: https://www.easyship.com
  - Flexport: https://www.flexport.com
  - Shipa Freight: https://www.shipafreight.com
  - FreightAmigo: https://www.freightamigo.com
  - Ship4wd: https://ship4wd.com
  - Boxme Global: https://boxme.asia
  - Etsy Shipping & Asendia: https://www.etsy.com

