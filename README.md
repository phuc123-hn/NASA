# README — Research Exploration: Earth Observation, AI & Environmental Science

> **Trạng thái dự án: OPEN DISCUSSION — CHƯA CHỐT ĐỀ TÀI**
>
> Tài liệu này được xây dựng nhằm giúp các thành viên hiểu bối cảnh, chuẩn bị kiến thức, xác định những vấn đề chưa được giải quyết và cùng thảo luận các hướng nghiên cứu tiềm năng.
>
> Các hướng được nêu ra chỉ là giả thuyết và gợi ý ban đầu. Chưa có quyết định cuối cùng về bài toán, phương pháp, dữ liệu hoặc sản phẩm nghiên cứu.

---

## 1. Mục đích của giai đoạn hiện tại

Chúng ta đang tìm kiếm một vấn đề khoa học hoặc kỹ thuật đủ quan trọng để phát triển thành một dự án nghiên cứu có thể kiểm chứng.

Dữ liệu viễn thám, NISAR, GIS, AI/ML và mô hình toán học là những công cụ tiềm năng, không phải mục tiêu bắt buộc của dự án.

Nhóm cần tìm hiểu:

- Những vấn đề thực tế hoặc khoa học nào vẫn còn khó giải quyết?
- Các phương pháp hiện có đang gặp hạn chế gì?
- Có thể phát triển một mô hình, phương pháp đánh giá hoặc quy trình kỹ thuật để khắc phục những hạn chế đó không?
- Có dữ liệu đủ tốt để kiểm chứng giả thuyết không?
- Đóng góp tiềm năng có thể là gì: một phát hiện khoa học, mô hình toán học, thuật toán, phương pháp kiểm định hay hệ thống kỹ thuật?
- Làm thế nào để chứng minh kết quả có giá trị thay vì chỉ tạo ra một sản phẩm trực quan?

**Mục tiêu của giai đoạn này không phải hoàn thành một mô hình. Mục tiêu là tìm được vấn đề đáng giải quyết và hiểu đủ sâu để quyết định có nên theo đuổi nó hay không.**

## 2. Ý tưởng xuất phát

Một ý tưởng ban đầu được đưa ra để thảo luận:

Kết hợp dữ liệu vệ tinh NISAR, GIS và các phương pháp AI/ML; nghiên cứu quy trình xử lý, đánh giá chất lượng dữ liệu raster và xem xét khả năng ứng dụng trong dự báo nguy cơ cháy rừng hoặc phân tích hạn–mặn, có kiểm định dữ liệu và mô hình.

Ý tưởng này chưa được xem là đề tài chính thức. Nó đang được dùng làm điểm xuất phát để tìm ra các câu hỏi nghiên cứu có chiều sâu hơn.

Một số vấn đề cần phản biện:

1. Cháy rừng và hạn–mặn có nên được kết hợp hay phải nghiên cứu riêng?
2. Chất lượng dữ liệu vệ tinh ảnh hưởng thế nào đến kết quả phân tích?
3. NISAR có cung cấp thông tin bổ sung mà các nguồn dữ liệu khác chưa cung cấp tốt không?
4. Việc xử lý raster hiện nay còn hạn chế nào đáng nghiên cứu?
5. Có thể nghiên cứu độ bất định, khả năng tổng quát hóa hoặc giới hạn suy luận thay vì chỉ tối ưu độ chính xác không?
6. Có những vấn đề khoa học nào đáng quan tâm hơn nhưng nhóm chưa nhận diện được?

Nhóm được khuyến khích đề xuất cả những hướng không sử dụng NISAR, GIS hoặc AI nếu chúng có giá trị khoa học và tính khả thi cao hơn.

## 3. Những hướng vấn đề đang mở

Các hướng sau không phải danh sách lựa chọn cuối cùng. Chúng là những nhóm câu hỏi để thành viên tìm hiểu và phản biện.

### Hướng A — Chất lượng và độ tin cậy của dữ liệu

- Dữ liệu sau xử lý có thể còn những loại sai số nào?
- Có thể định lượng chất lượng dữ liệu thay vì chỉ đánh dấu dữ liệu hợp lệ hoặc không hợp lệ không?
- Những sai số nào ảnh hưởng đáng kể đến kết quả của mô hình?
- Có thể phát hiện trước khi chạy mô hình rằng dữ liệu không đủ tin cậy cho một nhiệm vụ cụ thể không?
- Các tiêu chí chất lượng nên được thiết kế chung hay riêng cho từng bài toán?

### Hướng B — Giá trị thông tin của dữ liệu vệ tinh

- Một nguồn dữ liệu mới có thực sự cải thiện kết quả so với mô hình cơ sở không?
- Dữ liệu radar cung cấp thông tin gì khác với ảnh quang học, thời tiết hoặc địa hình?
- Khi nào việc kết hợp nhiều nguồn dữ liệu tạo ra giá trị, và khi nào chỉ làm tăng độ phức tạp?
- Có thể xác định điều kiện mà một nguồn dữ liệu không còn hữu ích không?

### Hướng C — Mô hình toán học và phương pháp suy luận

- Có thể biểu diễn mối quan hệ giữa chất lượng dữ liệu, sai số và độ tin cậy đầu ra bằng một mô hình toán học không?
- Có thể định lượng bất định thay vì chỉ đưa ra một giá trị dự báo không?
- Có thể xây dựng tiêu chí xác định khi nào mô hình nên đưa ra kết quả, cảnh báo hoặc từ chối dự báo không?
- Những giả định nào của các mô hình hiện tại chưa được kiểm chứng đầy đủ?

### Hướng D — Khả năng tổng quát hóa

- Mô hình có hoạt động tốt ở khu vực hoặc thời gian chưa từng được sử dụng trong huấn luyện không?
- Kết quả có phụ thuộc quá nhiều vào một địa điểm, mùa vụ hoặc loại thảm phủ không?
- Có thể phân biệt sự cải thiện thực sự với kết quả tốt do cách chia dữ liệu thuận lợi không?
- Làm thế nào để đánh giá mô hình trong điều kiện dữ liệu khác với dữ liệu huấn luyện?

### Hướng E — Các bài toán môi trường

Các ứng dụng ban đầu có thể gồm:

- Dự báo nguy cơ cháy rừng.
- Phân tích hạn và thiếu nước.
- Ước lượng hoặc lập bản đồ độ mặn.
- Theo dõi biến đổi bề mặt và thảm thực vật.
- Phân tích độ ẩm đất hoặc các trạng thái môi trường khác.

Nhóm không cần chọn ngay một ứng dụng. Mỗi ứng dụng phải được đánh giá dựa trên cơ chế khoa học, dữ liệu tham chiếu, khả năng kiểm định và ý nghĩa thực tiễn.

### Hướng F — Những vấn đề chưa được nhận diện

Đây là phần mở hoàn toàn.

Thành viên có thể đề xuất vấn đề từ các ngành khác như vật lý, thống kê, tối ưu hóa, khoa học hệ thống, xử lý tín hiệu, mô hình hóa bất định hoặc các lĩnh vực liên quan.

Không nên giới hạn ý tưởng chỉ vì chúng không nằm trong phạm vi của một công cụ hoặc công nghệ quen thuộc.

## 4. Kiến thức thành viên nên chuẩn bị

Không yêu cầu mọi thành viên phải thành thạo tất cả các lĩnh vực. Mục tiêu là tạo nền tảng chung để nhóm có thể đọc tài liệu và phản biện cùng nhau.

| Lĩnh vực | Kiến thức cần tìm hiểu | Mục đích |
|---|---|---|
| Phương pháp nghiên cứu khoa học | Câu hỏi nghiên cứu, giả thuyết, đối chứng, khả năng bác bỏ giả thuyết | Phân biệt ý tưởng hấp dẫn với nghiên cứu có thể kiểm chứng |
| Viễn thám | Ảnh quang học, SAR, độ phân giải, góc quan sát, tán xạ radar | Hiểu dữ liệu thực sự đo được gì |
| NISAR | Cấu trúc sản phẩm, cấp xử lý, metadata, chất lượng và giới hạn dữ liệu | Xác định dữ liệu phù hợp với bài toán nào |
| GIS và dữ liệu raster | Hệ tọa độ, phép chiếu, độ phân giải, ghép lớp, dữ liệu thiếu | Tránh sai lệch khi kết hợp dữ liệu không gian |
| Toán học và thống kê | Xác suất, hồi quy, sai số, bất định, tương quan, kiểm định giả thuyết | Xây dựng và đánh giá mô hình có cơ sở |
| AI/ML | Huấn luyện, kiểm định, overfitting, baseline, leakage, class imbalance | Đánh giá công bằng hiệu quả của mô hình |
| Validation và calibration | Kiểm định dữ liệu, kiểm định mô hình, hiệu chuẩn xác suất | Đánh giá chất lượng và độ tin cậy đúng cách |
| Khoa học môi trường | Cơ chế cháy, hạn, độ mặn, độ ẩm và thảm thực vật | Tránh suy luận sai từ dữ liệu quan sát |
| Lập trình và quản lý dữ liệu | Python, xử lý dữ liệu, Git, tài liệu hóa thí nghiệm | Tạo quy trình tái lập và làm việc nhóm |

## 5. Tài liệu nền tảng để bắt đầu

Ưu tiên tài liệu chính thức và các bài báo khoa học có phương pháp, dữ liệu và kết quả kiểm chứng rõ ràng.

### Nguồn dữ liệu và viễn thám

- NASA NISAR Mission: https://science.nasa.gov/mission/nisar/
- NASA NISAR Data: https://science.nasa.gov/mission/nisar/data/
- NISAR Products Overview: https://nisar-docs.asf.alaska.edu/products-overview/
- NISAR Calibration and Validation: https://science.nasa.gov/mission/nisar/calibration-and-validation/
- NASA FIRMS — Active Fire Data: https://firms.modaps.eosdis.nasa.gov/

### Tìm kiếm tài liệu khoa học

- NASA ADS: https://ui.adsabs.harvard.edu/
- Google Scholar: https://scholar.google.com/
- Crossref: https://search.crossref.org/
- IEEE Xplore: https://ieeexplore.ieee.org/
- ScienceDirect: https://www.sciencedirect.com/
- Springer Nature: https://link.springer.com/

Các từ khóa ban đầu có thể gồm:

- `NISAR data quality assessment`
- `SAR uncertainty propagation`
- `remote sensing model validation`
- `wildfire risk prediction spatial temporal validation`
- `soil salinity remote sensing field validation`
- `task-aware geospatial data quality`
- `probabilistic calibration environmental prediction`
- `remote sensing domain generalization`

Đây là từ khóa để khảo sát, không phải khẳng định rằng các hướng này đều có khoảng trống nghiên cứu.

## 6. Cách đọc và phản biện một bài báo

Mỗi thành viên khi đọc tài liệu nên ghi lại:

1. **Vấn đề:** Bài báo đang giải quyết câu hỏi nào?
2. **Động cơ:** Vì sao vấn đề đó quan trọng?
3. **Phương pháp hiện có:** Những cách tiếp cận nào đã được sử dụng?
4. **Hạn chế:** Tác giả đã chỉ ra những giới hạn nào?
5. **Dữ liệu:** Dữ liệu có đại diện cho bài toán và điều kiện thực tế không?
6. **Thiết kế kiểm chứng:** Có baseline, dữ liệu độc lập và kiểm định phù hợp không?
7. **Kết quả:** Kết quả chứng minh được điều gì, và không chứng minh được điều gì?
8. **Câu hỏi tiếp theo:** Có giả thuyết nào có thể kiểm tra dựa trên những giới hạn đó?

Không nên xem phần “future work” của một bài báo là bằng chứng đầy đủ về tính mới. Cần tìm các công trình liên quan để kiểm tra liệu vấn đề đó đã được giải quyết ở nơi khác hay chưa.

## 7. Nguyên tắc thảo luận trong nhóm

- Không mặc định ý tưởng ban đầu là đúng.
- Không lựa chọn thuật toán trước khi xác định bài toán.
- Không xem việc sử dụng AI hoặc dữ liệu vệ tinh là đóng góp khoa học tự thân.
- Phân biệt sự kiện quan sát, giả thuyết và kết luận.
- Đề xuất mới phải đi kèm lý do, điều kiện khả thi và cách kiểm chứng.
- Ưu tiên phản biện bằng tài liệu, dữ liệu và thí nghiệm hơn là trực giác.
- Không loại bỏ một hướng chỉ vì nó chưa sử dụng công nghệ mà thành viên quen thuộc.
- Chấp nhận kết quả âm nếu nó được thiết kế và kiểm chứng khoa học.

## 8. Đầu ra mong muốn của giai đoạn thảo luận

Giai đoạn này chưa yêu cầu sản phẩm AI hoàn chỉnh, bản đồ cuối cùng hoặc bài báo hoàn thiện.

Các đầu ra mong muốn gồm:

- Danh sách các vấn đề khoa học và kỹ thuật đáng quan tâm.
- Bộ tài liệu nền tảng có ghi chú và nguồn kiểm chứng.
- Bảng tổng hợp các phương pháp hiện có và hạn chế của chúng.
- Các giả thuyết nghiên cứu ứng viên.
- Đánh giá sơ bộ về dữ liệu, tính khả thi và nguồn lực.
- Danh sách các câu hỏi còn chưa được giải đáp.
- Một quyết định có căn cứ về việc tiếp tục, thu hẹp, kết hợp hay loại bỏ từng hướng.

## 9. Tiêu chí để một ý tưởng được xem xét phát triển

Một hướng nghiên cứu nên được đánh giá qua các câu hỏi:

- Vấn đề có ý nghĩa khoa học hoặc thực tiễn rõ ràng không?
- Có thể diễn đạt thành một câu hỏi nghiên cứu cụ thể không?
- Có cơ sở để cho rằng phương pháp hiện tại còn hạn chế không?
- Có thể thu thập dữ liệu phù hợp để kiểm chứng không?
- Có baseline hoặc phương pháp đối chứng hợp lý không?
- Có thể đánh giá bằng dữ liệu độc lập không?
- Đóng góp tiềm năng có khác biệt đáng kể với các nghiên cứu trước không?
- Nhóm có đủ thời gian, kiến thức và nguồn lực để thực hiện không?

Chưa cần chấm điểm hoặc xếp hạng các hướng ngay. Trước hết, nhóm cần thống nhất cách hiểu các tiêu chí này.

## 10. Trạng thái hiện tại và bước tiếp theo

**Trạng thái hiện tại:**

- Chưa chốt đề tài.
- Chưa chọn thuật toán hoặc mô hình toán học.
- Chưa xác định NISAR là nguồn dữ liệu bắt buộc.
- Chưa quyết định cháy rừng và hạn–mặn sẽ kết hợp hay tách riêng.
- Chưa khẳng định tính mới hoặc hiệu quả của bất kỳ phương pháp nào.

**Bước tiếp theo:**

1. Các thành viên đọc tài liệu nền tảng.
2. Mỗi người đề xuất những vấn đề mình cho là quan trọng, kèm nguồn và lập luận.
3. Cùng phân biệt vấn đề đã được giải quyết, vấn đề còn tranh luận và vấn đề chưa đủ bằng chứng.
4. Xây dựng danh sách giả thuyết nghiên cứu ứng viên.
5. Chỉ sau đó mới đánh giá tính mới, khả năng kiểm chứng và quyết định hướng phát triển.

---

## Tuyên bố định hướng

Dự án bắt đầu bằng việc tìm hiểu một vấn đề, không bắt đầu bằng việc chọn một công nghệ.

Chúng ta chưa cần biết trước kết quả cuối cùng sẽ là một bài báo, mô hình toán học, thuật toán, quy trình kỹ thuật hay một hệ thống ứng dụng. Những hình thức đó sẽ được quyết định sau khi hiểu rõ vấn đề và xác định được loại đóng góp phù hợp.

**Mục tiêu chung là tìm ra một câu hỏi đáng nghiên cứu, hiểu những gì đã được biết, nhận diện điều còn chưa rõ và xây dựng cách kiểm chứng đủ chặt chẽ để tạo ra tri thức mới.**
