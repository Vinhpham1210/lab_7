# 🦁 Lab 7: Computer Vision Model Zoo for AIoT

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![FastAPI](https://img.shields.io/badge/FastAPI-0.100+-009688.svg)
![YOLO](https://img.shields.io/badge/YOLOv8-Ultralytics-FF5722.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-5C3EE8.svg)

Dự án này là bài thực hành mở rộng nhằm trải nghiệm đa dạng các mô hình Thị giác máy tính (Computer Vision). Thay vì chỉ giới hạn ở Object Detection (YOLO), hệ thống cung cấp một "Model Zoo" cho phép thử nghiệm nhiều dạng output khác nhau, từ đó lựa chọn công nghệ phù hợp nhất cho các hệ thống AIoT thực tế.

---

## 🎯 Các nhóm mô hình hỗ trợ (Model Zoo)

Hệ thống hỗ trợ xử lý linh hoạt nhiều bài toán CV khác nhau:

| Nhóm Model | Output chính | Ứng dụng trong AIoT |
| :--- | :--- | :--- |
| **YOLO Detection** | Bounding box, Class, Confidence | Nhận diện và định vị vật thể |
| **Tracking / Counting** | Object ID, Centroid, Count | Theo dõi quỹ đạo, đếm người/vật qua vạch |
| **Pose Landmark** | Body landmarks | Phân tích tư thế, phát hiện té ngã |
| **Hand / Gesture** | Hand landmarks, Gesture label | Điều khiển thiết bị bằng cử chỉ tay |
| **Face Landmark** | Face landmarks, Attention cue | Đánh giá trạng thái khuôn mặt (buồn ngủ, chú ý) |
| **OCR** | Text, Bbox, Confidence | Nhận diện chữ (biển số xe, mã vận đơn) |
| **Segmentation** | Mask, Mask area, Bbox | Đo diện tích vùng lỗi, phân tích ảnh y tế/nông nghiệp |
| **OpenCV Motion** | Motion area, Bbox | Cảnh báo chuyển động nhẹ, tối ưu tài nguyên tính toán |

---

## ⚙️ Hướng dẫn cài đặt & Khởi chạy

### 1. Cài đặt môi trường

```bash
# Tạo và kích hoạt môi trường ảo
python -m venv .venv

# Windows:
.\.venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

# Cài đặt thư viện cốt lõi
pip install -r requirements_core.txt
