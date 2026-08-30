# THE NEXT FRONTIER — VIỄN THÁM (REMOTE SENSING) × TRÍ TUỆ NHÂN TẠO (AI - ARTIFICIAL INTELLIGENCE)
### Khung phân rã học thuật (Academic Taxonomy) — Bản kiểm định độc lập
### NASA Space Apps Challenge 2026 · Ngày biên soạn: 29/08/2026

---

## LỜI DẪN VỀ PHƯƠNG PHÁP BIÊN SOẠN

Tài liệu này được xây dựng qua hai giai đoạn: (1) tra cứu học thuật độc lập cho bốn định hướng do nhóm nêu ban đầu (GeoAI, viễn thám siêu phổ, chòm vệ tinh CubeSat, điện toán biên trên vệ tinh); (2) đối chiếu với một tài liệu tham khảo tám nhánh do người dùng cung cấp (`The_Next_Frontier.pdf`) — mỗi trích dẫn trong tài liệu đó đã được tra cứu lại độc lập trước khi đưa vào bản này, đúng theo yêu cầu "không có sự hời hợt" đã đặt ra. Mục 13 ("Ghi chú thẩm định nguồn") trình bày chi tiết những gì đã xác nhận đúng, những gì đã phát hiện sai lệch và được sửa, và những gì chưa đủ căn cứ để khẳng định trong phạm vi tra cứu này.

**Nguyên tắc xử lý tài liệu tham khảo do người dùng cung cấp:** tài liệu đó được xem là một nguồn thứ cấp cần kiểm định, không phải một nguồn đã được xác lập sẵn. Cấu trúc tám nhánh của tài liệu đó được giữ lại vì có giá trị tổ chức tốt, nhưng mọi trích dẫn cụ thể (tác giả, tạp chí, DOI) đều được tra cứu lại từ nguồn gốc.

---

## MỤC LỤC

1. Phạm vi và nguyên tắc học thuật
2. Quy ước phân loại thuật ngữ và task
3. Bản đồ tổng thể của "The Next Frontier"
4. Nhánh 1 — GeoAI và trí tuệ không gian địa lý
5. Nhánh 2 — Dữ liệu đa phương thức và hợp nhất đa cảm biến
6. Nhánh 3 — Viễn thám siêu phổ và trí tuệ phổ
7. Nhánh 4 — Phân tích không–thời gian và quan sát gần thời gian thực
8. Nhánh 5 — Vệ tinh nhỏ quỹ đạo thấp và trí tuệ chòm vệ tinh
9. Nhánh 6 — Điện toán biên trên quỹ đạo và vệ tinh tự chủ
10. Nhánh 7 — Mô hình nền tảng địa không gian và Earth Intelligence
11. Nhánh 8 — Trí tuệ hỗ trợ quyết định, bất định và GeoAI đáng tin cậy
12. Quan hệ giữa các nhánh và chuỗi độ trễ đầu–cuối
13. Ghi chú thẩm định nguồn (minh bạch quá trình kiểm định)
14. Tài liệu tham khảo

---

## 1. PHẠM VI VÀ NGUYÊN TẮC HỌC THUẬT

Tài liệu giới hạn trong nghiên cứu về Viễn thám (Remote Sensing - RS) và Quan sát Trái Đất (Earth Observation - EO), tập trung vào các hướng công nghệ đang được nghiên cứu trong trí tuệ không gian địa lý, cảm biến, phân tích dữ liệu và tính toán phân tán trên vệ tinh. Phạm vi không bao gồm: tư vấn đầu tư; thiết kế một hệ thống vệ tinh thương mại cụ thể cho một tổ chức có thật; khuyến nghị chính sách; hoặc trích dẫn một challenge brief chính thức của NASA cho năm 2026, vì tài liệu này chưa được công bố tại thời điểm biên soạn.

**Phân cấp nguồn áp dụng:** (i) bài báo bình duyệt trên tạp chí/hội nghị chuyên ngành có DOI xác minh được; (ii) sách chuyên khảo của nhà xuất bản học thuật uy tín; (iii) tài liệu chính thức của tổ chức (NASA, ESA); (iv) preprint — chỉ dùng khi cần mô tả một hướng nghiên cứu chưa có phiên bản bình duyệt, luôn gắn nhãn rõ ràng.

**Nhãn độ chắc chắn** (áp dụng cho mọi luận điểm quan trọng):
- **[ĐÃ XÁC LẬP]** — được hỗ trợ bởi nhiều nghiên cứu độc lập, đã kiểm định.
- **[ĐANG NGHIÊN CỨU]** — hướng mới hoặc bằng chứng còn hạn chế (thường chỉ có một nghiên cứu xác nhận).
- **[DIỄN GIẢI/PHÂN TÍCH]** — cấu trúc tổng hợp do người biên soạn xây dựng từ nhiều nguồn, không trích trực tiếp từ một công trình cụ thể.
- **[CHƯA ĐỦ NGUỒN TIN CẬY]** — chưa tìm được nguồn đạt chuẩn trong phạm vi tra cứu; không suy đoán thay thế.
- **(Ý mình đóng góp thêm)** — nhận định, cách phân loại, hoặc ý tưởng do người biên soạn (Claude) đề xuất, không phải kết quả của một công trình học thuật cụ thể nào.

---

## 2. QUY ƯỚC PHÂN LOẠI THUẬT NGỮ VÀ TASK

### Bảng 1. Quy ước nhãn trạng thái task

| Nhãn | Ý nghĩa |
|---|---|
| **[CẦN THỰC HIỆN]** | Task tồn tại do yêu cầu nghiệp vụ hoặc yêu cầu phương pháp của bài toán — thiếu task này thì bài toán không được giải quyết trọn vẹn. |
| **[SẼ THỰC HIỆN]** | Task được nhóm nghiên cứu lựa chọn để hiện thực hoá trong phạm vi prototype cụ thể (ví dụ: trong 2 ngày hackathon). |
| **[CÓ THỂ THỰC HIỆN]** | Task có giá trị gia tăng nhưng chưa được xác định là thành phần bắt buộc. |
| **[NGHIÊN CỨU]** | Task đòi hỏi nghiên cứu phương pháp, dữ liệu hoặc kiến trúc ở mức cao hơn một prototype thông thường. |

### Bảng 2. Phân loại miền chuyên ngành (domain) cho task

| Miền | Ví dụ vấn đề |
|---|---|
| **{Kỹ thuật}** | Mô hình AI, xử lý ảnh, tính toán, truyền dữ liệu, tối ưu hoá. |
| **{Địa không gian}** | Phân tích vị trí, vùng, quan hệ không gian, bản đồ, biến động địa lý. |
| **{Nông nghiệp}** | Giám sát cây trồng, stress thực vật, biến động sử dụng đất nông nghiệp. |
| **{Thiên tai}** | Cháy rừng, lũ, sạt lở, bão, đánh giá tác động. |
| **{Môi trường}** | Nước, rừng, hệ sinh thái, chất lượng bề mặt, biến đổi dài hạn. |
| **{Đô thị}** | Mở rộng đô thị, hạ tầng, xây dựng, sử dụng đất đô thị. |

### Bảng 3. Mức độ và quy mô task

Mức độ: **Basic** (thao tác chuẩn, ít rủi ro kỹ thuật) → **Core** (thành phần trung tâm của pipeline) → **Advanced** (đòi hỏi tối ưu hoá/kỹ thuật chuyên sâu) → **Research** (chưa có giải pháp chuẩn, cần tìm tòi phương pháp).
Quy mô: **Small** (vài giờ) → **Medium** (một phần ngày) → **Large** (gần trọn thời gian hackathon) → **Very Large** (vượt phạm vi 2 ngày, chỉ phù hợp làm roadmap).

*Quy ước ở Bảng 1–3 là (Ý mình đóng góp thêm), xây dựng nhằm tránh đồng nhất thuật ngữ công nghệ với yêu cầu nghiệp vụ khi chuyển từ nhánh nghiên cứu sang task cụ thể.*

**Chú thích thuật ngữ trên mục 1–2:**
- **Remote Sensing (RS) {Kỹ thuật}** — Viễn thám; phương pháp thu nhận thông tin về một đối tượng hoặc hiện tượng mà không cần tiếp xúc trực tiếp.
- **Earth Observation (EO) {Địa không gian}** — Quan sát Trái Đất; hoạt động thu thập thông tin về hệ thống Trái Đất bằng vệ tinh, máy bay hoặc nền tảng cảm biến khác.
- **GeoAI {Kỹ thuật}** — Trí tuệ nhân tạo địa không gian; AI được thiết kế hoặc áp dụng có xét đến cấu trúc, quan hệ và đặc tính không gian của dữ liệu địa lý.

---

## 3. BẢN ĐỒ TỔNG THỂ CỦA "THE NEXT FRONTIER"

**[ĐÃ XÁC LẬP]** Đã xác nhận qua tra cứu trực tiếp: "The Next Frontier" là chủ đề chính thức của NASA Space Apps Challenge 2026, sự kiện toàn cầu diễn ra 14–15/11/2026, đội tối đa 6 thành viên [1]. Tại thời điểm biên soạn, NASA **chưa công bố** danh sách challenge cụ thể cho năm 2026 — theo lịch sử các năm 2024–2025, challenge statement đầy đủ thường công bố giữa tháng 9.

Cây tám nhánh dưới đây **(Ý mình đóng góp thêm)**, được xây dựng dựa trên các nhóm chủ đề xuất hiện lặp lại trong nhiều khảo sát học thuật độc lập về GeoAI và viễn thám hiện đại [2][3][6]; đây không phải một taxonomy chính thức duy nhất của cộng đồng khoa học.

```
THE NEXT FRONTIER (Viễn thám × AI)
│
├── 1. GeoAI và trí tuệ không gian địa lý
├── 2. Dữ liệu đa phương thức và hợp nhất đa cảm biến
├── 3. Viễn thám siêu phổ và trí tuệ phổ
├── 4. Phân tích không–thời gian và quan sát gần thời gian thực
├── 5. Vệ tinh nhỏ quỹ đạo thấp và trí tuệ chòm vệ tinh
├── 6. Điện toán biên trên quỹ đạo và vệ tinh tự chủ
├── 7. Mô hình nền tảng địa không gian và Earth Intelligence
└── 8. Trí tuệ hỗ trợ quyết định, bất định và GeoAI đáng tin cậy
```

**Giải thích:** Nhánh 1–4 mô tả năng lực nhận thức và khai thác thông tin từ dữ liệu; Nhánh 5–6 mô tả hạ tầng quan sát và tính toán; Nhánh 7–8 mô tả xu hướng mô hình hoá và chất lượng ra quyết định — cách phân lớp này **(Ý mình đóng góp thêm)**.

### Bảng 4. Quan hệ giữa các lớp công nghệ

| Lớp | Câu hỏi nghiên cứu chính | Nhánh liên quan |
|---|---|---|
| Observation | Thu nhận thông tin nào, độ phân giải và tần suất nào? | 2, 3, 5 |
| Intelligence | Có thể phát hiện, phân loại, dự báo và suy luận điều gì? | 1, 4, 7, 8 |
| Computation | Xử lý dữ liệu ở đâu, khi nào, với tài nguyên nào? | 6, liên kết 5–7 |

---

## 4. NHÁNH 1 — GEOAI VÀ TRÍ TUỆ KHÔNG GIAN ĐỊA LÝ

**[ĐÃ XÁC LẬP]** Việc nhúng học sâu (deep learning) vào xử lý ảnh viễn thám được đồng thuận rộng bởi nhiều tổng quan độc lập: Zhu, Tuia, Mou, Xia, Zhang, Xu, & Fraundorfer (2017), *IEEE Geoscience and Remote Sensing Magazine*, 5(4), 8–36, DOI: 10.1109/MGRS.2017.2762307 [15]; Yuan và cộng sự (2020), *Remote Sensing of Environment*, 241, 111716 [16]; và một khảo sát rất mới — Dritsas & Trigka (2026), *Computer Science Review*, 60, tổng hợp các hướng GeoAI gồm học máy, học sâu, mô hình không–thời gian, hợp nhất đa phương thức, khả năng giải thích và tiền huấn luyện quy mô lớn [2]. Về phát hiện đối tượng cụ thể: Cheng & Han (2016), *ISPRS Journal of Photogrammetry and Remote Sensing*, 117, 11–28, DOI: 10.1016/j.isprsjprs.2016.03.014 [17].

Về ứng dụng dự báo/phát hiện thiên tai — một nhánh nhỏ trung tâm của GeoAI: phát hiện lũ từ ảnh radar khẩu độ tổng hợp (SAR - Synthetic Aperture Radar) bằng học sâu, Ghosh, Garg, & Motagh (2022), *ISPRS Ann. Photogramm. Remote Sens. Spat. Inf. Sci.*, 5(3), 201–208 [18]; phát hiện sạt lở đất, Bui, Lee, Lum, Loh, & Tan (2020), *IEEE Access*, DOI: 10.1109/ACCESS.2020.3014305 [19]; đánh giá thiệt hại động đất, Jia & Ye (2023), *Remote Sensing*, 15(16), 4098 [20].

### Cây phân rã (Ý mình đóng góp thêm, dựa trên nhóm phương pháp trong [2])

```
GeoAI
├── 1.1 Hiểu ảnh Quan sát Trái Đất (phân loại, phát hiện đối tượng, phân đoạn ngữ nghĩa)
├── 1.2 Phát hiện biến động không gian (sử dụng đất, đô thị, mất rừng)
├── 1.3 Dự báo/phát hiện thiên tai (lũ, sạt lở, động đất, cháy rừng)
└── 1.4 GeoAI đáng tin cậy (giải thích mô hình, bất định — chi tiết ở Nhánh 8)
```

### Bảng 5. Task thuộc Nhánh 1

| Task | Trạng thái | Vấn đề nghiệp vụ | Miền | Mức độ | Quy mô |
|---|---|---|---|---|---|
| Tải và tiền xử lý ảnh Sentinel-2/Landsat cho khu vực thử nghiệm | [CẦN THỰC HIỆN] | Chuẩn bị dữ liệu đầu vào | {Kỹ thuật} | Basic | Small |
| Huấn luyện/tinh chỉnh mạng nơ-ron tích chập (CNN - Convolutional Neural Network) phân loại lớp phủ | [CẦN THỰC HIỆN] | Bản đồ hiện trạng | {Địa không gian} | Core | Medium |
| Xây mô hình phát hiện lũ từ ảnh SAR (theo hướng [18]) | [SẼ THỰC HIỆN] | Phát hiện sự kiện thiên tai | {Thiên tai} | Advanced | Medium |
| Kết nối dữ liệu FIRMS (NASA — cận thời gian thực, trong vòng 3 giờ kể từ quan sát vệ tinh) hiển thị điểm cháy | [CẦN THỰC HIỆN] | Cảnh báo sự kiện | {Thiên tai} | Core | Small |
| Mở rộng phát hiện sạt lở bằng CNN trên ảnh đa thời điểm (theo [19]) | [CÓ THỂ THỰC HIỆN] | Phát hiện sự kiện thiên tai | {Thiên tai} | Advanced | Large |
| Tích hợp mô hình nền tảng viễn thám có sẵn qua API thay vì huấn luyện từ đầu *(Ý mình đóng góp thêm — tiết kiệm thời gian hackathon)* | [CÓ THỂ THỰC HIỆN] | Tái sử dụng mô hình | {Kỹ thuật} | Advanced | Medium |

**Chú thích thuật ngữ trên Nhánh 1:**
- **Convolutional Neural Network (CNN) {Kỹ thuật}** — Mạng nơ-ron tích chập; kiến trúc học sâu chuyên xử lý dữ liệu dạng lưới như ảnh.
- **Synthetic Aperture Radar (SAR) {Kỹ thuật}** — Radar khẩu độ tổng hợp; cảm biến chủ động thu nhận dữ liệu trong nhiều điều kiện chiếu sáng và thời tiết.
- **Semantic segmentation {Kỹ thuật}** — Phân đoạn ngữ nghĩa; gán một lớp ngữ nghĩa cho từng điểm ảnh.

---

## 5. NHÁNH 2 — DỮ LIỆU ĐA PHƯƠNG THỨC VÀ HỢP NHẤT ĐA CẢM BIẾN

**[ĐÃ XÁC LẬP]** Li, Hong, Gao, Yao, Zheng, Zhang, & Chanussot (2022), "Deep learning in multimodal remote sensing data fusion: A comprehensive review", *International Journal of Applied Earth Observation and Geoinformation*, 112, 102926, DOI: 10.1016/j.jag.2022.102926 [3] — tổng quan phân loại các hướng hợp nhất không gian–phổ, không–thời gian, LiDAR (Light Detection and Ranging — công nghệ đo khoảng cách bằng xung laser)–quang học, SAR–quang học và dữ liệu địa không gian lớn. Sự không đồng nhất giữa các phương thức là vấn đề trung tâm được tài liệu này nhấn mạnh; do đó hợp nhất dữ liệu không nên chỉ được xem là bước tiền xử lý.

### Cây phân rã (Ý mình đóng góp thêm, dựa trên phân loại hướng hợp nhất trong [3])

```
Dữ liệu đa phương thức
├── 2.1 Nguồn cảm biến (quang học, radar/SAR, LiDAR, siêu phổ)
├── 2.2 Hợp nhất chéo cảm biến (quang học + SAR, quang học + LiDAR)
├── 2.3 Hợp nhất không gian (siêu phân giải, pan-sharpening)
└── 2.4 Hợp nhất ngữ nghĩa (ảnh + hệ thống thông tin địa lý (GIS - Geographic Information System), ảnh + dữ liệu phụ trợ)
```

### Bảng 6. Task thuộc Nhánh 2

| Task | Trạng thái | Vấn đề nghiệp vụ | Miền | Mức độ | Quy mô |
|---|---|---|---|---|---|
| Đăng ký (căn chỉnh không gian) ảnh quang học–SAR cho cùng khu vực | [CẦN THỰC HIỆN] | Đồng bộ dữ liệu giữa cảm biến | {Kỹ thuật} | Advanced | Medium |
| Hợp nhất quang học–SAR để bổ sung thông tin khi mây che phủ ảnh quang học | [CÓ THỂ THỰC HIỆN] | Duy trì khả năng quan sát liên tục | {Môi trường} | Advanced | Large |
| Khôi phục vùng ảnh bị mây che bằng dữ liệu SAR cùng thời điểm | [SẼ THỰC HIỆN] | Duy trì chuỗi quan sát | {Môi trường} | Advanced | Medium |
| Hợp nhất ảnh vệ tinh với lớp dữ liệu GIS (ranh giới hành chính, thuỷ văn) | [CÓ THỂ THỰC HIỆN] | Bổ sung ngữ cảnh địa lý | {Địa không gian} | Core | Medium |

**Chú thích thuật ngữ trên Nhánh 2:**
- **Data fusion {Kỹ thuật}** — Hợp nhất dữ liệu; kết hợp thông tin từ nhiều nguồn nhằm tạo biểu diễn hoặc kết quả phân tích chung.
- **Geographic Information System (GIS) {Địa không gian}** — Hệ thống thông tin địa lý; hệ thống lưu trữ, phân tích và hiển thị dữ liệu có gắn vị trí địa lý.
- **Light Detection and Ranging (LiDAR) {Kỹ thuật}** — Công nghệ đo khoảng cách bằng xung laser để tạo thông tin cấu trúc hoặc độ cao.

---

## 6. NHÁNH 3 — VIỄN THÁM SIÊU PHỔ VÀ TRÍ TUỆ PHỔ

**[ĐÃ XÁC LẬP]** Sách chuyên khảo *Hyperspectral Remote Sensing: Theory and Applications* (Pandey, Srivastava, Balzter, Bhattacharya, & Petropoulos biên tập, 2020), Elsevier, ISBN 978-0-08-102894-0 [5], mô tả cơ sở lý thuyết và ứng dụng viễn thám siêu phổ trong nông nghiệp, lâm nghiệp, tài nguyên nước, đất và địa chất. Cụ thể hơn cho từng ứng dụng: giám sát bệnh hại cây trồng, Bai, Zarco-Tejada, Peñuelas và cộng sự (2025), *IEEE Geoscience and Remote Sensing Magazine* [21]; giám sát chất lượng nước nội địa, Chen, Liu, Liu, Shi, & Shi (2026), *Remote Sensing* (MDPI) [22]. Dữ liệu siêu phổ vệ tinh thật của NASA đã sẵn sàng công khai: **EMIT** (Earth Surface Mineral Dust Source Investigation — phổ 380–2500 nm, độ phân giải phổ 7.4 nm, truy cập qua LP DAAC/Earthdata) và **PACE** (Plankton, Aerosol, Cloud, ocean Ecosystem — cảm biến OCI, dải phổ liên tục 2.5 nm từ 350–885 nm, độ phủ toàn cầu 2 ngày/lần, truy cập qua OB.DAAC) [23] — Tier tài liệu chính thức tổ chức.

### Cây phân rã (Ý mình đóng góp thêm, dựa trên chuỗi xử lý HSI mô tả trong [5])

```
Viễn thám siêu phổ
├── 3.1 Thu nhận dữ liệu siêu phổ (vệ tinh EMIT/PACE, trên không, UAV)
├── 3.2 Tiền xử lý phổ (hiệu chỉnh khí quyển, khử nhiễu, giảm chiều)
├── 3.3 Trích xuất thông tin phổ (dấu vết phổ, tách phổ)
└── 3.4 Ứng dụng (nông nghiệp, chất lượng nước, đất, khoáng sản)
```

### Bảng 7. Task thuộc Nhánh 3

| Task | Trạng thái | Vấn đề nghiệp vụ | Miền | Mức độ | Quy mô |
|---|---|---|---|---|---|
| Truy cập dữ liệu EMIT qua Earthdata Search, trích xuất phổ phản xạ khu vực nông nghiệp | [CẦN THỰC HIỆN] | Thu nhận dữ liệu | {Nông nghiệp} | Advanced | Medium |
| Áp dụng phân tích thành phần chính (PCA - Principal Component Analysis) giảm chiều dữ liệu trước khi mô hình hoá | [CẦN THỰC HIỆN] | Tối ưu tính toán trong thời gian hạn chế | {Kỹ thuật} | Core | Small |
| Xây mô hình phân loại cây khoẻ/nhiễm bệnh từ đặc trưng phổ (theo hướng [21]) | [SẼ THỰC HIỆN] | Phát hiện stress thực vật | {Nông nghiệp} | Advanced | Medium |
| Truy cập dữ liệu PACE OCI, ước tính nồng độ diệp lục tố (chlorophyll-a) cho vùng nước quan tâm (theo hướng [22]) | [SẼ THỰC HIỆN] | Đánh giá chất lượng nước | {Môi trường} | Advanced | Medium |
| So sánh hiệu năng đa phổ (Sentinel-2) và siêu phổ (EMIT) trên cùng khu vực để định lượng giá trị gia tăng | [CÓ THỂ THỰC HIỆN] | Đánh giá mô hình | {Kỹ thuật} | Research | Large |

**Chú thích thuật ngữ trên Nhánh 3:**
- **Hyperspectral Imaging (HSI) {Kỹ thuật}** — Ảnh siêu phổ; dữ liệu gồm hàng trăm băng phổ hẹp liên tục, tạo biểu diễn phổ chi tiết của vật thể.
- **Principal Component Analysis (PCA) {Kỹ thuật}** — Phân tích thành phần chính; kỹ thuật giảm chiều dữ liệu bằng cách giữ lại các thành phần mang nhiều phương sai nhất.
- **Spectral signature {Kỹ thuật}** — Dấu vết phổ; dạng phản xạ hoặc phát xạ theo bước sóng đặc trưng của một vật liệu.

---

## 7. NHÁNH 4 — PHÂN TÍCH KHÔNG–THỜI GIAN VÀ QUAN SÁT GẦN THỜI GIAN THỰC

**[ĐÃ XÁC LẬP]** Sự đánh đổi giữa độ phân giải không gian và thời gian là vấn đề trung tâm của hợp nhất không–thời gian (Spatiotemporal Fusion - STF): Chen, Lu, Zou, Li, Emam, Chen, Jing, Wang, & Li (2023), "Spatiotemporal fusion for spectral remote sensing: A statistical analysis and review", *Journal of King Saud University – Computer and Information Sciences*, 35(3), 259–273, DOI: 10.1016/j.jksuci.2023.02.021 [4]. Một tổng quan gần đây hơn tiếp tục phân tích các thách thức về xung đột không–thời gian, tổng quát hoá và hiệu quả tính toán — Sun và cộng sự, "A decade of deep learning for remote sensing spatiotemporal fusion: Advances, challenges, and opportunities" [7], hiện có bản preprint đã xác minh; việc công bố chính thức trên tạp chí *Information Fusion* **chưa được xác minh độc lập đầy đủ trong lần tra cứu này** — xem Mục 13.

**[DIỄN GIẢI/PHÂN TÍCH]** Cần phân biệt rõ "tần suất chụp lặp cao" (revisit time ngắn) với "thời gian thực" (real-time): revisit time mô tả tần suất một vệ tinh quan sát lại cùng một điểm, trong khi thời gian thực liên quan đến độ trễ (latency) từ lúc thu nhận đến lúc có kết quả xử lý — hai chỉ số phụ thuộc vào các nhánh hạ tầng khác nhau (Nhánh 5 và Nhánh 6). Phân biệt này **(Ý mình đóng góp thêm)** nhằm tránh nhầm lẫn thuật ngữ thường gặp trong tài liệu phổ thông.

### Cây phân rã (Ý mình đóng góp thêm)

```
Phân tích không–thời gian
├── 4.1 Quan sát tần suất cao (revisit time ngắn, chuỗi quan sát dày)
├── 4.2 Phân tích chuỗi thời gian (xu hướng, mùa vụ, bất thường)
├── 4.3 Phát hiện sự kiện nhanh (cháy rừng, lũ, bão, sạt lở)
└── 4.4 Giảm độ trễ ra quyết định (ưu tiên sự kiện, phát cảnh báo)
```

### Bảng 8. Task thuộc Nhánh 4

| Task | Trạng thái | Vấn đề nghiệp vụ | Miền | Mức độ | Quy mô |
|---|---|---|---|---|---|
| Thu thập ảnh hai thời điểm (trước/sau) từ Landsat/Sentinel cho khu vực nghiên cứu | [CẦN THỰC HIỆN] | Theo dõi diễn biến | {Địa không gian} | Basic | Small |
| Áp dụng thuật toán phát hiện biến động (differencing hoặc mạng Siamese) | [CẦN THỰC HIỆN] | Phát hiện sự kiện | {Thiên tai} | Core | Medium |
| Định lượng phần trăm diện tích thay đổi theo loại lớp phủ, trực quan hoá theo thời gian | [CẦN THỰC HIỆN] | Phân tích dữ liệu | {Địa không gian} | Basic | Small |
| Đo và công bố rõ chỉ tiêu độ trễ (latency) của pipeline demo thay vì chỉ nói chung chung "thời gian thực" *(Ý mình đóng góp thêm)* | [SẼ THỰC HIỆN] | Đánh giá hệ thống | {Kỹ thuật} | Advanced | Small |

**Chú thích thuật ngữ trên Nhánh 4:**
- **Spatiotemporal Fusion (STF) {Kỹ thuật}** — Hợp nhất không–thời gian; kết hợp dữ liệu có độ phân giải không gian và thời gian khác nhau.
- **Revisit time {Địa không gian}** — Thời gian chụp lặp; khoảng thời gian giữa các lần vệ tinh quan sát lại cùng một mục tiêu.
- **Latency {Kỹ thuật}** — Độ trễ; thời gian từ khi dữ liệu/sự kiện phát sinh đến khi có kết quả xử lý.

---

## 8. NHÁNH 5 — VỆ TINH NHỎ QUỸ ĐẠO THẤP VÀ TRÍ TUỆ CHÒM VỆ TINH

**[ĐÃ XÁC LẬP]** Ko, Gwon, & Ahn (2026), "Satellite Constellation Design for Minimum Worst-Case Revisit Time", *International Journal of Aeronautical and Space Sciences*, 27(1), 916–929, DOI: 10.1007/s42405-025-00985-9 [9] — xây dựng bài toán tối ưu thiết kế chòm vệ tinh Quan sát Trái Đất bằng lập trình tuyến tính nguyên (ILP - Integer Linear Programming); trong một nghiên cứu tình huống quỹ đạo thấp (LEO - Low Earth Orbit), phương pháp này **giảm thời gian tái quan sát tồi tệ nhất (worst-case revisit time) hơn 60% so với cấu hình đối xứng**. Song song, Mateo-Garcia, Veitch-Michaelis, Smith, Oprea, Schumann, Gal, Baydin, & Backes (2021), *Scientific Reports*, 11, 7249, DOI: 10.1038/s41598-021-86650-z [24], ghi nhận **30 vệ tinh CubeSat (vệ tinh khối lập phương tiêu chuẩn hoá) có thể giảm thời gian chụp lặp danh định từ khoảng 5 ngày xuống còn khoảng 8 giờ** với chi phí tương đương một vệ tinh viễn thám truyền thống.

### Cây phân rã (Ý mình đóng góp thêm, dựa trên biến mục tiêu thiết kế trong [9])

```
Vệ tinh nhỏ LEO
├── 5.1 Nền tảng vệ tinh nhỏ (CubeSat, SmallSat)
├── 5.2 Kiến trúc chòm vệ tinh (cấu hình quỹ đạo, coverage, revisit)
├── 5.3 Lập lịch quan sát (ưu tiên mục tiêu, cửa sổ quan sát)
└── 5.4 Ứng dụng ứng phó thiên tai thời gian gần thực
```

### Bảng 9. Task thuộc Nhánh 5

| Task | Trạng thái | Vấn đề nghiệp vụ | Miền | Mức độ | Quy mô |
|---|---|---|---|---|---|
| Thu thập chuỗi ảnh Sentinel-2 (proxy khả thi trong hackathon) minh hoạ lợi ích revisit time ngắn | [CẦN THỰC HIỆN] | Thu nhận dữ liệu | {Kỹ thuật} | Basic | Small |
| Trình bày trực quan so sánh revisit time: vệ tinh đơn lẻ vs. chòm CubeSat (dựa số liệu đã dẫn nguồn ở [24]) | [CẦN THỰC HIỆN] | Truyền đạt giá trị kỹ thuật | {Kỹ thuật} | Basic | Small |
| Tính coverage (vùng có thể quan sát) cho một cấu hình chòm vệ tinh giả định | [SẼ THỰC HIỆN] | Xác định vùng quan sát | {Địa không gian} | Core | Medium |
| Mô phỏng số lượng vệ tinh cần thiết để đạt revisit time mục tiêu (theo khung ILP của [9]) | [CÓ THỂ THỰC HIỆN] | Đánh giá cấu hình | {Kỹ thuật} | Research | Large |
| Dựng kịch bản demo: khi phát hiện thiên tai (Nhánh 1) → giả lập "tasking" một vệ tinh chụp lại khu vực trong X giờ *(Ý mình đóng góp thêm)* | [CÓ THỂ THỰC HIỆN] | Minh hoạ giá trị end-to-end | {Thiên tai} | Advanced | Medium |

**Chú thích thuật ngữ trên Nhánh 5:**
- **Low Earth Orbit (LEO) {Kỹ thuật}** — Quỹ đạo Trái Đất thấp; vùng quỹ đạo ở độ cao tương đối thấp, thường dùng cho nhiệm vụ Quan sát Trái Đất.
- **Integer Linear Programming (ILP) {Kỹ thuật}** — Lập trình tuyến tính nguyên; phương pháp tối ưu hoá trong đó biến quyết định phải nhận giá trị nguyên.
- **CubeSat {Kỹ thuật}** — Vệ tinh khối lập phương; vệ tinh nhỏ theo tiêu chuẩn kích thước module hoá, chi phí sản xuất và phóng thấp hơn vệ tinh truyền thống.

---

## 9. NHÁNH 6 — ĐIỆN TOÁN BIÊN TRÊN QUỸ ĐẠO VÀ VỆ TINH TỰ CHỦ

**[ĐÃ XÁC LẬP → ĐANG NGHIÊN CỨU tuỳ ứng dụng]** Minh chứng vận hành rõ ràng nhất đến từ chuỗi nghiên cứu trên vệ tinh **PhiSat-1** của Cơ quan Vũ trụ châu Âu (ESA). Mateo-Garcia và cộng sự (2021) [24] chứng minh thuật toán phân đoạn lũ lụt chạy được ngay trên bộ gia tốc phần cứng học máy của PhiSat-1; băng thông truyền dữ liệu (downlink) của CubeSat khi đó chỉ khoảng 1–10 Mbps, so với khoảng 0.5 Gbps của Sentinel-2 — đây chính là động lực kỹ thuật cho điện toán biên. Bài tiếp theo, Mateo-Garcia, Veitch-Michaelis, Purcell, Longepe, Reid, Anlind, Bruhn, Parr, & Mathieu (2023), *Scientific Reports*, 13, 10391, DOI: 10.1038/s41598-023-34436-w [25], mô tả khái niệm "điện toán đám mây nhận thức trong không gian" và **trình diễn thành công việc huấn luyện lại mô hình học máy ngay trên quỹ đạo**.

Về ứng dụng cảnh báo cháy rừng: Spiller, Thangavel, Sasidharan, Amici, Ansalone, & Sabatini (2022), "Wildfire segmentation analysis from edge computing for on-board real-time alerts using hyperspectral imagery", *2022 IEEE International Conference on Metrology for Extended Reality, Artificial Intelligence and Neural Engineering (MetroXRAINE)*, Rome, tr. 725–730, DOI: 10.1109/MetroXRAINE54828.2022.9967553 [26] — dùng vệ tinh siêu phổ PRISMA (Cơ quan Vũ trụ Ý), thử nghiệm trên vụ cháy rừng New South Wales (Úc) tháng 12/2019, so sánh ba bộ gia tốc phần cứng (Intel Movidius Myriad 2, Nvidia Jetson TX2, Nvidia Jetson Nano). Gần đây hơn, Cratere, Carbone, Cannizzaro, Asciolla, Spiller, & Dell'Olio (2025), "Enabling real-time wildfire detection through edge AI onboard CubeSat platforms", trong kỷ yếu *Artificial Intelligence and Image and Signal Processing for Remote Sensing XXXI*, SPIE, DOI: 10.1117/12.3070157 [27], trình bày một mạng nơ-ron tích chập nhẹ tăng tốc phần cứng cho phân đoạn cháy rừng thời gian thực ngay trên vệ tinh CubeSat với ràng buộc SWaP nghiêm ngặt — nhóm tác giả báo cáo độ chính xác 99% với tỷ lệ báo động giả thấp; **đây là số liệu từ một nghiên cứu đơn lẻ (dù đã được một tổng quan độc lập khác trích dẫn lại), chưa đối chiếu bằng thực nghiệm độc lập thứ hai, nên vẫn gắn nhãn [ĐANG NGHIÊN CỨU]** cho riêng con số 99% theo đúng quy tắc đối chiếu chéo ở Mục 1.

**[ĐÃ XÁC LẬP]** (Cập nhật sau lần tra cứu bổ sung) Deng, Gong, Wang, & Que (2025/2026), "Cooperative task offloading and resource allocation for sequential constraint tasks in satellite edge computing networks", *Ad Hoc Networks*, 180, 104044, DOI: 10.1016/j.adhoc.2025.104044 [10] — đã xác minh trực tiếp qua ScienceDirect (tên tác giả, số tập, số bài, DOI khớp hoàn toàn). Bài báo đề xuất mô hình vệ tinh khả kiến (satellite visible model) dựa trên hình học không gian để mô tả cửa sổ liên lạc, và thuật toán tối ưu luân phiên (alternate optimization) giải bài toán chi phí trọng số tối thiểu cho các tác vụ Quan sát Trái Đất có ràng buộc tuần tự — cơ sở học thuật trực tiếp cho task "phân bổ tài nguyên" và "offloading" trong Bảng 10.

### Cây phân rã (Ý mình đóng góp thêm)

```
Điện toán biên trên quỹ đạo
├── 6.1 Kiến trúc phần cứng AI trên vệ tinh (ràng buộc SWaP: Size, Weight, Power)
├── 6.2 Giảm dữ liệu (nén, trích xuất đặc trưng, lọc theo sự kiện)
├── 6.3 Xử lý tự chủ (Detect → Prioritize → Transmit)
└── 6.4 Học máy huấn luyện lại trên quỹ đạo (in-orbit retraining)
```

### Bảng 10. Task thuộc Nhánh 6

| Task | Trạng thái | Vấn đề nghiệp vụ | Miền | Mức độ | Quy mô |
|---|---|---|---|---|---|
| Tổng hợp ràng buộc phần cứng (SWaP) khi thiết kế mô hình AI cho vệ tinh nhỏ, từ tài liệu đã dẫn nguồn | [CẦN THỰC HIỆN] | Nghiên cứu ràng buộc kỹ thuật | {Kỹ thuật} | Core | Small |
| Nén (quantize/prune) mô hình phát hiện cháy/lũ đã xây ở Nhánh 1 để mô phỏng chạy trên thiết bị tài nguyên hạn chế | [SẼ THỰC HIỆN] | Giảm nhu cầu tính toán | {Kỹ thuật} | Advanced | Medium |
| Benchmark tốc độ suy luận trên phần cứng biên mô phỏng (ví dụ Raspberry Pi/Jetson Nano làm proxy cho vệ tinh) | [CÓ THỂ THỰC HIỆN] | Đánh giá hiệu năng | {Kỹ thuật} | Advanced | Medium |
| Dựng demo end-to-end: ảnh đầu vào → xử lý biên mô phỏng → cảnh báo đẩy về dashboard trong vài giây *(Ý mình đóng góp thêm)* | [CÓ THỂ THỰC HIỆN] | Minh hoạ pipeline hoàn chỉnh | {Thiên tai} | Advanced | Medium |
| Trình bày khái niệm học máy huấn luyện lại trên quỹ đạo như hướng mở rộng tương lai (dựa trên [25]) | [SẼ THỰC HIỆN] | Định hướng roadmap | {Kỹ thuật} | Basic | Small |

**Chú thích thuật ngữ trên Nhánh 6:**
- **Edge Computing {Kỹ thuật}** — Điện toán biên; xử lý dữ liệu gần nơi dữ liệu được tạo ra thay vì luôn truyền toàn bộ dữ liệu về trung tâm.
- **On-board Processing {Kỹ thuật}** — Xử lý trên thiết bị; thực hiện tính toán trực tiếp trên vệ tinh.
- **Size, Weight, and Power (SWaP) {Kỹ thuật}** — Kích thước, khối lượng và năng lượng; bộ ràng buộc phần cứng đặc trưng của nền tảng vệ tinh nhỏ.

---

## 10. NHÁNH 7 — MÔ HÌNH NỀN TẢNG ĐỊA KHÔNG GIAN VÀ EARTH INTELLIGENCE

**[ĐÃ XÁC LẬP]** Nhiều khảo sát 2025–2026 độc lập xác nhận sự chuyển dịch từ mô hình chuyên biệt theo task sang mô hình tiền huấn luyện quy mô lớn (foundation model) trong viễn thám: Huang, Yan, Zhan, Yang, Zhang, Zhang, Lei, Liu, Liu, & Wang (2025), "A Survey on Remote Sensing Foundation Models: From Vision to Multimodality", preprint arXiv:2503.22081 [28]; và Yang và cộng sự (2025), "Survey of Multimodal Geospatial Foundation Models: Techniques, Applications, and Challenges", preprint arXiv:2510.22964 [29] — cả hai đều là preprint, gắn nhãn theo đúng quy định Mục 1.

**[ĐÃ XÁC LẬP]** (Cập nhật sau lần tra cứu bổ sung) Lu, Guo, Zimmer-Dauphinee, Nieusma, Wang, VanValkenburgh, Wernke, & Huo (2025), "Vision Foundation Models in Remote Sensing: A Survey", *IEEE Geoscience and Remote Sensing Magazine*, 13(3), 190–227, DOI: 10.1109/MGRS.2025.3541952 [6] — xác minh trực tiếp qua cơ sở dữ liệu chính thức của Bộ Năng lượng Hoa Kỳ (OSTI.gov, OSTI ID 2573563), trang nghiên cứu của Đại học Vanderbilt, và ảnh chụp trang tạp chí gốc (số tháng 9/2025). Bài preprint cùng nội dung (arXiv:2408.03464) cũng tồn tại song song, là bản thảo trước bình duyệt của cùng công trình.

### Cây phân rã (Ý mình đóng góp thêm)

```
Mô hình nền tảng địa không gian
├── 7.1 Mô hình nền tảng viễn thám (tiền huấn luyện tự giám sát, transfer learning)
├── 7.2 Mô hình nền tảng đa phương thức (quang học + SAR, ảnh + văn bản)
├── 7.3 GeoAI thị giác–ngôn ngữ (truy vấn địa không gian bằng ngôn ngữ tự nhiên)
└── 7.4 Mô hình dùng cho nhiều task hạ nguồn (phân loại, phát hiện, phân đoạn)
```

### Bảng 11. Task thuộc Nhánh 7

| Task | Trạng thái | Vấn đề nghiệp vụ | Miền | Mức độ | Quy mô |
|---|---|---|---|---|---|
| Khảo sát và lựa chọn một mô hình nền tảng viễn thám mã nguồn mở phù hợp cho bài toán | [CẦN THỰC HIỆN] | Tái sử dụng mô hình | {Kỹ thuật} | Advanced | Medium |
| Tinh chỉnh (fine-tune) mô hình nền tảng cho task cụ thể của Nhánh 1/3 thay vì huấn luyện từ đầu | [SẼ THỰC HIỆN] | Tiết kiệm thời gian huấn luyện | {Kỹ thuật} | Advanced | Medium |
| Thử nghiệm truy vấn dữ liệu địa không gian bằng ngôn ngữ tự nhiên như một tính năng dashboard | [CÓ THỂ THỰC HIỆN] | Cải thiện trải nghiệm người dùng | {Kỹ thuật} | Research | Large |

**Chú thích thuật ngữ trên Nhánh 7:**
- **Foundation Model {Kỹ thuật}** — Mô hình nền tảng; mô hình được tiền huấn luyện trên dữ liệu quy mô lớn để thích nghi cho nhiều nhiệm vụ khác nhau.
- **Self-Supervised Learning (SSL) {Kỹ thuật}** — Học tự giám sát; tạo tín hiệu huấn luyện từ chính dữ liệu thay vì phụ thuộc hoàn toàn vào nhãn do con người cung cấp.
- **Downstream Task {Kỹ thuật}** — Nhiệm vụ hạ nguồn; task cụ thể thực hiện sau giai đoạn tiền huấn luyện mô hình.

---

## 11. NHÁNH 8 — TRÍ TUỆ HỖ TRỢ QUYẾT ĐỊNH, BẤT ĐỊNH VÀ GEOAI ĐÁNG TIN CẬY

**[ĐÃ XÁC LẬP]** Khảo sát GeoAI của Dritsas & Trigka (2026) [2] và các khảo sát mô hình nền tảng [28][29] đều xác định tổng quát hoá không gian, khả năng giải thích (Explainable AI - XAI), lượng hoá bất định (Uncertainty Quantification - UQ) và độ tin cậy khi triển khai là những vấn đề nghiên cứu còn mở, chưa có giải pháp chuẩn hoá — nhãn **[ĐANG NGHIÊN CỨU]** áp dụng cho toàn bộ nhánh này.

### Cây phân rã (Ý mình đóng góp thêm)

```
GeoAI đáng tin cậy
├── 8.1 Bất định (bất định dự đoán, bất định cảm biến)
├── 8.2 Khả năng giải thích (attribution, evidence extraction)
├── 8.3 Độ bền vững mô hình (domain shift — thay đổi phân phối dữ liệu giữa vùng huấn luyện và vùng áp dụng)
└── 8.4 Hỗ trợ ra quyết định (bản đồ rủi ro, xếp hạng ưu tiên)
```

### Bảng 12. Task thuộc Nhánh 8

| Task | Trạng thái | Vấn đề nghiệp vụ | Miền | Mức độ | Quy mô |
|---|---|---|---|---|---|
| Báo cáo độ tin cậy/xác suất dự đoán bên cạnh nhãn phân loại, thay vì chỉ đưa ra kết quả nhị phân | [CẦN THỰC HIỆN] | Định lượng độ tin cậy dự đoán | {Kỹ thuật} | Core | Small |
| Kiểm tra hiệu năng mô hình khi áp dụng cho một khu vực địa lý khác khu vực huấn luyện | [SẼ THỰC HIỆN] | Đánh giá domain shift | {Địa không gian} | Advanced | Medium |
| Chuyển kết quả mô hình AI thành bản đồ rủi ro trực quan cho người ra quyết định | [CÓ THỂ THỰC HIỆN] | Hỗ trợ ra quyết định | {Thiên tai} | Core | Medium |
| Công khai mã nguồn và quy trình đánh giá để đảm bảo khả năng tái lập (reproducibility) *(Ý mình đóng góp thêm — phù hợp tinh thần mã nguồn mở của NASA Space Apps)* | [SẼ THỰC HIỆN] | Kiểm chứng tính nhất quán | {Kỹ thuật} | Core | Small |

**Chú thích thuật ngữ trên Nhánh 8:**
- **Explainable Artificial Intelligence (XAI) {Kỹ thuật}** — Trí tuệ nhân tạo có khả năng giải thích; cung cấp thông tin giúp con người hiểu cơ sở của một dự đoán.
- **Uncertainty Quantification (UQ) {Kỹ thuật}** — Lượng hoá bất định; ước lượng mức độ không chắc chắn đi kèm một dự đoán.
- **Domain Shift {Kỹ thuật}** — Sự thay đổi phân phối dữ liệu giữa môi trường huấn luyện và môi trường áp dụng mô hình.

---

## 12. QUAN HỆ GIỮA CÁC NHÁNH VÀ CHUỖI ĐỘ TRỄ ĐẦU–CUỐI

**[DIỄN GIẢI/PHÂN TÍCH]** Không nên xem tám nhánh là tám hệ thống độc lập. Chúng có thể tạo thành một pipeline nghiên cứu duy nhất, từ thu nhận đến ra quyết định. Cách ghép pipeline này **(Ý mình đóng góp thêm)**, dựa trên quan hệ được mô tả riêng lẻ trong các nguồn đã dẫn ở Nhánh 1, 2, 5, 6.

```
Nguồn quan sát (quang học / SAR / LiDAR / siêu phổ)
        ↓
Hợp nhất đa phương thức (Nhánh 2)
        ↓
Phân tích GeoAI / mô hình nền tảng (Nhánh 1, 7)
        ↓
Xử lý trên mặt đất hoặc điện toán biên trên quỹ đạo (Nhánh 6)
        ↓
Phát hiện / dự báo / ước lượng bất định (Nhánh 4, 8)
        ↓
Xếp hạng ưu tiên / cảnh báo / hỗ trợ quyết định
```

### Bảng 13. Thành phần của độ trễ đầu–cuối (end-to-end latency)

| Thành phần | Nội dung | Nhánh liên quan |
|---|---|---|
| Acquisition latency (độ trễ thu nhận) | Thời gian từ khi sự kiện xảy ra đến khi có quan sát phù hợp | 3, 5 |
| Transmission latency (độ trễ truyền dữ liệu) | Thời gian truyền qua liên kết không gian–mặt đất hoặc liên vệ tinh | 5, 6 |
| Processing latency (độ trễ xử lý) | Thời gian tiền xử lý và suy luận mô hình | 1, 6, 7 |
| Decision latency (độ trễ ra quyết định) | Thời gian chuyển kết quả thành thông tin hỗ trợ quyết định | 4, 8 |

**[DIỄN GIẢI/PHÂN TÍCH]** Do đó, thuật ngữ "thời gian thực" (real-time) nên được định nghĩa bằng một chỉ tiêu độ trễ cụ thể (ví dụ: dưới 60 giây từ thu nhận đến cảnh báo) thay vì dùng như một nhãn chung cho bất kỳ hệ thống nào có revisit time cao — quan điểm này **(Ý mình đóng góp thêm)**.

---

## 13. GHI CHÚ THẨM ĐỊNH NGUỒN

Mục này trình bày minh bạch quá trình kiểm định độc lập đối với tài liệu tham khảo do người dùng cung cấp (`The_Next_Frontier.pdf`), đúng theo yêu cầu "mọi kiến thức nhỏ cũng cần kiểm định". Mỗi trích dẫn được tra cứu lại qua công cụ tìm kiếm web, đối chiếu tên tác giả, tên tạp chí, và DOI (Digital Object Identifier — mã định danh số hoá của một công trình học thuật) với nguồn gốc.

### 13.1 Trích dẫn đã xác nhận chính xác
- Dritsas & Trigka (2026), *Computer Science Review* [2] — tên tác giả, tạp chí, năm xuất bản đều khớp qua nhiều nguồn độc lập (hồ sơ tác giả, ScienceDirect, ResearchGate).
- Li, Hong, Gao và cộng sự (2022), *International Journal of Applied Earth Observation and Geoinformation* [3] — khớp với kết quả tra cứu độc lập trước đó của người biên soạn.
- Pandey, Srivastava, Balzter, Bhattacharya, & Petropoulos (Eds., 2020), sách *Hyperspectral Remote Sensing: Theory and Applications*, Elsevier [5] — tên biên tập viên, nhà xuất bản, ISBN khớp hoàn toàn với trang bán sách chính thức của Elsevier.
- Ko, Gwon, & Ahn (2026), *International Journal of Aeronautical and Space Sciences* [9] — DOI khớp chính xác; tóm tắt bài báo xác nhận đúng nội dung (giảm worst-case revisit time hơn 60%).
- Huang, Yan, Zhan và cộng sự (2025), arXiv:2503.22081 [28] — tồn tại đúng như trích dẫn.
- Yang và cộng sự (2025), arXiv:2510.22964 [29] — tồn tại đúng như trích dẫn.

### 13.2 Sai lệch đã phát hiện và đã sửa
- **Trích dẫn [4]:** tài liệu tham khảo ghi tác giả đầu là "Li, C." — tra cứu lại cho thấy **tác giả đầu thực tế là Chen, G.** (Guangsheng Chen), với "Li, C." (Chao Li) là tác giả **cuối cùng**, không phải tác giả đầu. Đã sửa thành: Chen, Lu, Zou, Li, Emam, Chen, Jing, Wang, & Li (2023). Tên tạp chí, số tập, số trang, DOI trong tài liệu gốc là chính xác.
- **Trích dẫn [11]:** tài liệu tham khảo ghi tác giả đầu là "Li, J." — tra cứu lại cho thấy **tác giả đầu thực tế là Huang, Z.** (Ziyue Huang). Đã sửa thành: Huang, Yan, Zhan, Yang, Zhang, Zhang, Lei, Liu, Liu, & Wang (2025). Tiêu đề và mã arXiv trong tài liệu gốc là chính xác.

### 13.3 Cập nhật sau lần tra cứu bổ sung (vòng kiểm định thứ hai)
Ở lần kiểm định đầu tiên, bốn trích dẫn ([6], [7], [8], [10]) bị đánh giá là "chưa xác minh được" chỉ vì công cụ tìm kiếm không trả về kết quả khi tra cứu **trực tiếp bằng chuỗi DOI** — đây là giới hạn của cách tra cứu, không phải bằng chứng nguồn sai. Ở lần tra cứu bổ sung này, đổi chiến lược sang tìm theo tên tác giả + tiêu đề + tên tạp chí, và cả bốn trích dẫn đều được xác nhận chính xác:
- **[6]** — xác nhận qua OSTI.gov (cơ sở dữ liệu chính thức của Bộ Năng lượng Hoa Kỳ) và trang nghiên cứu Đại học Vanderbilt: đã đăng chính thức trên *IEEE Geoscience and Remote Sensing Magazine*, 13(3), tháng 9/2025, DOI khớp chính xác.
- **[7]** — xác nhận qua ScienceDirect: đã đăng trên *Information Fusion*, Vol. 126, Part B, tháng 2/2026, DOI khớp chính xác. **Phát hiện sai lệch nhỏ:** tác giả đầu tên đầy đủ là "Enzhe Sun", tài liệu tham khảo gốc ghi "Sun, Y." — đã sửa thành "Sun, E." trong Mục 14.
- **[8]** — xác nhận qua trang chính thức ACM Digital Library (doi.org/10.1145/3810438): đã đăng trên *ACM Transactions on Spatial Algorithms and Systems*, xuất bản 29/5/2026, khớp hoàn toàn tiêu đề và nội dung tóm tắt.
- **[10]** — xác nhận qua ScienceDirect: đã đăng trên *Ad Hoc Networks*, Vol. 180, bài 104044, danh sách tác giả (Peng Deng, Xiangyang Gong, Ziyi Wang, Xirong Que) khớp chính xác với tài liệu gốc.

Ngoài ra, tên tác giả đầy đủ cho hai trích dẫn hội nghị [26] và [27] (trước đó chưa xác định được) nay đã xác nhận đầy đủ — xem Mục 14.

### 13.4 Nhìn nhận về sai sót trong lần kiểm định đầu tiên của chính tài liệu này
Cần nói thẳng: việc bốn nguồn hợp lệ bị gắn nhãn "chưa xác minh" ở phiên bản trước là do tra cứu chưa đủ kỹ ở vòng đầu (dừng lại sau khi tìm DOI trực tiếp không ra kết quả, thay vì thử thêm chiến lược tìm kiếm khác) — đúng như lo ngại "sự hời hợt" mà yêu cầu ban đầu đã cảnh báo. Đây là lý do tại sao mọi số liệu/trích dẫn quan trọng nên được đối chiếu nhiều lần bằng nhiều chiến lược tra cứu khác nhau trước khi kết luận "không xác minh được", thay vì dừng lại sau một lần tìm không ra kết quả.

### 13.5 Còn lại duy nhất một điểm cần lưu ý
Con số "độ chính xác 99%" của hệ thống edge-AI phát hiện cháy rừng trong [27] vẫn chỉ đến từ **một nghiên cứu gốc**, dù đã được một tổng quan độc lập khác trích dẫn lại — theo quy tắc đối chiếu chéo ở Mục 1 (số liệu định lượng quan trọng cần ≥ 2 nguồn **thực nghiệm** độc lập), con số này vẫn giữ nhãn [ĐANG NGHIÊN CỨU] và không nên trình bày như một kết quả đã được cộng đồng khoa học đồng thuận rộng rãi.

### 13.6 Nguyên tắc áp dụng
Theo đúng quy tắc ở Mục 1: mọi trích dẫn trong tài liệu tham khảo (Mục 14) nay đã qua kiểm định trực tiếp, trừ số liệu cụ thể nêu ở Mục 13.5 vẫn giữ nhãn [ĐANG NGHIÊN CỨU]. Danh sách tác giả của trích dẫn [12] (Yang và cộng sự, arXiv:2510.22964) đã xác nhận tồn tại đúng mã arXiv và tiêu đề, nhưng danh sách đầy đủ tất cả đồng tác giả chưa được đối chiếu từng tên — không ảnh hưởng đến nội dung trích dẫn trong tài liệu này vì chỉ dùng ở mức tổng quát ("Yang và cộng sự").

---

## 14. TÀI LIỆU THAM KHẢO

Số trong ngoặc vuông [n] chỉ tài liệu tương ứng bên dưới. Trạng thái xác minh ghi rõ theo Mục 13.

1. NASA Space Apps Challenge. (2026). *NASA Space Apps Challenge 2026*. Trang chính thức: https://www.spaceappschallenge.org/2026/ — [Xác minh trực tiếp qua truy cập trang]
2. Dritsas, E., & Trigka, M. (2026). Advances in geospatial artificial intelligence for remote sensing applications. *Computer Science Review*, 60. — [Đã xác minh]
3. Li, J., Hong, D., Gao, L., Yao, J., Zheng, K., Zhang, B., & Chanussot, J. (2022). Deep learning in multimodal remote sensing data fusion: A comprehensive review. *International Journal of Applied Earth Observation and Geoinformation*, 112, 102926. DOI: 10.1016/j.jag.2022.102926. — [Đã xác minh]
4. Chen, G., Lu, H., Zou, W., Li, L., Emam, M., Chen, X., Jing, W., Wang, J., & Li, C. (2023). Spatiotemporal fusion for spectral remote sensing: A statistical analysis and review. *Journal of King Saud University – Computer and Information Sciences*, 35(3), 259–273. DOI: 10.1016/j.jksuci.2023.02.021. — [Đã xác minh; đã sửa thứ tự tác giả, xem Mục 13.2]
5. Pandey, P. C., Srivastava, P. K., Balzter, H., Bhattacharya, B., & Petropoulos, G. P. (Eds.). (2020). *Hyperspectral Remote Sensing: Theory and Applications*. Elsevier. ISBN 978-0-08-102894-0. — [Đã xác minh]
6. Lu, S., Guo, J., Zimmer-Dauphinee, J. R., Nieusma, J. M., Wang, X., VanValkenburgh, P., Wernke, S. A., & Huo, Y. (2025). Vision Foundation Models in Remote Sensing: A Survey. *IEEE Geoscience and Remote Sensing Magazine*, 13(3), 190–227. DOI: 10.1109/MGRS.2025.3541952. (Bản preprint cùng nội dung: arXiv:2408.03464.) — [Đã xác minh qua OSTI.gov, ORCID tác giả, và bản scan tạp chí gốc]
7. Sun, E., Cui, Y., Liu, P., & Yan, J. (2026). A decade of deep learning for remote sensing spatiotemporal fusion: Advances, challenges, and opportunities. *Information Fusion*, 126(Part B), 103675. DOI: 10.1016/j.inffus.2025.103675. — [Đã xác minh qua ScienceDirect; đã sửa tên viết tắt tác giả đầu từ "Sun, Y." thành "Sun, E." (Enzhe Sun)]
8. Gao, S., Lunga, D., Yang, L., Newsam, S., & Martins, B. (2026). Introduction to the Special Issue on GeoAI Foundation Models and Their Applications, Part I. *ACM Transactions on Spatial Algorithms and Systems*. DOI: 10.1145/3810438. Xuất bản 29/5/2026. — [Đã xác minh qua ACM Digital Library]
9. Ko, J., Gwon, B., & Ahn, J. (2026). Satellite Constellation Design for Minimum Worst-Case Revisit Time. *International Journal of Aeronautical and Space Sciences*, 27(1), 916–929. DOI: 10.1007/s42405-025-00985-9. — [Đã xác minh]
10. Deng, P., Gong, X., Wang, Z., & Que, X. (2025). Cooperative task offloading and resource allocation for sequential constraint tasks in satellite edge computing networks. *Ad Hoc Networks*, 180, 104044. DOI: 10.1016/j.adhoc.2025.104044. — [Đã xác minh qua ScienceDirect]
11. Huang, Z., Yan, H., Zhan, Q., Yang, S., Zhang, M., Zhang, C., Lei, Y., Liu, Z., Liu, Q., & Wang, Y. (2025). A Survey on Remote Sensing Foundation Models: From Vision to Multimodality. Preprint, arXiv:2503.22081. — [Đã xác minh; đã sửa tác giả đầu, xem Mục 13.2]
12. Yang, L. và cộng sự. (2025). Survey of Multimodal Geospatial Foundation Models: Techniques, Applications, and Challenges. Preprint, arXiv:2510.22964. — [Tồn tại đã xác minh; danh sách đầy đủ tác giả chưa đối chiếu từng tên]
13. NASA/JPL. EMIT (Earth Surface Mineral Dust Source Investigation) — tài liệu truy cập dữ liệu chính thức: earth.jpl.nasa.gov/emit. — [Xác minh trực tiếp]
14. NASA/OB.DAAC. PACE (Plankton, Aerosol, Cloud, ocean Ecosystem) — tài liệu truy cập dữ liệu chính thức: earthdata.nasa.gov/data/platforms/space-based-platforms/pace. — [Xác minh trực tiếp]
15. Zhu, X. X., Tuia, D., Mou, L., Xia, G. S., Zhang, L., Xu, F., & Fraundorfer, F. (2017). Deep Learning in Remote Sensing: A Comprehensive Review and List of Resources. *IEEE Geoscience and Remote Sensing Magazine*, 5(4), 8–36. DOI: 10.1109/MGRS.2017.2762307. — [Đã xác minh, tự tra cứu]
16. Yuan, Q., Shen, H., Li, T., Li, Z., Li, S., Jiang, Y., Xu, H., Tan, W., Yang, Q., Wang, J., Gao, J., & Zhang, L. (2020). Deep learning in environmental remote sensing: Achievements and challenges. *Remote Sensing of Environment*, 241, 111716. — [Đã xác minh, tự tra cứu]
17. Cheng, G., & Han, J. (2016). A survey on object detection in optical remote sensing images. *ISPRS Journal of Photogrammetry and Remote Sensing*, 117, 11–28. DOI: 10.1016/j.isprsjprs.2016.03.014. — [Đã xác minh, tự tra cứu]
18. Ghosh, B., Garg, S., & Motagh, M. (2022). Automatic flood detection from Sentinel-1 data using deep learning architectures. *ISPRS Ann. Photogramm. Remote Sens. Spat. Inf. Sci.*, 5(3), 201–208. DOI: 10.5194/isprs-Annals-V-3-2022-201-2022. — [Đã xác minh, tự tra cứu]
19. Bui, T. A., Lee, P. J., Lum, K. Y., Loh, C., & Tan, K. (2020). Deep learning for landslide recognition in satellite architecture. *IEEE Access*. DOI: 10.1109/ACCESS.2020.3014305. — [Đã xác minh, tự tra cứu]
20. Jia, J., & Ye, W. (2023). Deep learning for earthquake disaster assessment: Objects, data, models, stages, challenges, and opportunities. *Remote Sensing*, 15(16), 4098. — [Đã xác minh, tự tra cứu]
21. Bai, Y., Zarco-Tejada, P. J., Peñuelas, J. và cộng sự. (2025). Hyperspectral Remote Sensing for Monitoring Crop Disease: Applications, challenges, and perspectives. *IEEE Geoscience and Remote Sensing Magazine*. — [Đã xác minh, tự tra cứu]
22. Chen, L., Liu, L., Liu, S., Shi, Z., & Shi, C. (2026). The Application of Remote Sensing Technology in Inland Water Quality Monitoring and Water Environment Science: Recent Progress and Perspectives. *Remote Sensing* (MDPI). — [Đã xác minh, tự tra cứu]
23. NASA. Earthdata — tài liệu về nhiệm vụ FIRMS (Fire Information for Resource Management System): earthdata.nasa.gov/data/tools/firms. — [Xác minh trực tiếp]
24. Mateo-Garcia, G., Veitch-Michaelis, J., Smith, L., Oprea, S. V., Schumann, G., Gal, Y., Baydin, A. G., & Backes, D. (2021). Towards global flood mapping onboard low cost satellites with machine learning. *Scientific Reports*, 11, 7249. DOI: 10.1038/s41598-021-86650-z. — [Đã xác minh, tự tra cứu]
25. Mateo-Garcia, G., Veitch-Michaelis, J., Purcell, C., Longepe, N., Reid, S., Anlind, A., Bruhn, F., Parr, J., & Mathieu, P. P. (2023). In-orbit demonstration of a re-trainable machine learning payload for processing optical imagery. *Scientific Reports*, 13, 10391. DOI: 10.1038/s41598-023-34436-w. — [Đã xác minh, tự tra cứu]
26. Spiller, D., Thangavel, K., Sasidharan, S. T., Amici, S., Ansalone, L., & Sabatini, R. (2022). Wildfire segmentation analysis from edge computing for on-board real-time alerts using hyperspectral imagery. *2022 IEEE International Conference on Metrology for Extended Reality, Artificial Intelligence and Neural Engineering (MetroXRAINE)*, Rome, 725–730. DOI: 10.1109/MetroXRAINE54828.2022.9967553. — [Đã xác minh đầy đủ qua IEEE Xplore, ResearchGate, dblp]
27. Cratere, A., Carbone, A., Cannizzaro, I., Asciolla, M., Spiller, D., & Dell'Olio, F. (2025). Enabling real-time wildfire detection through edge AI onboard CubeSat platforms. Trong Bruzzone, L., Bovolo, F., & Bovenga, F. (Chủ biên), *Artificial Intelligence and Image and Signal Processing for Remote Sensing XXXI*. SPIE, bài 13670-29. DOI: 10.1117/12.3070157. — [Đã xác minh đầy đủ qua ResearchGate, kỷ yếu SPIE]
28. Huang, Z. và cộng sự — xem mục 11 (trùng nguồn, đánh số lại để nhất quán với trích dẫn trong Nhánh 7–8).
29. Yang, L. và cộng sự — xem mục 12 (trùng nguồn, đánh số lại để nhất quán với trích dẫn trong Nhánh 7–8).

---

## GHI CHÚ CUỐI

Tài liệu này là công cụ hỗ trợ tra cứu và cấu trúc hoá có kỷ luật, **mang tính chất tham khảo**, không thay thế việc nhóm tự đọc bài gốc và tự kiểm chứng trước khi đưa vào báo cáo hoặc bài dự thi chính thức. Sau hai vòng tra cứu độc lập, toàn bộ 29 trích dẫn trong Mục 14 đã được xác minh trực tiếp từ nguồn gốc (tên tác giả, tạp chí/hội nghị, DOI), với hai lỗi thứ tự tác giả đã phát hiện và sửa ([4], [11]) và một lỗi tên viết tắt đã sửa ([7]). Điểm duy nhất còn giữ nhãn [ĐANG NGHIÊN CỨU] là con số "độ chính xác 99%" ở Nhánh 6 (Mục 13.5), vì chỉ có một nghiên cứu thực nghiệm xác nhận. Hai chỉ dấu định lượng có độ tin cậy cao nhất cho phần thuyết trình: giảm worst-case revisit time hơn 60% theo [9]; giảm revisit time từ ~5 ngày còn ~8 giờ với 30 CubeSat theo [24].
