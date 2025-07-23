## Customer Churn Prediction



## 📌 Problem Definition
The `Customer Churn table` contains information on all `7,043` customers from a `Telecommunications company` in California in Q2 2022

Each record represents `one customer`, and contains details about their `demographics`, `location`, `tenure`, `subscription services`, `status for the quarter` `(joined, stayed, or churned)`, and more!

The `Zip Code Population` table contains complimentary information on the estimated populations for the California zip codes in the Customer Churn table

We need to `predict` whether the customer will `churn`, `stay` or `join` the company based on the parameters of the dataset.
<br><br>

## 📓 Overview

| Machine Learning Models Applied            | Accuracy |
| ----------------- | ------------------------------------------------------------------ |
| Random Forest | 78.11% |
| Logistic Regression | 78.28% |
| Naive Bayes Gaussian | 36.77% |
| Decision Tree | 77.29% |
| XGB_Classifier | 80.86% |

<br>

## 👉 Application

The ability to predict churn before it happens allows businesses to take proactive actions to keep existing customers from churning. This could look like: 
```
  Customer success teams reaching out to those high-risk customers to provide support or to gauge 
  what needs may not be being met.
```

The advantage of calculating a company's churn rate is that it provides clarity on how well the business is retaining customers, which is a reflection on the quality of the service the business is providing, as well as its usefulness.

## 🔍 Data Exploration & Preprocessing

Trước khi xây dựng mô hình, dữ liệu đã được xử lý kỹ lưỡng để đảm bảo chất lượng:

- **Xử lý thiếu dữ liệu**: Cột `TotalCharges` chứa giá trị trống đã được làm sạch hoặc chuyển đổi phù hợp.
- **Chuyển đổi kiểu dữ liệu**: Một số cột được ép kiểu từ `object` sang `float` để phục vụ cho việc phân tích.
- **Biến đổi nhãn**: Sử dụng `Label Encoding` và `One-Hot Encoding` để xử lý các biến phân loại.
- **Cân bằng dữ liệu**: Kiểm tra phân phối nhãn và thực hiện điều chỉnh nếu cần thiết để cải thiện độ chính xác mô hình.

---

## 📊 Exploratory Data Analysis (EDA)

Phân tích dữ liệu ban đầu giúp hiểu rõ hơn về hành vi của khách hàng:

- Trực quan hóa mối quan hệ giữa `churn` và các yếu tố như: loại dịch vụ, phương thức thanh toán, thời gian sử dụng (tenure), v.v.
- Dùng biểu đồ cột, histogram, boxplot và heatmap để phát hiện các xu hướng, điểm bất thường và tương quan trong dữ liệu.

---

## ⚙️ Model Training & Evaluation

Các mô hình được huấn luyện và so sánh hiệu suất:

- **Tách tập dữ liệu**: 80% cho huấn luyện, 20% cho kiểm thử.
- **Chuẩn hóa dữ liệu**: Sử dụng `StandardScaler` để đảm bảo các mô hình hoạt động hiệu quả.
- **Huấn luyện nhiều mô hình**: Logistic Regression, Random Forest, Decision Tree, Gaussian Naive Bayes, XGBoost.
- **Đánh giá mô hình**: Dựa trên độ chính xác (`Accuracy`), cùng với `Confusion Matrix`, `Precision`, `Recall`, và `F1-score`.

---

## 📈 Visualization

Dữ liệu và kết quả được minh họa trực quan:

- Ma trận nhầm lẫn cho từng mô hình
- Biểu đồ so sánh độ chính xác giữa các thuật toán
- Biểu đồ phân phối khách hàng theo churn status
- ROC Curve cho bài toán phân loại (nếu applicable)

---

## 💡 Insights

Một số điểm rút ra từ quá trình phân tích:

- Khách hàng trả sau và dùng nhiều dịch vụ đồng thời có khả năng churn cao hơn.
- Thời gian gắn bó (`tenure`) càng thấp, khả năng churn càng cao.
- Một số khu vực địa lý có mật độ churn cao đáng kể.

## 📬 Contact

Mọi thắc mắc hoặc đóng góp, vui lòng liên hệ:

- 📧 Email: [luudoanngocphat@gmail.com](mailto:luudoanngocphat@gmail.com)
- 📞 Phone: 0905939655
