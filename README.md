# Smart Meal Tracker

Ứng dụng phân loại món ăn và tính dinh dưỡng trên di động.

- NL1 (CT271): phân loại món ăn on-device, so sánh ResNet-50 và ViT-B/16 trên 30VNFoods.
- NL2 (CT466): nhận diện thành phần cơm tấm và phở bò, ước lượng khẩu phần (YOLO26-seg trên server).

## Cấu trúc
- `app/` Flutter (dùng chung)
- `classification/` huấn luyện phân loại (NL1)
- `segmentation/` gán nhãn và huấn luyện phân vùng (NL2)
- `server/` backend FastAPI + SQLite (NL2)
- `evaluation/` đo sai số khối lượng, năng lượng (NL2)
- `docs/` báo cáo
- `data/` dữ liệu (không đưa lên git)