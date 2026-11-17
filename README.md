# 🎓 Phân tích và điều chỉnh tư thế ngồi bằng Mediapipe ứng dụng AIoT

<div align="center">

<p align="center" dir="auto">
  <a target="_blank" rel="noopener noreferrer" href=""><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d3/Logo_DAI_NAM.png/1200px-Logo_DAI_NAM.png" alt="DaiNam University Logo" width="200" style="max-width: 100%;"></a>
  <a target="_blank" rel="noopener noreferrer" href=""><img src="https://raw.githubusercontent.com/drkhanusa/DNU_PlagiarismChecker/main/docs/images/AIoTLab_logo.png" alt="AIoTLab Logo" width="170" style="max-width: 100%;"></a>
</p>
<p dir="auto"><a href="https://fit.dainam.edu.vn" rel="nofollow"><img src="https://camo.githubusercontent.com/14375b31490acab17dd414aef749f3c109a82abaeae50592667c9955b79ce09a/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4d616465253230627925323041496f544c61622d626c75653f7374796c653d666f722d7468652d6261646765" alt="Made by AIoTLab" data-canonical-src="https://img.shields.io/badge/Made%20by%20AIoTLab-blue?style=for-the-badge" style="max-width: 100%;"></a>
<a href="https://fit.dainam.edu.vn" rel="nofollow"><img src="https://camo.githubusercontent.com/f33b9e36f6d7e3878c31898033ff8514d824d4f51d8cab187bf3eddc84e2a99e/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f466163756c74792532306f66253230496e666f726d6174696f6e253230546563686e6f6c6f67792d677265656e3f7374796c653d666f722d7468652d6261646765" alt="Faculty of IT" data-canonical-src="https://img.shields.io/badge/Faculty%20of%20Information%20Technology-green?style=for-the-badge" style="max-width: 100%;"></a>
<a href="https://dainam.edu.vn" rel="nofollow"><img src="https://camo.githubusercontent.com/b503f479f429296dbff6eb7e1e583a962657044af1feb98e6dfc4a68a106a49e/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4461694e616d253230556e69766572736974792d7265643f7374796c653d666f722d7468652d6261646765" alt="DaiNam University" data-canonical-src="https://img.shields.io/badge/DaiNam%20University-red?style=for-the-badge" style="max-width: 100%;"></a></p>
</div>

<p align="center">
  <a href="#-architecture">Kiến trúc hệ thống</a> •
  <a href="#-key-features">Tính năng</a> •
  <a href="#-tech-stack">Công cụ</a> •
  <a href="#-installation">Cài đặt</a> •
  <a href="#-getting-started">Triển khai</a> •
  <a href="#-documentation">Video hướng dẫn chi tiết</a>
</p>

## 🏗️ Kiến trúc hệ thống

<p align="center">
  <img src="Báo cáo/images/system_architecture.png" alt="System Architecture" width="800"/>
</p>

Hệ thống sử dụng kiến trúc ba lớp:

1. **📷 Camera Layer**: Thu thập dữ liệu hình ảnh từ camera theo thời gian thực.
2. **🧠 AI Processing Layer**: Phân tích tư thế ngồi bằng Mediapipe Pose và OpenCV.
3. **📊 Feedback Layer**: Hiển thị kết quả và cảnh báo thông qua giao diện web.

## ✨ Các tính năng chính

### 🧠 Công nghệ AI tiên tiến
- **Mediapipe Pose**: Phát hiện 33 điểm đặc trưng trên cơ thể với độ chính xác cao.
- **Tính toán góc nghiêng**: Xác định tư thế ngồi dựa trên góc nghiêng của cổ và lưng.
- **Cảnh báo thời gian thực**: Phản hồi ngay lập tức khi phát hiện tư thế sai.

### ⚡ Hiệu suất cao
- **Xử lý 30 FPS**: Đảm bảo phản hồi nhanh chóng và mượt mà.
- **Tối ưu hóa thuật toán**: Sử dụng lọc Kalman để ổn định dữ liệu và giảm nhiễu.

### 📊 Phân tích toàn diện
- **Hiển thị trực quan**: Giao diện web hiển thị góc nghiêng và trạng thái tư thế.
- **Lưu trữ lịch sử**: Theo dõi thời gian ngồi đúng và sai tư thế.

## 🔧 Công cụ

<div align="center">

### Công nghệ cốt lõi
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)](https://opencv.org/)
[![Mediapipe](https://img.shields.io/badge/Mediapipe-FF6F00?style=for-the-badge&logo=mediapipe&logoColor=white)](https://mediapipe.dev/)

</div>

## 📥 Cài đặt

### 🛠️ Yêu cầu tiên quyết

- 🐍 **Python** `3.8+` - Ngôn ngữ lập trình chính.
- 📦 **OpenCV** - Xử lý hình ảnh và video.
- 🧠 **Mediapipe** - Phát hiện các điểm đặc trưng trên cơ thể.
- 🌐 **Flask** - Xây dựng giao diện web và xử lý yêu cầu HTTP.

### ⚙️ Thiết lập dự án

1. 📦 **Sao chép kho lưu trữ**
   ```bash
   git clone https://github.com/dtb0405/Phan-tich-va-dieu-chinh-tu-the-ngoi-bang-Mediapipe.git
   cd Phan-tich-va-dieu-chinh-tu-the-ngoi-bang-Mediapipe
2. 📚 **Cài đặt thư viện cần thiết**
   ```bash
   pip install -r requirements.txt
3. ⚡ **Chạy ứng dụng**
   ```bash
   python app.py
4. 🌐 **Truy cập ứng dụng**

Mở trình duyệt và truy cập http://localhost:5000.
### 🚀 Triển khai
**⚡ Khởi động nhanh**
1. Khởi động hệ thống bằng lệnh:
   ```bash
   python app.py
2. Mở trình duyệt và truy cập http://localhost:5000.
3. Hệ thống sẽ hiển thị video trực tiếp từ camera và cảnh báo khi phát hiện tư thế sai.

**📝 License**

© 2025 Nhóm 5, CNTT 16-04, AIoTLab, Khoa Công nghệ Thông tin, Trường Đại học Đại Nam. 

## 🎥 Video Hướng Dẫn Chi Tiết

Để hiểu rõ hơn về cách cài đặt và sử dụng hệ thống, bạn có thể xem video hướng dẫn chi tiết dưới đây:

[![Video Hướng Dẫn](https://img.youtube.com/vi/ms6KwI8QnPs/0.jpg)](https://youtu.be/ms6KwI8QnPs)

**Nhấn vào hình ảnh để xem video trên YouTube.**

<div align="center">

Thực hiện bởi Nhóm 5 - CNTT1604, AIoTLab, Đại học Đại Nam

Website • GitHub • Contact Us

</div>
