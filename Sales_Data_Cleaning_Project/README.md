# Sales_Data_Cleaning_Project
Làm sạch dữ liệu bán hàng mô phỏng của Nike/ Clean up Nike's simulated sales data.
# [TÊN DỰ ÁN] Nike's Simulated Sales Data Cleaning & Analysis

## 1. Mục tiêu (Objective)
Dự án này tập trung vào việc xử lý và làm sạch bộ dữ liệu bán lẻ (Retail Sales) chứa nhiều lỗi định dạng, giá trị rỗng và lỗi logic kinh doanh, nhằm chuẩn bị dữ liệu sạch phục vụ cho việc phân tích doanh thu và xu hướng bán hàng.

## 2. Công cụ sử dụng (Tools Used)
- **Python** (Pandas, NumPy)
- **Visualization**: Seaborn, Matplotlib (dùng để check outliers)

## 3. Quy trình xử lý (Key Steps)
Tôi đã thực hiện các bước làm sạch chính sau đây:
- **Xử lý ngày tháng**: Chuẩn hóa định dạng hỗn hợp (mixed format) và loại bỏ các bản ghi thiếu ngày tháng nghiêm trọng.
- **Xử lý logic doanh thu**: Phát hiện 75% dữ liệu gốc bị sai lệch doanh thu. Đã tính toán lại cột `Revenue` dựa trên công thức `Unit * (Price - Discount)`.
- **Xử lý Outliers**: Giữ lại các đơn hàng giá trị cao (Whales) và loại bỏ các đơn hàng rỗng (0 đồng).
- **Kết quả**: Từ 2500 dòng dữ liệu thô, lọc ra được 844 dòng dữ liệu chất lượng cao (High-quality records).

## 4. Cấu trúc thư mục (File Description)
- `Cleaning.ipynb`: Mã nguồn Python chi tiết các bước làm sạch.
- `Data_Uncleaned.csv`: Dữ liệu gốc ban đầu.
- `Data_Cleaned.csv`: Dữ liệu sạch sau khi xử lý.

## 5. Tác giả
Nguyễn Trần Đại Dương
