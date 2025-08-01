#  Patient Clustering with Data Mining

##  Giới thiệu
Dự án này thực hiện **phân cụm bệnh nhân** dựa trên dữ liệu y tế (70,000 bản ghi), nhằm nhận diện các nhóm bệnh nhân có đặc điểm sức khỏe tương đồng, hỗ trợ phân tích và dự đoán nguy cơ bệnh tim.

Dự án được phát triển trên **Google Colab** bằng Python, áp dụng các kỹ thuật tiền xử lý dữ liệu, trực quan hóa, và phân cụm với nhiều thuật toán khác nhau.

---

##  Dataset
- **Nguồn dữ liệu:** `cardio_train.csv`
- **Kích thước:** ~70,000 bản ghi – 12 cột
- **Thuộc tính nổi bật:**
  - `age`, `height`, `weight`, `ap_hi`, `ap_lo` (định lượng)
  - `gender`, `cholesterol`, `gluc`, `smoke`, `alco`, `active`, `cardio` (định tính)
- Không có giá trị thiếu (NaN).

---

##  Công nghệ sử dụng
- **Ngôn ngữ:** Python 3.10+
- **Công cụ:** Google Colab, Jupyter Notebook
- **Thư viện chính:**
  - `numpy`, `pandas` – Xử lý dữ liệu
  - `matplotlib`, `seaborn` – Trực quan hóa dữ liệu
  - `scikit-learn` – Phân cụm & đánh giá (Silhouette Score, Davies-Bouldin, Calinski-Harabasz)
  - `scipy` – Tính toán khoảng cách

---

##  Các bước thực hiện
1️ **Data Understanding** – Khám phá dữ liệu, loại bỏ cột `id`, tạo thêm trường `age_years`.  
2️ **Data Preparation** – Làm sạch dữ liệu (lọc huyết áp không hợp lý, tính BMI, chuẩn hóa dữ liệu).  
3️ **Modeling** – Áp dụng thuật toán phân cụm (STING, K-Means, hoặc tương tự).  
4️ **Evaluation** – Đánh giá chất lượng cụm bằng **Silhouette Score**, **Davies-Bouldin Score**.  
5️ **Visualization** – Vẽ biểu đồ cụm, biểu đồ phân bố để minh họa kết quả.

---



