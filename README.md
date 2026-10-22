# README — Nghiên cứu NISAR, GIS và AI/ML cho phân tích môi trường

**Tên dự án tạm thời:** Nghiên cứu chất lượng dữ liệu radar NISAR và giá trị thông tin của dữ liệu trong mô hình phân tích, dự báo rủi ro môi trường.

**Trạng thái:** Giai đoạn hình thành câu hỏi nghiên cứu và khảo sát tài liệu.

**Lĩnh vực:** Viễn thám radar · GIS · Khoa học dữ liệu · AI/ML · Mô hình toán học · Phân tích không gian–thời gian.

> **Lưu ý:** Đây là đề cương nghiên cứu ban đầu, chưa phải một phương pháp đã được kiểm chứng. Chưa khẳng định tính mới, hiệu quả của NISAR hay khả năng triển khai tất cả các nhánh đề tài.

---

## 1. Tổng quan dự án

Dự án nghiên cứu cách sử dụng dữ liệu radar vệ tinh NISAR kết hợp với dữ liệu địa không gian và phương pháp thống kê, học máy để giải quyết các bài toán môi trường.

Thay vì chỉ xây dựng bản đồ hoặc triển khai một thuật toán AI, dự án tập trung vào ba vấn đề nền tảng:

1. **Chất lượng dữ liệu:** Dữ liệu vệ tinh sau các bước xử lý còn những nguồn sai số và giới hạn nào?
2. **Giá trị thông tin:** Dữ liệu NISAR có cung cấp thông tin hữu ích bổ sung cho các mô hình phân tích hoặc dự báo môi trường hay không?
3. **Độ tin cậy khoa học:** Làm thế nào để chứng minh kết quả có khả năng tổng quát hóa, định lượng được bất định và được kiểm chứng bằng dữ liệu độc lập?

Hai ứng dụng ban đầu được xem xét là dự báo nguy cơ cháy rừng và phân tích hạn–mặn. Tuy nhiên, đây là những bài toán khác nhau về cơ chế vật lý, dữ liệu tham chiếu và phương pháp đánh giá. Chúng không mặc định thuộc cùng một đề tài.

## 2. Bối cảnh và cơ sở khoa học

NISAR (*NASA–ISRO Synthetic Aperture Radar*) là sứ mệnh vệ tinh radar hợp tác giữa NASA và ISRO. Hệ thống sử dụng radar băng tần L và S để quan sát những thay đổi của bề mặt Trái Đất và các đặc tính liên quan đến đất, thảm thực vật, băng và những hệ thống tự nhiên khác.

Nguồn thông tin chính thức:

- NASA NISAR Mission: https://science.nasa.gov/mission/nisar/
- NISAR Data: https://science.nasa.gov/mission/nisar/data/
- NISAR Products Overview: https://nisar-docs.asf.alaska.edu/products-overview/
- NISAR Calibration and Validation: https://science.nasa.gov/mission/nisar/calibration-and-validation/
- NISAR Data User Guide: https://nisar-docs.asf.alaska.edu/

Dữ liệu radar có đặc điểm khác với ảnh quang học. Tín hiệu radar chịu ảnh hưởng bởi cấu trúc bề mặt, độ ẩm, thảm phủ, hình học quan sát và các yếu tố khác. Vì vậy, không thể mặc định rằng một đặc trưng radar đơn lẻ tương đương trực tiếp với một đại lượng môi trường cụ thể.

Đặc biệt, cần phân biệt:

- Dữ liệu đã hiệu chuẩn với dữ liệu đã được kiểm định đầy đủ cho mọi mục đích sử dụng.
- Raster có cấu trúc kỹ thuật hợp lệ với dữ liệu có chất lượng đo lường tốt.
- Phát hiện điểm nóng đang diễn ra với dự báo nguy cơ cháy trong tương lai.
- Chỉ báo hạn với phép đo độ mặn.
- Độ chính xác phân loại với độ tin cậy của xác suất dự báo.

## 3. Vấn đề nghiên cứu tổng quát

Vấn đề cốt lõi không phải là liệu có thể kết hợp NISAR, GIS và AI hay không, mà là:

**Chất lượng và đặc tính của dữ liệu radar ảnh hưởng như thế nào đến khả năng suy luận về các trạng thái môi trường, và làm thế nào xác định được giá trị thông tin bổ sung của dữ liệu đó bằng thực nghiệm độc lập?**

Câu hỏi này có thể được triển khai thành nhiều hướng nghiên cứu riêng. Mỗi hướng cần xác định đại lượng cần nghiên cứu, giả thuyết, dữ liệu tham chiếu và tiêu chí kiểm chứng trước khi lựa chọn thuật toán.

## 4. Các nhánh nghiên cứu tiềm năng

### Hướng A — Giá trị bổ sung của NISAR trong dự báo nguy cơ cháy rừng

**Câu hỏi nghiên cứu**

Việc bổ sung các đặc trưng radar NISAR có cải thiện chất lượng dự báo nguy cơ cháy rừng so với mô hình cơ sở không sử dụng NISAR hay không?

**Giả thuyết cần kiểm chứng**

NISAR có thể cung cấp thông tin bổ sung về trạng thái bề mặt hoặc thảm thực vật trong một số điều kiện. Tuy nhiên, mức cải thiện thực tế chưa được xác định và có thể thay đổi theo hệ sinh thái, thời gian, chất lượng dữ liệu và cách xây dựng mô hình.

**Luồng nghiên cứu**

1. Xác định khu vực, thời hạn dự báo và định nghĩa sự kiện cháy.
2. Thu thập dữ liệu sự kiện cháy, thời tiết, thảm thực vật, địa hình và NISAR.
3. Xây dựng mô hình cơ sở không sử dụng NISAR.
4. Xây dựng mô hình mở rộng có thêm các đặc trưng NISAR.
5. Kiểm định trên các vùng hoặc thời kỳ độc lập.
6. Đánh giá mức cải thiện, độ tin cậy xác suất và giới hạn chuyển giao.

**Dữ liệu tham chiếu tiềm năng**

NASA FIRMS cung cấp dữ liệu điểm nóng và bất thường nhiệt từ MODIS/VIIRS: https://firms.modaps.eosdis.nasa.gov/

Điểm nóng vệ tinh chỉ là dữ liệu quan sát tham chiếu có giới hạn, không phải nhãn hoàn hảo cho mọi sự kiện cháy. Cần cân nhắc bỏ sót do mây, sai lệch thời gian quan sát và độ phân giải không gian.

**Đóng góp tiềm năng**

Định lượng được khi nào NISAR có giá trị dự báo bổ sung, thay vì chỉ chứng minh một mô hình AI có thể tạo ra bản đồ nguy cơ.

### Hướng B — Ảnh hưởng của chất lượng dữ liệu radar đến độ tin cậy của mô hình

**Câu hỏi nghiên cứu**

Các nguồn sai số và giới hạn chất lượng dữ liệu radar làm thay đổi đầu ra của mô hình môi trường như thế nào?

**Luồng nghiên cứu**

1. Xác định sản phẩm NISAR và cấp xử lý được sử dụng.
2. Xác định các nguồn sai số có liên quan đến sản phẩm và bài toán.
3. Xây dựng chỉ số hoặc tiêu chí đánh giá chất lượng.
4. Đo độ nhạy của mô hình đối với các điều kiện chất lượng khác nhau.
5. Kiểm chứng mối quan hệ giữa chỉ số chất lượng đầu vào và sai số đầu ra.
6. Xác định điều kiện sử dụng đáng tin cậy và những giới hạn cần cảnh báo.

**Mô hình khái niệm**

\[
\Delta Q=f(q_1,q_2,\ldots,q_k)
\]

Trong đó \(q_i\) là các chỉ số chất lượng đầu vào được định nghĩa cụ thể và \(\Delta Q\) là thay đổi chất lượng của kết quả mô hình.

Đây chỉ là cách biểu diễn giả thuyết ban đầu. Dạng hàm, các biến cần sử dụng và quan hệ thực nghiệm phải được xác định qua khảo sát tài liệu và dữ liệu.

**Đóng góp tiềm năng**

Xây dựng được phương pháp định lượng ảnh hưởng của chất lượng dữ liệu đến kết quả suy luận, hoặc xác định được điều kiện mà mô hình không còn đáng tin cậy.

### Hướng C — Đánh giá chất lượng raster theo nhiệm vụ phân tích

**Câu hỏi nghiên cứu**

Có thể xây dựng một quy trình đánh giá dữ liệu địa không gian dựa trên yêu cầu của bài toán, thay vì chỉ kiểm tra định dạng và hệ tọa độ, hay không?

**Luồng nghiên cứu**

1. Xác định yêu cầu đầu vào của bài toán.
2. Kiểm tra hệ tọa độ, độ phân giải, vùng phủ, thời gian và dữ liệu thiếu.
3. Đánh giá những đặc tính chất lượng có ý nghĩa đối với sản phẩm radar.
4. Tạo báo cáo chất lượng cho từng lớp dữ liệu.
5. Kiểm tra xem các cảnh báo chất lượng có liên hệ với sai số của mô hình hay không.

**Đóng góp tiềm năng**

Phát triển quy trình đánh giá chất lượng dữ liệu có tính đến mục tiêu sử dụng (*task-aware data quality assessment*).

Việc ghép nối các công cụ GIS có sẵn chưa đủ để tạo ra đóng góp khoa học. Cần xác định tiêu chí mới, cơ chế ra quyết định hoặc bằng chứng thực nghiệm chứng minh lợi ích.

### Hướng D — Lập bản đồ hạn hoặc độ mặn có định lượng bất định

**Câu hỏi nghiên cứu**

Có thể ước lượng một đại lượng hạn hoặc độ mặn cụ thể từ dữ liệu viễn thám với độ tin cậy được định lượng và kiểm chứng độc lập hay không?

Trước khi lựa chọn mô hình, phải xác định rõ đại lượng đích:

- Hạn khí tượng.
- Hạn nông nghiệp hoặc độ ẩm đất.
- Độ mặn đất.
- Độ mặn nước hoặc xâm nhập mặn.
- Tổ hợp hạn–mặn được định nghĩa bằng các tiêu chí đo lường rõ ràng.

**Luồng nghiên cứu**

1. Chọn đại lượng đích và thang đo.
2. Thu thập dữ liệu quan trắc hoặc đo đạc tham chiếu phù hợp.
3. Xác định những biến viễn thám có cơ sở vật lý.
4. Xây dựng mô hình cơ sở và mô hình mở rộng có NISAR nếu phù hợp.
5. Kiểm định trên mẫu độc lập.
6. Đánh giá sai số, độ bất định và điều kiện áp dụng.

**Đóng góp tiềm năng**

Không chỉ tạo bản đồ mà còn xác định được điều kiện mà dữ liệu đủ thông tin để ước lượng đại lượng cần nghiên cứu, cùng những trường hợp mà kết quả chưa đáng tin cậy.

## 5. Có nên kết hợp các nhánh thành một đề tài?

Các nhánh có thể dùng chung hạ tầng dữ liệu, nhưng không nhất thiết phải ghép thành một bài toán khoa học duy nhất.

Cấu trúc hợp lý ban đầu:

- **Nền tảng dữ liệu:** Hướng B và Hướng C.
- **Ứng dụng dự báo cháy:** Hướng A, có thể kết hợp một phần Hướng B.
- **Ứng dụng hạn hoặc độ mặn:** Hướng D, có thể sử dụng quy trình chất lượng dữ liệu chung.

Chỉ nên kết hợp hai ứng dụng khi có một câu hỏi khoa học chung, dữ liệu đủ tương thích và một thiết kế thí nghiệm có thể kiểm chứng lợi ích của việc tích hợp.

## 6. Quy trình nghiên cứu tổng quát

### Giai đoạn 1 — Khảo sát tài liệu

- Đọc tài liệu chính thức của NASA/ISRO và hướng dẫn sản phẩm NISAR.
- Đọc các nghiên cứu về bài toán môi trường đã chọn.
- Xác định các phương pháp hiện có, cách kiểm định và hạn chế đã được công bố.
- Lập bảng so sánh các công trình gần nhất.

### Giai đoạn 2 — Đánh giá khả thi dữ liệu

- Xác định khu vực và thời kỳ nghiên cứu.
- Kiểm tra độ phủ, tần suất quan sát và loại sản phẩm NISAR.
- Tìm dữ liệu tham chiếu độc lập.
- Kiểm tra tính tương thích về không gian, thời gian và đại lượng đo.

### Giai đoạn 3 — Xây dựng quy trình dữ liệu

- Kiểm tra metadata và tính hợp lệ của dữ liệu.
- Thực hiện các bước tiền xử lý phù hợp với sản phẩm.
- Đánh giá dữ liệu thiếu, sai số và các giới hạn chất lượng.
- Tạo các đặc trưng đầu vào có cơ sở khoa học.

### Giai đoạn 4 — Xây dựng mô hình và đối chứng

- Xây dựng mô hình cơ sở.
- Xây dựng mô hình mở rộng với dữ liệu hoặc phương pháp đề xuất.
- Giữ nguyên nguyên tắc so sánh công bằng giữa các mô hình.
- Kiểm tra độ nhạy và tránh rò rỉ dữ liệu.

### Giai đoạn 5 — Kiểm định độc lập

- Chia dữ liệu theo không gian và/hoặc thời gian phù hợp với mục tiêu.
- Sử dụng nhiều chỉ số đánh giá, không dựa vào một chỉ số duy nhất.
- Đánh giá hiệu chuẩn xác suất khi đầu ra là xác suất.
- Định lượng bất định và xác định giới hạn áp dụng.

### Giai đoạn 6 — Xác định đóng góp

- Đối chiếu kết quả với các phương pháp trước đó.
- Xác định giả thuyết nào được hỗ trợ và giả thuyết nào bị bác bỏ.
- Báo cáo trường hợp mô hình không cải thiện hoặc không đủ dữ liệu.
- Xác định kết quả có thể phát triển thành bài báo, mô hình toán học hoặc công cụ kỹ thuật.

## 7. Phân biệt calibration và validation

| Khái niệm | Mục tiêu |
|---|---|
| Hiệu chuẩn dữ liệu radar | Đưa tín hiệu về thang đo hoặc đặc tính đo lường theo quy trình sản phẩm |
| Kiểm định sản phẩm | Đánh giá chất lượng dữ liệu bằng các phép đo hoặc nguồn tham chiếu phù hợp |
| Kiểm định mô hình | Đánh giá khả năng dự báo hoặc ước lượng trên dữ liệu độc lập |
| Hiệu chuẩn xác suất | Đánh giá mức độ phù hợp giữa xác suất dự báo và tần suất sự kiện quan sát |

Các bước này không thay thế cho nhau. Một sản phẩm đã hiệu chuẩn không đồng nghĩa mô hình sử dụng sản phẩm đó đã được kiểm định; một mô hình có độ chính xác cao cũng không mặc nhiên có xác suất dự báo đáng tin cậy.

## 8. Tiêu chí đánh giá kết quả nghiên cứu

Dự án không nên được đánh giá chỉ dựa trên việc tạo được bản đồ hoặc đạt một chỉ số AI cao.

Các tiêu chí cần xem xét:

- Tính hợp lệ về vật lý của các biến đầu vào.
- Chất lượng và tính độc lập của dữ liệu tham chiếu.
- Hiệu quả so với mô hình cơ sở.
- Khả năng tổng quát hóa theo không gian và thời gian.
- Độ tin cậy xác suất và mức độ bất định.
- Khả năng tái lập thí nghiệm.
- Mức độ rõ ràng của đóng góp so với các công trình trước.

## 9. Rủi ro và giới hạn

1. Dữ liệu NISAR có thể không đủ độ phủ hoặc tần suất quan sát cho thời hạn dự báo mong muốn.
2. Dữ liệu điểm nóng có thể không đại diện đầy đủ cho toàn bộ sự kiện cháy.
3. Độ mặn không thể được suy ra trực tiếp từ mọi đặc trưng radar.
4. Dữ liệu tham chiếu có thể không đồng nhất về thời gian, không gian hoặc phương pháp đo.
5. Mô hình có thể đạt kết quả tốt do rò rỉ dữ liệu hoặc tương quan không gian.
6. Một cải thiện thống kê không tự động chứng minh cơ chế nhân quả.
7. Tính mới chỉ có thể được đánh giá sau khi khảo sát có hệ thống các công trình gần nhất.

## 10. Lộ trình đề xuất

**Bước 1:** Khảo sát tài liệu và xây dựng bảng so sánh các nghiên cứu hiện có.

**Bước 2:** Kiểm tra dữ liệu NISAR thực tế và các nguồn dữ liệu tham chiếu.

**Bước 3:** Chọn một bài toán có thể kiểm chứng, một khu vực và một khoảng thời gian cụ thể.

**Bước 4:** Viết câu hỏi nghiên cứu, giả thuyết, tiêu chí bác bỏ và thiết kế thí nghiệm.

**Bước 5:** Chỉ sau khi xác nhận tính khả thi mới lựa chọn thuật toán, mô hình toán học và cấu trúc hệ thống.

## 11. Tiêu chí để quyết định có tiếp tục hay không

Nên tiếp tục khi có thể trả lời thỏa đáng các câu hỏi sau:

- Bài toán có ý nghĩa khoa học hoặc thực tiễn rõ ràng không?
- Có dữ liệu đủ chất lượng để kiểm chứng giả thuyết không?
- Có mô hình cơ sở hợp lý để so sánh không?
- Có thiết kế kiểm định độc lập để tránh kết quả quá lạc quan không?
- Có khả năng xác định chính xác đóng góp so với nghiên cứu trước không?

Nếu chưa đáp ứng các điều kiện trên, cần thu hẹp hoặc đổi hướng trước khi đầu tư vào một mô hình phức tạp.

---

## 12. Kết luận

Dự án hiện nên được xem là một chương trình khảo sát gồm nhiều nhánh nghiên cứu tiềm năng, không phải một mô hình AI hoàn chỉnh.

Ba hướng cần ưu tiên khảo sát là:

1. Giá trị thông tin bổ sung của NISAR trong một bài toán môi trường cụ thể.
2. Ảnh hưởng của chất lượng dữ liệu radar đến sai số và độ tin cậy của mô hình.
3. Phương pháp đánh giá chất lượng dữ liệu địa không gian dựa trên nhiệm vụ sử dụng.

Hạn–mặn nên được phát triển thành một nhánh riêng nếu chưa có giả thuyết chung đủ mạnh để liên kết với dự báo cháy rừng.

**Nguyên tắc xuyên suốt:** Không mặc định công nghệ tạo ra giá trị khoa học. Giá trị phải được chứng minh thông qua câu hỏi rõ ràng, đối chứng hợp lý, dữ liệu tham chiếu đáng tin cậy và kết quả kiểm định độc lập.

**Trạng thái hiện tại:** Chưa chọn đề tài cuối cùng; chưa khẳng định tính mới; chưa xác nhận tính khả thi của toàn bộ dữ liệu; chưa có kết quả thực nghiệm.
