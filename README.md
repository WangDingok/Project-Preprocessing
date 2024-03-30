# Football Europe 
 Preprocessing data and use classification model to classify match 

## Project Overview
Dữ liệu này cung cấp cho chúng ta thông tin về các trận đấu đã diễn ra tại giải đấu Europe và tỷ lệ cược trên các sàn cá độ tài trợ như Bet365 và Blue Square. Mục tiêu của dự án này là xây dựng mô hình học máy để phân loại các trận đấu thắng và thua trong giải đấu để cung cấp thông tin hợp lý cho các nhà cái , dựa trên các thuộc tính đã có sẵn trong bộ dữ liệu 

### Dataset Information
Tập dữ liệu này chứa thông tin về các đội bóng thuộc liên đoàn bóng đá Châu Âu và các trận đấu đã thi đấu cùng với tỉ lệ cược trên các sàn cá độ được diễn ra trong giải đấu Europe

#### Data Features
Tập dữ liệu bao gồm 18 biến, bao gồm :

1. **ID:** ID của từng trận đấu
2. **Country_name:** Tên quốc gia của đội bóng tham gia giải đấu
3. **League_name:** Tên giải đấu 
4. **Season:** Mùa giải thi đấu
5. **Date:** Ngày diễn ra trận đấu
6. **Home_team:** Đội nhà
7. **Away_team:** Đội khách
8. **B365H , B365D , B365A:** Tỷ lệ cá cược đội nhà thắng , hòa và đội khách thắng trên sàn 365bet
9. **BSH , BSD , BSA:** Tỷ lệ cá cược đội nhà thắng , hòa và đội khách thắng trên sàn Blue Square
10. **Diff_goals:** Hiệu số bàn thắng
11. **Target:** Mục tiêu

## Data Preprocessing
1. **Data Cleaning:** Kiểm tra các giá trị còn thiếu và xử lý chúng một cách thích hợp. Đảm bảo tính nhất quán trong các kiểu dữ liệu.
2. **Data Exploration:** Thực hiện phân tích dữ liệu khám phá (EDA) để hiểu sự phân bổ dữ liệu và mối quan hệ giữa các tính năng.
3. **Feature Engineering:** Create new features if necessary and encode categorical variables  (e.g., one-hot encoding for education and marriage).
4. **Data Split:** Chia tập dữ liệu thành tập huấn luyện và tập kiểm tra để đánh giá mô hình.

## Model Building
1. **Model Selection:** Chọn một thuật toán học máy thích hợp để phân loại nhị phân. Các lựa chọn phổ biến bao gồm Hồi quy logistic, Rừng ngẫu nhiên hoặc Tăng cường độ dốc.
2. **Model Training:** Huấn luyện mô hình đã chọn trên dữ liệu huấn luyện.
3. **Model Evaluation:** Evaluate the model's performance using appropriate metrics such as accuracy, precision, recall, F1-score on the testing data.

## Conclusion
Dự án phân loại các trận đấu bao gồm quá trình tiền xử lý dữ liệu, xây dựng mô hình và triển khai mô hình học máy để phân loại các trận đấu bóng đá.

Dự án nhằm mục đích hỗ trợ cung cấp thông tin cho các nhà cái nhằm thao tác nhanh hơn và tổng hợp dữ liệu để đưa ra các phương án hợp lý cho các nhà cái.