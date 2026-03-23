# Định lượng các yếu tố kinh tế – xã hội chi phối mức độ hạnh phúc toàn cầu 🌍
## What Really Drives Happiness?  
*A Data-Driven Investigation of Economic and Social Factors*

---

# 1. Mục tiêu phân tích

Bài phân tích này nhằm khám phá các yếu tố cốt lõi ảnh hưởng đến mức độ hạnh phúc toàn cầu thông qua cách tiếp cận dựa trên dữ liệu.

Cụ thể, dự án tập trung vào:

1. Phân tích phân bố mức độ hạnh phúc giữa các quốc gia nhằm nhận diện xu hướng, sự chênh lệch và khác biệt theo khu vực.

2. Khai thác và đánh giá mức độ ảnh hưởng của các yếu tố kinh tế - xã hội quan trọng, bao gồm:
   - GDP (thu nhập bình quân đầu người)  
   - Sức khỏe (tuổi thọ)  
   - Hỗ trợ xã hội  
   - Mức độ tự do cá nhân
   - Mức độ hào phóng dành cho người khác
   - Niềm tin vào chính phủ  

3. Đo lường mối quan hệ giữa các biến số và mức độ hạnh phúc thông qua các kỹ thuật phân tích khám phá dữ liệu (EDA) và tương quan.

4. Xác định các quốc gia có mức độ hạnh phúc cao hoặc thấp hơn kỳ vọng so với điều kiện kinh tế, từ đó làm rõ vai trò của các yếu tố phi kinh tế.

5. Đưa ra các kết luận phân tích có giá trị, hỗ trợ định hướng chính sách và cung cấp góc nhìn toàn diện về phát triển phúc lợi xã hội.

---

## 🧠 Các câu hỏi nghiên cứu

1. 10 Quốc gia nào có mức độ hạnh phúc cao nhất?  
2. Hạnh phúc có thay đổi theo thời gian không?  
3. Quốc gia giàu có luôn hạnh phúc hơn không?  
4. Yếu tố nào ảnh hưởng mạnh nhất đến hạnh phúc?  
5. Có quốc gia nào vượt kỳ vọng so với GDP không?  

---

# 2. Mô tả dữ liệu

Dataset được sử dụng là **World Happiness Report (2015–2019)** từ Kaggle. Dataset gồm dữ liệu đa quốc gia theo chuỗi thời gian (2015–2019), phản ánh mức độ hạnh phúc và các yếu tố kinh tế – xã hội liên quan.

📌 Link dataset:  
https://www.kaggle.com/datasets/unsdsn/world-happiness

---

## 🎯 Tổng quan dataset

- ~170 quốc gia  
- 5 năm dữ liệu  
- Mỗi dòng đại diện cho một quốc gia trong một năm

| Country     | Year | Happiness Score | GDP per Capita | Social Support | Life Expectancy | Freedom | Generosity | Corruption |
| ----------- | ---- | --------------- | -------------- | -------------- | --------------- | ------- | ---------- | ---------- |
| Finland     | 2019 | 7.769           | 1.340          | 1.587          | 0.986           | 0.596   | 0.153      | 0.393      |
| Denmark     | 2019 | 7.600           | 1.383          | 1.573          | 0.996           | 0.592   | 0.252      | 0.410      |
| Norway      | 2019 | 7.554           | 1.488          | 1.582          | 1.028           | 0.603   | 0.271      | 0.341      |
| Iceland     | 2019 | 7.494           | 1.380          | 1.624          | 1.026           | 0.591   | 0.354      | 0.118      |
| Netherlands | 2019 | 7.488           | 1.396          | 1.522          | 0.999           | 0.557   | 0.322      | 0.298      |

Bảng trên chỉ trình bày một phần dữ liệu đại diện cho mục đích minh họa; toàn bộ dataset bao gồm 781 quan sát và 9 biến trong giai đoạn 2015–2019.


## 📌 Các biến quan trọng

- Country: Tên quốc gia  
- Happiness Score: Điểm hạnh phúc  
- Economy (GDP per Capita): GDP  
- Social Support : Hỗ trợ xã hội  
- Health (Life Expectancy): Tuổi thọ  
- Freedom: Tự do
- Genorosity : Độ hào phóng cho người khác
- Trust (Government Corruption): Niềm tin vào chính phủ
- Year: Năm
  
  ---
  
# 3. Phương pháp phân tích

Quy trình phân tích được thực hiện theo hướng tiếp cận dữ liệu, bao gồm các bước chính:

1. **Data Understanding**: Khảo sát cấu trúc và ý nghĩa dữ liệu  
2. **Data Cleaning**: Làm sạch và chuẩn hóa dữ liệu  
3. **EDA**: Khám phá xu hướng và mối quan hệ giữa các biến  
4. **Visualization**: Sử dụng Power BI để trực quan hóa dữ liệu, giúp làm nổi bật các xu hướng, so sánh giữa các quốc gia và hỗ trợ diễn giải kết quả một cách trực quan và hiệu quả.
5. **Kết luận phân tích**: Tổng hợp các phát hiện chính từ dữ liệu, từ đó đưa ra các kết luận có giá trị và hàm ý đối với việc hiểu và cải thiện mức độ hạnh phúc của các quốc gia

## 🚀 Công cụ và công nghệ sử dụng

Quá trình phân tích được thực hiện với sự hỗ trợ của các công cụ sau:

- **Python (GG colab)**: Xử lý dữ liệu, làm sạch dữ liệu và thực hiện phân tích khám phá (EDA)  
- **Power BI**: Trực quan hóa dữ liệu và xây dựng dashboard nhằm hỗ trợ diễn giải kết quả  
- **GitHub**: Quản lý mã nguồn và trình bày dự án một cách minh bạch, có hệ thống

---

# BÀI PHÂN TÍCH

# Cấu trúc dữ liệu

![ERD](https://drive.google.com/uc?export=view&id=1w-nd2dIMUubCV1wT-YH0yIEv1v8IEmcS)

# Phân tích 1: 10 Quốc gia nào có mức độ hạnh phúc cao nhất?  
### Giả thuyết  
Phần lớn các quốc gia có mức hạnh phúc ở ngưỡng trung bình, trong khi số quốc gia đạt mức rất cao hoặc rất thấp chiếm tỷ trọng nhỏ.

| Happiness Group | Count |
|-----------------|------:|
| 0-4             | 18   |
| 4-5             | 43   |
| 5-6             | 59   |
| 6-7             | 36   |
| 7+              | 14   |

<img width="640" height="341" alt="image" src="https://github.com/user-attachments/assets/19f0e134-4eed-4e77-9fe7-133fe81243a9" />

### Kết luận:
Phân bố cho thấy mức độ hạnh phúc toàn cầu tập trung chủ yếu trong khoảng 5–7 điểm, phản ánh một “mặt bằng trung bình” tương đối ổn định giữa các quốc gia;  mức hạnh phúc rất cao (trên 7 điểm) chỉ chiếm một tỷ lệ nhỏ.  
Điều này cho thấy mức hạnh phúc cao không phải là kết quả của một yếu tố đơn lẻ, mà là sự tổng hòa của nhiều điều kiện kinh tế, xã hội và thể chế.

---

# Phân tích 2: Hạnh phúc có thay đổi theo thời gian không?

### Giả thuyết: 
Mức độ hạnh phúc toàn cầu duy trì tương đối ổn định trong giai đoạn 2015–2019, chỉ có những biến động nhỏ theo thời gian.

| Year | Avg Happiness |
| ---- | ------------- |
| 2015 | ~5.37         |
| 2016 | ~5.38         |
| 2017 | ~5.35         |
| 2018 | ~5.36         |
| 2019 | ~5.41         |

<img width="663" height="320" alt="image" src="https://github.com/user-attachments/assets/13a052e4-e9a5-46cc-b054-7d4019bc0a99" />

### Kết luận:
Mặc dù mức độ hạnh phúc toàn cầu có biến động nhẹ trong giai đoạn 2015–2019, đặc biệt là sự sụt giảm vào năm 2017 và phục hồi sau đó, nhưng biên độ thay đổi nhìn chung khá nhỏ.

Điều này cho thấy hạnh phúc là một chỉ số vĩ mô có tính ổn định tương đối theo thời gian và không dễ bị tác động bởi các biến động ngắn hạn. Nói cách khác, những thay đổi về hạnh phúc có xu hướng diễn ra chậm và cần các yếu tố mang tính cấu trúc, dài hạn để tạo ra sự khác biệt đáng kể.




