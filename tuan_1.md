# Tuần 1: Giới thiệu về Chuỗi Thời gian
---

## Mục lục
1. Giới thiệu về Chuỗi Thời gian
2. Các khái niệm cơ bản
3. Các mô hình chuỗi thời gian dừng
4. Các mô hình chuỗi thời gian không dừng
5. Ước lượng dự báo
6. Mô hình có tính mùa vụ
7. Một số mô hình với phương sai thay đổi
8. Một số mô hình học máy
---
## 1. Giới thiệu về chuỗi thời gian (CTG)
- Chuỗi thời gian là dãy các quan sát về một biến số theo thời gian: {$X_t, t \in T$}
    - $X_t$: giá trị quan sát tại thời gian $t$
    - $T$: khoảng thời gian quan sát
- Có thể là chuỗi liên tục ($T$ liên tục) hoặc rời rạc ($T$ rời rạc)
- Khoảng cách giữa các lần quan sát thường chia đều nhau

## 2. Các khái niệm cơ bản
- Ứng dụng: lãi suất, cổ phiếu, nhiệt độ, mưa, gió, sản xuất, điện tim, v.v.
- Ôn tập các đại lượng thống kê:
  - Trung bình (mẫu), trung vị (mẫu), mode (đo xu thế trung tâm)
  - Phương sai (mẫu), độ lệch, $\Delta$ (max-min), $\Delta_Q$ (Q3-Q1), outlier (đo độ phân tán)
- Tính chất kỳ vọng và phương sai:
  - $E(c) = c, D(c) = 0$
  - $E(cX) = cE(X), D(cX) = c^2D(X)$
  - $E(X \pm Y) = E(X) \pm E(Y)$
  - $D(X \pm Y) = D(X) + D(Y)$
- Phân phối chuẩn: $X \sim N(\mu, \delta ^ 2)$

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
- **Thành phần xu hướng (Trend)**: là yếu tố thể hiện xu hướng thay đổi theo thời gian. Thành phần này dùng để chỉ xu hướng tăng hay giảm trong thời gian dài. Biểu diễn bởi một đường thẳng hoặc một đường cong trơn.
- **Thành phần mùa (Seasonal)**: dùng để chỉ xu hướng tăng hay giảm theo mùa trong năm.
- **Thành phần chu kỳ (Cyclical)**: chỉ sự thay đổi theo chu kỳ. Thành phần này khác thành phần mùa ở
chu kỳ kéo dài hơn 1 năm. 
- **Thành phần bất thường (Irregular)**: chỉ sự thay đổi bất thường của giá trị trong chuỗi thời gian. Sự thay đổi này không thể sự đoán bằng các số liệu kinh nghiệm trong quá khứ, không có tính chu kỳ.

## 8. Một số hàm đặc trưng
- **Hàm trung bình:** $\mu_t = E(X_t)$
- **Hàm phương sai:** $\delta^2_t = Var(X_t)$
- **Hàm hiệp phương sai:** $Cov(X_t, X_s) = E[(X_t - \mu_t)(X_s - \mu_s)] = E(X_t, X_s) - \mu_t\mu_s$
- **Hàm tự tương quan:** $\gamma_k = Cov(X_t, X_{t+k})$
- **Hệ số tương quan:** $\rho$ (gần $\pm1$: phụ thuộc tuyến tính mạnh, gần $0$: phụ thuộc yếu)

## 9. Thực hành và kiểm tra
- Thực hành với R
- Kiểm tra:
  - Thường xuyên: 20% (điểm danh, bài tập)
  - Giữa kỳ: 20% (bài kiểm tra)
  - Cuối kỳ: 60% (báo cáo/thi thực hành)

---

> **Ghi chú**: Xem thêm chi tiết và ví dụ trong sách giáo khoa.