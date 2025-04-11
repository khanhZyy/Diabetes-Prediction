# Dataset Diabetes Prediction
Tập dữ liệu cung cấp các thông tin y tế liên quan đến bệnh tiểu đường của các bệnh nhân gồm 100000 
hàng và 9 cột:  
• gender (giới tính) : đề cập đến giới tính sinh học của bệnh nhân, có thể ảnh hưởng đến khả năng mắc bệnh tiểu đường của họ. Có ba danh mục trong đó: Male (nam), 
Female (nữ) và Other (khác).  
• age (tuổi): là một yếu tố quan trọng vì tiểu đường thường được chẩn đoán nhiều hơn ở người lớn tuổi. Tuổi biến động từ 0-80 trong tập dữ liệu.  
• hypertension (cao huyết áp): là một tình trạng y tế trong đó áp suất máu trong các động mạch tăng liên tục. Nó có giá trị 0 hoặc 1, trong đó 0 cho biết họ không có cao huyết áp và 1 cho biết họ có cao huyết áp.   
• heart_disease (Bệnh tim): là một tình trạng y tế khác liên quan đến việc tăng nguy cơ mắc bệnh tiểu đường. Nó có giá trị 0 hoặc 1, trong đó 0 cho biết họ không có bệnh tim và 1 cho biết họ có bệnh tim.  
• smoking_history (Lịch sử hút thuốc): cũng được coi là một yếu tố nguy cơ cho tiểu đường và có thể làm tăng các vấn đề liên quan đến tiểu đường. Trong tập dữ liệu, có 6 danh mục: not current(không hiện tại) ,former (trước đây),No Info (không có 
thông tin) ,current (hiện tại), never (không bao giờ) and ever (đã từng).  
• BMI (Body Mass Index) là thước đo lượng mỡ cơ thể dựa trên cân nặng và chiều cao. Chỉ số BMI cao hơn có liên quan đến nguy cơ mắc bệnh tiểu đường cao hơn. Phạm vi BMI trong tập dữ liệu là từ 10,16 đến 71,55. BMI dưới 18,5 là thiếu cân, 
18,5-24,9 là bình thường, 25-29,9 là thừa cân, và 30 trở lên là béo phì.  
• HbA1c_level: HbA1c (Hemoglobin A1c) là thước đo mức đường huyết trung bình của một người trong vòng 2-3 tháng qua. Các mức cao hơn chỉ ra nguy cơ cao về tiểu đường. Đa số mức HbA1c trên 6,5% chỉ ra tiểu đường.  
• blood_glucose_level: Mức đường huyết đề cập đến lượng glucose trong máu tại mộtthời điểm nhất định. Mức đường huyết cao là dấu hiệu chính của bệnh tiểu đường.  
• diabetes (tiểu đường) là biến mục tiêu đang được dự đoán, với giá trị 1 cho biết có bệnh tiểu đường và 0 cho biết không có bệnh tiểu đường.  
# Thực hiện bài toán
Quy trình thực hiện bài toán  
![image](https://github.com/user-attachments/assets/849e3b18-4248-404a-a934-942ec3031a06)
Xây dựng 3 mô hình:  xây dựng mô hình Logistic Regression, Decision Tree, và Random Forest  
Kết quả sau khi huấn luyện
![image](https://github.com/user-attachments/assets/90eacb30-8d50-4b79-9722-7b1e5c470233)
Dựa vào bảng kết quả đánh giá các mô hình, ta thấy là sau khi huấn luyện các mô hình đều có độ chính xác khá cao. Đặc biệt là các mô hình Decision Tree, Random Forest đều có độ chính xác 96% - 97%. Đồng thời thì các thông số khác như độ chuẩn xác 
(precision), độ bao phủ (recall), F1-score đều cao. Trong cả 3 mô hình được train thì mô hình Random Forest có độ chính xác cao nhất là 0.974 tuy nhiên thời gian huấn luyện tương đối lâu 33.9707 giây. Khi so sánh mô hình Random Forest với mô hình độ chính xác cao 
thứ 2 là Decision Tree (0.9626) thì sự chênh lệch về độ chính xác của 2 mô hình là rất nhỏ khoảng 0.0114, trong khi đó thì mô hình Decision Tree lại có thời gian huấn luyện tương đối ngắn chỉ 0.5889 giây. Vì vậy mà mô hình tốt nhất được lựa chọn để triển khai ở đây là 
Decision Tree. 



