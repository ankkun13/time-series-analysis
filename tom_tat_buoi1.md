# Tóm tắt và ghi chép môn Phân tích chuỗi thời gian

## 1. Giới thiệu về chuỗi thời gian (CTG)
- Chuỗi thời gian là dãy các quan sát về một biến số theo thời gian: {X_t, t ∈ T}
- X_t: giá trị quan sát tại thời gian t
- T: khoảng thời gian quan sát
- Có thể là chuỗi liên tục (T liên tục) hoặc rời rạc (T rời rạc)
- Khoảng cách giữa các lần quan sát thường chia đều nhau

## 2. Các khái niệm cơ bản
- Ứng dụng: lãi suất, cổ phiếu, nhiệt độ, mưa, gió, sản xuất, điện tim, v.v.
- Ôn tập các đại lượng thống kê:
  - Trung bình, trung vị, mode (đo xu thế trung tâm)
  - Phương sai, độ lệch, delta (max-min), Delta Q (Q3-Q1), outlier (đo độ phân tán)
- Tính chất kỳ vọng và phương sai:
  - E(c) = c, D(c) = 0
  - E(cX) = cE(X), D(cX) = c²D(X)
  - E(X±Y) = E(X)±E(Y)
  - D(X±Y) = D(X) + D(Y)
- Phân phối chuẩn: X ~ N(EX, DX)

## 3. Các mô hình chuỗi thời gian
- Chuỗi dừng
- Chuỗi không dừng
- Mô hình có tính mùa vụ
- Mô hình với phương sai thay đổi
- Một số mô hình học máy

## 4. Ước lượng và dự báo
- Phương pháp bình phương tối thiểu
- Phương pháp mô men
- MLE (Maximum Likelihood Estimation)

## 5. Mục đích phân tích chuỗi thời gian
- Hiểu và mô hình hóa chuỗi thời gian
- Dự báo các giá trị tương lai

## 6. Các bước xây dựng mô hình chuỗi thời gian
1. Xác định mô hình
2. Điều chỉnh mô hình (model fitting)
3. Chuẩn đoán mô hình

## 7. Các thành phần của dữ liệu chuỗi thời gian
- **Xu hướng (Trend):** thay đổi dài hạn, tăng/giảm, biểu diễn bởi đường thẳng hoặc cong trơn
- **Mùa vụ (Seasonal):** thay đổi theo mùa trong năm
- **Chu kỳ (Cyclical):** thay đổi theo chu kỳ dài hơn 1 năm
- **Bất thường (Irregular):** biến động không dự đoán được, không có tính chu kỳ

## 8. Một số hàm đặc trưng
- **Hàm trung bình:** μ_t = E(X_t)
- **Hàm phương sai:** σ²_t = Var(X_t)
- **Hàm hiệp phương sai:** Cov(X_t, X_s) = E[(X_t - μ_t)(X_s - μ_s)] = E(X_t, X_s) - μ_tμ_s
- **Hàm tự tương quan:** γ_k = Cov(X_t, X_{t+k})
- **Hệ số tương quan:** ρ (gần ±1: phụ thuộc tuyến tính mạnh, gần 0: phụ thuộc yếu)
- **Trung bình trượt**

## 9. Thực hành và kiểm tra
- Thực hành với R
- Kiểm tra:
  - Thường xuyên: 20% (điểm danh, bài tập)
  - Giữa kỳ: 20% (bài kiểm tra)
  - Cuối kỳ: 60% (báo cáo/thi thực hành)

---

*Ghi chú: Xem thêm chi tiết và ví dụ trong sách giáo khoa. Tính dừng, trung bình trượt, các mô hình cụ thể sẽ được học sâu hơn ở các buổi sau.*
