# Phân tích A/B Testing: Tối ưu hóa Retention cho Mobile Game

## 📌 Tổng quan
Dự án thực hiện phân tích tác động của việc thay đổi vị trí "cổng khóa màn" (level gate) từ cấp độ 30 sang 40 đối với tỷ lệ giữ chân người chơi (Retention).

## 📊 Dữ liệu sử dụng
- **Quy mô:** 90,189 bản ghi người chơi.
- **Các chỉ số chính:**
  - `sum_gamerounds`: Tổng số ván chơi.
  - `retention_1`: Tỷ lệ quay lại sau 1 ngày (D1).
  - `retention_7`: Tỷ lệ quay lại sau 7 ngày (D7).

## 🛠️ Quy trình thực hiện
1. **Làm sạch dữ liệu:** Xử lý các giá trị ngoại lai (Outliers), loại bỏ các tài khoản bot hoặc dữ liệu bất thường (ví dụ: người chơi >40.000 ván).
2. **Phân tích Retention:** Tính toán và so sánh tỷ lệ % giữ chân giữa hai nhóm thử nghiệm `gate_30` và `gate_40`.
3. **Kiểm định thống kê:** Áp dụng **Chi-Square Test** để xác nhận sự khác biệt giữa các nhóm có ý nghĩa thống kê hay không (p-value).

## 📈 Kết quả then chốt
- **Retention D1:** Nhóm Gate 30 (44.82%) cao hơn Gate 40 (44.23%).
- **Retention D7:** Nhóm Gate 30 (**19.02%**) vượt trội hơn Gate 40 (**18.20%**).
- **Kết luận:** Kiểm định Chi-Square cho thấy việc đặt cổng ở level 40 làm giảm đáng kể khả năng giữ chân người chơi.

## 💡 Đề xuất 
Dựa trên dữ liệu, đề xuất **giữ nguyên vị trí cổng ở level 30** để tối ưu hóa chỉ số Retention và trải nghiệm người dùng.
