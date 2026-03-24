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

1. Điều gì tạo nên hạnh phúc ở 10 quốc gia top đầu?
2. Hạnh phúc có thay đổi theo thời gian không?  
3. Quốc gia giàu có có luôn hạnh phúc hơn không?  
4. Yếu tố nào ảnh hưởng mạnh nhất đến hạnh phúc?  
5. Mức độ chênh lệch hạnh phúc giữa các quốc gia có đang thu hẹp hay gia tăng theo thời gian? 

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

# Phân tích 1: Điều gì tạo nên hạnh phúc ở 10 quốc gia top đầu?

### Giả thuyết  
Các quốc gia có mức độ hạnh phúc cao không chỉ dựa vào một yếu tố đơn lẻ (như GDP), mà đạt được kết quả này nhờ sự kết hợp cân bằng giữa các yếu tố kinh tế, xã hội và chất lượng sống.

| Mã giả thuyết | Giả thuyết                                                                 | Kỳ vọng                                                                 |
|--------------|--------------------------------------------------------------------------------------|-------------------------------------------------------------------------|
| H1           | GDP bình quân đầu người cao dẫn đến mức độ hạnh phúc cao hơn                         | Quốc gia có GDP cao sẽ có điểm hạnh phúc cao hơn                       |
| H2           | Hỗ trợ xã hội có ảnh hưởng đáng kể đến hạnh phúc                   | Quốc gia có mức hỗ trợ xã hội cao sẽ xếp hạng cao về hạnh phúc         |
| H3           | Tuổi thọ có tác động tích cực đến hạnh phúc                       | Quốc gia có tuổi thọ cao hơn sẽ có mức hạnh phúc cao hơn               |
| H4           | Tự do trong việc đưa ra lựa chọn cuộc sống làm tăng mức độ hạnh phúc                | Quốc gia có mức độ tự do cao sẽ có điểm hạnh phúc cao hơn              |
| H5           | Hạnh phúc được tạo nên từ sự kết hợp của nhiều yếu tố                               | Các quốc gia top có cấu trúc điểm cân bằng, không phụ thuộc 1 yếu tố    |
| H6           | Mức độ tham nhũng thấp (niềm tin vào chính phủ cao) góp phần làm tăng hạnh phúc     | Quốc gia có mức tham nhũng thấp sẽ có điểm hạnh phúc cao hơn           |

<img width="919" height="557" alt="image" src="https://github.com/user-attachments/assets/ccfbdd44-3e73-4167-85c1-f50c15fdf37d" />


### Kết luận:
Phân tích cho thấy các quốc gia có mức độ hạnh phúc cao không phụ thuộc vào một yếu tố duy nhất, mà đạt được nhờ sự cân bằng đồng đều giữa nhiều khía cạnh như kinh tế, hỗ trợ xã hội và chất lượng sống.

Mặc dù GDP và hỗ trợ xã hội đóng vai trò quan trọng, chúng không đủ để giải thích hoàn toàn sự khác biệt về mức độ hạnh phúc. Thay vào đó, các quốc gia top đầu thể hiện một “hệ sinh thái hạnh phúc” ổn định, nơi tất cả các yếu tố cùng đạt mức cao một cách nhất quán.

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

# Phân tích 3: Quốc gia giàu có luôn hạnh phúc hơn không?  
### Giả thuyết:
GDP bình quân đầu người cao có liên quan đến mức độ hạnh phúc cao hơn, nhưng không phải là yếu tố quyết định duy nhất đến hạnh phúc của một quốc gia.

| Mã giả thuyết | Giả thuyết                                                                 | Kỳ vọng                                             |
|--------------|---------------------------------------------------------------------------|-------------------------------------------------------------------------|
| H1           | Các quốc gia có GDP cao có xu hướng hạnh phúc cao hơn                     | Tồn tại mối tương quan dương rõ ràng giữa GDP và Happiness Score        |
| H2           | GDP là yếu tố quyết định chính đến mức độ hạnh phúc                       | GDP giải thích phần lớn sự biến thiên của Happiness Score               |
| H3           | Top 10 quốc gia giàu nhất có mức độ hạnh phúc tương đối đồng đều          | Các điểm dữ liệu tập trung, ít phân tán trên biểu đồ                    |

<img width="513" height="335" alt="image" src="https://github.com/user-attachments/assets/f542fe03-f82f-42fb-b56e-51c442453769" />

### Kết luận:
GDP tạo nền tảng, nhưng chính yếu tố xã hội mới tạo ra sự khác biệt về hạnh phúc giữa các quốc gia.

# Phân tích 4: Yếu tố nào ảnh hưởng mạnh nhất đến hạnh phúc?
### Giả thuyết:
| Indicator        | Giả thuyết                                                                 | Kỳ vọng                                                                                       |
|------------------|---------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| GDP              | GDP cao sẽ làm tăng mức độ hạnh phúc                                       | Các quốc gia có GDP cao sẽ có Happiness Score cao hơn                                        |
| Social Support   | Hỗ trợ xã hội là yếu tố quan trọng ảnh hưởng đến hạnh phúc                 | Quốc gia có social support cao sẽ có mức hạnh phúc cao hơn                                   |
| Health           | Sức khỏe và tuổi thọ cao góp phần nâng cao mức độ hạnh phúc                | Quốc gia có life expectancy cao sẽ có Happiness Score cao                                    |
| Freedom          | Tự do cá nhân có tác động tích cực đến mức độ hạnh phúc                    | Quốc gia có mức độ tự do cao sẽ có Happiness Score cao                                       |
| Trust (Corruption)| Mức độ minh bạch cao (ít tham nhũng) giúp tăng mức độ hạnh phúc            | Quốc gia có mức độ tham nhũng thấp sẽ có Happiness Score cao                                 |
| Generosity       | Sự hào phóng có liên quan tích cực đến hạnh phúc                           | Quốc gia có generosity cao sẽ có Happiness Score cao                                         |

<img width="911" height="527" alt="image" src="https://github.com/user-attachments/assets/ae3dc71b-1983-4d5a-aee1-44e0c231977e" />

### Kết luận: 
Kinh tế tạo nền tảng cho hạnh phúc, nhưng chính yếu tố xã hội và sức khỏe mới quyết định sự bền vững của hạnh phúc.

# Phân tích 5: Mức độ chênh lệch hạnh phúc giữa các quốc gia có đang thu hẹp hay gia tăng theo thời gian?




