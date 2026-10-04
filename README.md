# 🎮 Roblox Skills (Tiếng Việt) cho Claude

Bộ **skill** giúp Claude hỗ trợ làm game Roblox: từ ý tưởng, chọn model 3D, dựng giao diện, viết code Luau đến kiểm tra map trước khi publish. Các skill trả lời bằng **tiếng Việt** (tên thuộc tính, class, Enum và từ khóa tìm kiếm giữ tiếng Anh).

> Mỗi skill là một thư mục chứa file `SKILL.md` (và các file tham chiếu đi kèm). Claude tự đọc skill khi yêu cầu của bạn khớp với mô tả của skill đó.

---

## 📦 Danh sách skill

| Skill | Dùng khi nào |
|---|---|
| [`roblox-game`](./roblox-game) | Trợ lý tổng quát để làm game Roblox: Luau, Roblox Studio, MCP, game design, bảo mật, tối ưu hiệu năng. |
| [`roblox-luau-genres`](./roblox-luau-genres) | Viết code Luau gọn, chạy được cho vòng lặp gameplay cốt lõi của từng thể loại (Simulator, Tycoon, Horror, RPG, FPS, Obby, Sci-Fi, Anime/Fighting), kèm lưu dữ liệu và RemoteEvent. |
| [`roblox-ui-designer`](./roblox-ui-designer) | Tư vấn và dựng GUI (HUD, Shop, Inventory, Pop-up): bảng màu HEX, font, UICorner/UIStroke, bố cục responsive cho Mobile/PC/Console, hiệu ứng TweenService. |
| [`roblox-art-director`](./roblox-art-director) | Chọn art style, danh sách model, từ khóa Toolbox, tối ưu và kiểm tra virus/backdoor cho free model theo thể loại game. |
| [`roblox-3d-model-selector`](./roblox-3d-model-selector) | Chọn, đánh giá và tối ưu model 3D, asset hình ảnh cho từng thể loại trong Roblox Studio. |
| [`roblox-map-qa`](./roblox-map-qa) | Kiểm tra chất lượng map: chỗ ra khỏi map, part đè nhau/z-fighting, spawn bị che, lỗi riêng từng thể loại, script theo dõi lỗi khi playtest. |

---

## 🚀 Cách cài đặt

1. **Tải repo về:** bấm **Code → Download ZIP** rồi giải nén, hoặc dùng Git:
   ```bash
   git clone https://github.com/duyquanvudinh-lang/roblox-skill-vietnamese.git
   ```
2. **Chọn skill cần dùng** (ví dụ `roblox-ui-designer`) và nén **riêng thư mục đó** thành file `.zip`. Bên trong file zip, `SKILL.md` phải nằm trong thư mục skill.
3. **Tải lên Claude:** mở phần **Customize → Skills** trong Claude và thêm file `.zip` vừa tạo. Kiểm tra skill đã được bật (công tắc ở trạng thái bật).

> Tên và vị trí nút tải lên có thể thay đổi theo phiên bản giao diện, hãy xem hướng dẫn mới nhất của Claude nếu không thấy.

---

## 💡 Ví dụ cách dùng

Sau khi bật skill, chỉ cần mô tả việc bạn muốn, không cần gọi tên skill:

- *"Làm cái shop cho game simulator"* → `roblox-ui-designer`
- *"Làm quái đuổi người trong game horror"* → `roblox-luau-genres`
- *"Tôi đang làm game horror, nên dùng model gì?"* → `roblox-art-director`
- *"Kiểm tra map giúp mình có chỗ nào người chơi rơi ra ngoài không"* → `roblox-map-qa`

---

## 🗂️ Cấu trúc repo

```
roblox-skill-vietnamese/
├── README.md
├── roblox-game/
│   └── SKILL.md
├── roblox-luau-genres/
│   └── SKILL.md
├── roblox-ui-designer/
│   ├── SKILL.md
│   └── references/
├── roblox-art-director/
│   └── SKILL.md
├── roblox-3d-model-selector/
│   └── SKILL.md
└── roblox-map-qa/
    └── SKILL.md
```

---

## 🤝 Đóng góp

Góp ý hoặc sửa lỗi đều được hoan nghênh: mở **Issue** để báo lỗi/đề xuất, hoặc gửi **Pull Request** với thay đổi của bạn. Khi thêm skill mới, hãy tạo một thư mục riêng có file `SKILL.md` với phần mô tả (`description`) nêu rõ khi nào skill nên được dùng.

## 📄 Giấy phép

Xem file `LICENSE` trong repo (nếu có).
