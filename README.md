# Hand Gesture Particle System

Một ứng dụng web tương tác sử dụng thị giác máy tính (Computer Vision) và hệ thống hạt 3D để trực quan hóa các cử chỉ tay và giọng nói. Dự án này kết hợp **Three.js** cho đồ họa 3D và **MediaPipe Hands** để theo dõi chuyển động tay theo thời gian thực.

## 🌟 Tính năng

- **Theo dõi tay thời gian thực**: Sử dụng webcam để phát hiện bàn tay và ngón tay với độ trễ thấp.
- **Hệ thống hạt 3D (Particle System)**: Hàng ngàn hạt ánh sáng tạo thành các chữ cái và hiệu ứng hình ảnh đẹp mắt.
- **Điều khiển bằng cử chỉ**:
  - ☝️ **1 Ngón**: Hiển thị chữ "I"
  - ✌️ **2 Ngón**: Hiển thị chữ "LOVE"
  - 🤟 **3 Ngón**: Hiển thị chữ "YOU"
  - ✋ **4 Ngón**: Hiển thị trọn vẹn "I LOVE YOU"
  - ✊ **Nắm tay (Fist)**: Thu nhỏ/Co cụm các hạt lại.
  - 👋 **Mở tay**: Phân tán các hạt ra xung quanh.
- **Chế độ Giọng nói (Voice Mode)**: Nói bất kỳ từ nào để các hạt tự động xếp thành chữ đó (Hỗ trợ tiếng Anh).
- **Tương tác Vật lý**: Dùng tay để "chạm" và đẩy các hạt bay ra xa.
- **Giao diện tùy biến**: Cửa sổ camera có thể kéo thả và thay đổi kích thước.

## 🛠️ Công nghệ sử dụng

- **Vite**: Build tool nhanh chóng và nhẹ.
- **Three.js**: Thư viện 3D JavaScript mạnh mẽ.
- **MediaPipe Hands**: Giải pháp theo dõi tay của Google.
- **Web Speech API**: Nhận dạng giọng nói trực tiếp trên trình duyệt.

## 🚀 Cài đặt và Chạy dự án

Yêu cầu: Đã cài đặt [Node.js](https://nodejs.org/).

1. **Cài đặt các gói phụ thuộc:**
   ```bash
   npm install
   ```

2. **Chạy dự án ở môi trường development:**
   ```bash
   npm run dev
   ```

3. **Mở trình duyệt:**
   Truy cập đường dẫn hiển thị trong terminal (thường là `http://localhost:3000`).
   *Lưu ý: Hãy cấp quyền truy cập Camera và Microphone khi được hỏi để ứng dụng hoạt động.*

## 📝 Hướng dẫn sử dụng

1. **Khởi động**: Đợi hệ thống tải và cấp quyền Camera.
2. **Điều khiển**:
   - Đưa tay lên trước camera.
   - Giơ số ngón tay tương ứng để thay đổi chữ.
   - Di chuyển tay qua các hạt để thấy hiệu ứng tương tác.
3. **Voice Mode**:
   - Nhấn nút "Enable Voice Mode" trên giao diện.
   - Nói to rõ ràng một từ tiếng Anh (ví dụ: "HELLO", "WORLD").
