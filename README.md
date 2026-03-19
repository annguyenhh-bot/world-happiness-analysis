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

1. Quốc gia nào có mức độ hạnh phúc cao nhất?  
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

---

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

