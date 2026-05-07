# 📊 Data Jobs Market Analysis Dashboard 

## 📝 Tổng quan dự án (Project Overview)
Dự án này là một Interactive Dashboard được xây dựng trên Power BI nhằm phân tích sâu thị trường việc làm trong lĩnh vực Dữ liệu (Data Analytics, Data Science, Data Engineering...). 
Mục tiêu của dự án là cung cấp góc nhìn trực quan về xu hướng kỹ năng (Top Skills), mức lương trung bình (Median Salary) cho từng vị trí, và các chỉ số tổng quan của thị trường để hỗ trợ ứng viên và nhà tuyển dụng đưa ra quyết định dựa trên dữ liệu.
##
![Data Jobs Dashboard v2.0](image/imagedashboard.png)
## 🚀 Các tính năng nổi bật (Key Features)
- **Dynamic Field Parameters:** Tối ưu hóa UI/UX bằng cách cho phép người dùng tự do chuyển đổi thước đo (Ví dụ: Chuyển đổi linh hoạt giữa *Median Hourly Salary* và *Median Yearly Salary*, hoặc xem xét kỹ năng theo *Job Count* và *Job Percent*) trên cùng một không gian biểu đồ.
- **Interactive Filtering:** Tích hợp hệ thống Slicers linh hoạt (Job Title, Country) cùng nút `Clear Slicers` tiện lợi.
- **Dark Theme UI:** Thiết kế giao diện theo phong cách tối (Dark mode) hiện đại, áp dụng nguyên tắc thị giác chữ Z (Z-Pattern) giúp làm nổi bật các chỉ số KPIs quan trọng nhất ở góc trên.

## 🛠 Công cụ & Kỹ thuật sử dụng (Tools & Techniques)
- **Power Query:** Làm sạch dữ liệu thô (Data Wrangling), xử lý lỗi định dạng, và trích xuất đặc trưng (Feature Extraction).
- **Data Modeling:** Xây dựng mô hình dữ liệu chuẩn **Star Schema** (Fact & Dimension tables) để tối ưu hiệu suất truy vấn.
- **DAX (Data Analysis Expressions):**
  - Xây dựng hệ thống Explicit Measures.
  - Sử dụng các hàm điều hướng Filter Context nâng cao (`CALCULATE`, `ALL`) để tính toán tỷ lệ phần trăm phức tạp.
- **Data Visualization:** Thiết kế Dashboard tương tác trên **Power BI Desktop**.


## 💡 Key Insights (Kết quả Phân tích từ Dữ liệu)
Dựa trên tập dữ liệu gồm **479K** tin tuyển dụng, dưới đây là những thông tin cốt lõi rút ra được:

1. **Tổng quan thị trường (Market Overview):** - Mức lương trung bình năm (Median Yearly Salary) của ngành dữ liệu đạt mức **$113.25K**.
   - Trung bình mỗi tin tuyển dụng yêu cầu ứng viên phải đáp ứng khoảng **4.8** kỹ năng (Skills Per Job).
2. **Kỹ năng "Vàng" (Top Demand Skills):** - **Python** và **SQL** là hai kỹ năng thống trị tuyệt đối, xuất hiện trong khoảng 50% tổng số tin tuyển dụng ngành dữ liệu.
   - Các nền tảng Điện toán đám mây (Cloud Computing) như **AWS** và **Azure** theo sát ở vị trí tiếp theo, cho thấy xu hướng dịch chuyển dữ liệu lên Cloud của các doanh nghiệp.
3. **Mức lương theo vị trí (Top Paying Jobs):** - Các vị trí cấp cao như **Senior Data Scientist** và **Machine Learning Engineer** dẫn đầu bảng lương với mức Median Salary xấp xỉ hoặc vượt ngưỡng **$150K/năm**.
   - Vai trò cốt lõi về hạ tầng như **Data Engineer/Software Engineer** có mức định giá cao hơn so với **Data Analyst/Business Analyst**. Tuy nhiên, Data Analyst vẫn giữ mức lương trung bình ổn định ở khoảng $90K - $100K/năm.

## 📂 Cấu trúc thư mục (Repository Structure)
- `/DataJob_ver2`
  - `/image`: Chứa hình ảnh chụp màn hình Dashboard (`imagedashboard.png`).
  - `Data_Jobs_Dashboard_upgraded.pbix`: File Power BI chứa toàn bộ Data Model, DAX và Report (Version 2.0).
  - `README.md`: Tài liệu mô tả dự án.