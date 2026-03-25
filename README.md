# Phân tích A/B Testing: Tối ưu hóa Retention cho Mobile Game

## 📌 Tổng quan
Dự án phân tích tác động của việc thay đổi vị trí "cổng khóa màn" (level gate) từ cấp độ 30 sang 40 đối với tỷ lệ giữ chân người chơi (Retention).

## 📊 Dữ liệu sử dụng
- [cite_start]Quy mô: **90,189** bản ghi người chơi[cite: 27].
- [cite_start]Các chỉ số chính: `sum_gamerounds` (số ván chơi), `retention_1` (D1), `retention_7` (D7)[cite: 23, 29].

## 🛠️ Quy trình thực hiện
1. [cite_start]**Làm sạch dữ liệu:** Loại bỏ các điểm ngoại lai (Outliers) như tài khoản bot chơi >40.000 ván để đảm bảo tính chính xác[cite: 28].
2. [cite_start]**Phân tích Retention:** Tính toán và so sánh tỷ lệ giữ chân D1 và D7 giữa hai nhóm Gate 30 và Gate 40[cite: 29].
3. [cite_start]**Kiểm định thống kê:** Sử dụng **Chi-Square Test** để xác định sự khác biệt có ý nghĩa thống kê hay không[cite: 23, 30].

## 📈 Kết quả then chốt
- **Gate 30** cho tỷ lệ giữ chân D7 cao hơn (**19.02%**) so với Gate 40 (**18.20%**).
- [cite_start]Kiểm định Chi-Square xác nhận việc chuyển cổng lên level 40 làm giảm tỷ lệ giữ chân người chơi một cách đáng kể (p-value < 0.05)[cite: 30].

## 💡 Đề xuất kinh doanh
Để tối ưu hóa trải nghiệm và giữ chân người chơi lâu dài, sản phẩm nên **giữ nguyên vị trí cổng ở level 30**.
