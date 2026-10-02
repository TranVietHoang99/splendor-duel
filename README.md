# 💎 Splendor Duel

Game **Splendor Duel** (Marc André & Bruno Cathala, Space Cowboys) cho 2 người, chơi ngay trên trình duyệt: lấy đá quý trên bàn 5×5, mua lá trang sức, gom vương miện và điểm uy tín.

Chơi online: https://tranviethoang99.github.io/splendor-duel/

## Chế độ chơi
- **Chơi với máy**: nhập tên, bấm *Chơi với máy*.
- **Online 1 đấu 1**: bấm *Tạo phòng*, gửi mã hoặc link cho bạn bè; bạn bè nhập mã và bấm *Vào phòng*.
  Người tạo phòng phải **giữ tab mở**, vì máy chủ phòng giữ trạng thái ván chơi.

## Luật tóm tắt
- 25 viên: 4 viên mỗi màu (trắng, lam, lục, đỏ, đen), 2 ngọc trai, 3 vàng (vàng thay được mọi loại khi trả).
- **Thắng ngay cuối lượt** nếu đạt: 20 điểm uy tín, **hoặc** 10 vương miện, **hoặc** 10 điểm trên các lá cùng một màu.
- Tuỳ chọn trước hành động chính: dùng đặc quyền (lấy 1 viên bất kỳ, không phải vàng); bổ sung bàn (đối thủ nhận 1 đặc quyền).
- Hành động chính (chọn 1):
  - lấy tới 3 viên liền nhau trên một đường thẳng (3 viên cùng màu hoặc 2 ngọc trai → đối thủ nhận 1 đặc quyền);
  - lấy 1 vàng và giữ 1 lá (tối đa 3 lá);
  - mua 1 lá. Lá màu đã mua giảm giá vĩnh viễn màu đó.
- Khả năng của lá: thêm lượt, lấy thêm 1 viên cùng màu, nhận đặc quyền, cướp 1 viên của đối thủ, lá đa sắc.
- Đạt 3 và 6 vương miện: nhận lá hoàng gia. Cuối lượt giữ tối đa 10 viên.

Bộ 67 lá bài và 4 lá hoàng gia lấy theo bản chính thức.

## Kỹ thuật
Một file `index.html` duy nhất. Kết nối P2P bằng [PeerJS](https://peerjs.com/), cùng khung với Azul, Jaipur và 7 Wonders Duel.
Chạy thử: `npx http-server splendor-duel -p 5185`.
