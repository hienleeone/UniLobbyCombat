<div align="center">

# ⚔️ UNILOBBYCOMBAT
### *Next-Generation Lobby PvP, Weapon Skills & Combat-Tag Engine*

[![Minecraft](https://img.shields.io/badge/Minecraft-1.21.4%2B-55FF55?style=for-the-badge&logo=minecraft&logoColor=white)](https://papermc.io)
[![Engine](https://img.shields.io/badge/Engine-Paper%20%7C%20Purpur%20%7C%20Leaf-00F5D4?style=for-the-badge)](https://papermc.io)
[![Database](https://img.shields.io/badge/Storage-Async%20SQLite%20%7C%20YAML-FFA502?style=for-the-badge)](https://sqlite.org)
[![Security](https://img.shields.io/badge/Anti--Dupe-PDC%20SafeGuard-FF4757?style=for-the-badge)](https://github.com)
[![Java](https://img.shields.io/badge/Java-21%2B-blueviolet?style=for-the-badge&logo=openjdk&logoColor=white)](https://www.oracle.com/java/)

<br/>

**UniLobbyCombat** là giải pháp đấu trường PvP sảnh cao cấp toàn diện dành cho máy chủ Minecraft hiện đại.  
Được phát triển với mục tiêu **"PvP Công Bằng — Kỹ Năng Đỉnh Cao — Chống Gian Lận Tuyệt Đối"**, plugin biến khu vực sảnh chờ (Lobby/Hub) thành một đấu trường chiến đấu sống động, lôi cuốn người chơi giải trí trong lúc chờ đợi.

[Tính Năng](#-tại-sao-unilobbycombat-vượt-trội) • [Hệ Thống Kỹ Năng](#-hệ-thống-kỹ-năng-vũ-khí-rpg) • [Lệnh & Quyền](#-lệnh--quyền-hạn) • [Placeholders](#-placeholderapi-tích-hợp) • [Cài Đặt Nhanh](#-cài-đặt-trong-30-giây)

---

</div>

## ⚡ Tại Sao UniLobbyCombat Vượt Trội?

```yaml
  🛡️ Cách Ly Tuyệt Đối   ── Chỉ người cùng bật PvP mới tương tác sát thương với nhau.
  🔒 PDC SafeGuard       ── Sao lưu 100% túi đồ gốc, gắn thẻ PDC chống trộm/dupe giáp.
  💥 Kỹ Năng RPG 3D      ── Tích hợp chiêu thức Khí Trảm & Hộ Thể ngay trên thanh kiếm.
  🚫 Anti-Combat Log     ── Khóa lệnh bay/teleport/NPC, xử tử kẻ trốn chạy khi đang giao tranh.
  ⚡ SQLite Async Engine ── Lưu trữ Kills/Deaths/Streak ngầm, bảng xếp hạng Top O(1).
  🎁 Mốc Thưởng Streak   ── Tự động phát quà & vinh danh toàn server khi đạt chuỗi hạ gục.
```

---

## 💎 Điểm Nhấn Tính Năng

### 1. ⚔️ Cơ Chế Giao Tranh Công Bằng (Isolated Combat Logic)
* **Người chơi tự do tham gia:** Người chơi mới vào sảnh nhận ngay Kiếm Chiến Đấu hoặc gõ `/pvp` để tham chiến mà **không cần cấu hình quyền phức tạp**.
* **Bảo vệ người xem:** Người chơi chưa bật PvP **hoàn toàn bất tử** trước mọi đòn đánh cận chiến, cung tên, đinh ba hoặc bình thuốc từ người đang giao tranh.
* **Bộ đếm thời gian an toàn:** Có âm thanh và tiêu đề đếm ngược khi bật/tắt để chống lạm dụng bật tắt liên tục né sát thương.

---

### 2. 🪄 Hệ Thống Kỹ Năng Vũ Khí RPG (Weapon Skills)
Tăng tính kịch tính cho các trận solo tại sảnh với 2 kỹ năng độc quyền:

<table>
<tr>
<td width="50%">

#### 🗡️ Kỹ Năng Tấn Công: Khí Trảm
*Thao tác: `Shift + Chuột Phải` kiếm chiến đấu*
- 💥 Phóng luồng kiếm khí tầm xa gây **3 tim sát thương**.
- 💫 Hiệu ứng hạt quét kiếm chém (*Sweep/Sonic*) & âm thanh uy lực.
- ⏳ Thời gian hồi chiêu độc lập với thông báo trên thanh Actionbar.

</td>
<td width="50%">

#### 💖 Kỹ Năng Hồi Phục: Hộ Thể
*Thao tác: `Shift + Chuột Trái` kiếm chiến đấu*
- 🌿 Hồi phục ngay **3 tim máu** & nhận hiệu ứng Hồi Máu (*Regeneration*).
- ✨ Hào quang trái tim và hạt hào quang bảo hộ quanh thân.
- ⏳ Hỗ trợ người chơi lật ngược tình thế trong các pha giao tranh nghẹt thở.

</td>
</tr>
</table>

---

### 3. 🔐 Bảo Vệ Túi Đồ & Chống Trốn Chạy (SafeGuard & Anti-Log)

* 🎒 **Zero Data Loss (Khôi phục túi đồ gốc 100%):**
  * Tự động cất túi đồ cá nhân vào bộ nhớ an toàn trước khi phát Set Giáp Kim Cương và Kiếm Chiến Đấu.
  * Khi rời PvP, bị hạ gục hoặc server tắt/reload ➔ Túi đồ ban đầu được hoàn trả nguyên vẹn tức thì.
* 🚫 **Chặn Dupe & Di Chuyển Đồ (PDC Locked):**
  * Trang bị chiến đấu bị khóa cứng trên người, không thể cất vào rương, không thể vứt ra đất.
* ⚡ **Chặn Lệnh Thông Minh (Command Whitelist):**
  * Tự động chặn các lệnh chuyển server, dịch chuyển (`/tp`, `/spawn`, `/menu`, `/server`) và chặn click vào NPC khi đang bật PvP hoặc bị gắn thẻ Combat Tag.
* ☠️ **Xử Tử Kẻ Thoát Game:**
  * Người chơi cố tình ngắt kết nối khi đang bị Combat Tag sẽ bị xử tử ngay lập tức, tính điểm Kill và Killstreak cho đối thủ vừa tấn công.

---

## 🎮 Lệnh & Quyền Hạn

### 👤 Người Chơi *(Mặc định ai cũng dùng được)*
| Lệnh | Mô Tả |
| :--- | :--- |
| `/pvp` *(hoặc `/pvp toggle`)* | Bật / Tắt trạng thái chiến đấu |
| `/pvp on` / `/pvp off` | Kích hoạt bộ đếm ngược bật/tắt PvP |
| `/pvp stats [player]` | Xem bảng thống kê Kills, Deaths, KDR, Chuỗi mạng |
| `/pvp top [kills/streak]` | Xem Bảng Xếp Hạng Top 10 cao thủ sảnh |

### 🛠️ Quản Trị Viên *(Quyền: `unilobbycombat.admin` hoặc `OP`)*
| Lệnh | Mô Tả |
| :--- | :--- |
| `/unilobbycombat reload` | Tải lại cấu hình `config.yml` tức thì |
| `/unilobbycombat toggle <player>` | Ép bật/tắt chế độ PvP cho người chơi |
| `/unilobbycombat give <player>` | Phát lại kiếm chiến đấu cho người chơi |
| `/unilobbycombat reset <player>` | Đặt lại toàn bộ chỉ số chiến đấu của người chơi |
| `/unilobbycombat setkills <player> <số>` | Chỉnh sửa số mạng hạ gục |
| `/unilobbycombat setstreak <player> <số>` | Chỉnh sửa chuỗi mạng hạ gục |

---

## 📊 PlaceholderAPI Tích Hợp

> Tương thích $100\%$ với **TAB, Scoreboard, Holograms, DeluxeMenus**. Hỗ trợ cả định dạng mới `%unilobbycombat_*%` và định dạng cũ `%hubpvp_*%`:

| Placeholder | Mô Tả Dữ Liệu |
| :--- | :--- |
| `%unilobbycombat_status%` | Trạng thái chiến đấu (`Bật` / `Tắt`) |
| `%unilobbycombat_status_color%` | Mã màu trạng thái (`&a` hoặc `&c`) |
| `%unilobbycombat_kills%` | Tổng số mạng đã hạ gục |
| `%unilobbycombat_deaths%` | Tổng số lần bị hạ gục |
| `%unilobbycombat_kdr%` | Tỉ lệ mạng hạ/chết (K/D Ratio) |
| `%unilobbycombat_killstreak%` | Chuỗi hạ gục hiện tại |
| `%unilobbycombat_best_streak%` | Kỷ lục chuỗi hạ gục cao nhất |
| `%unilobbycombat_combattime%` | Thời gian Combat Tag còn lại (giây) |
| `%unilobbycombat_top_<1-10>_name%` | Tên người chơi Top 1 đến Top 10 |
| `%unilobbycombat_top_<1-10>_kills%` | Số kill của người chơi Top X |
| `%unilobbycombat_top_<1-10>_streak%` | Chuỗi cao nhất của người chơi Top X |

---

## 🚀 Cài Đặt Trong 30 Giây

1. Thả `UniLobbyCombat.jar` vào thư mục `/plugins/`.
2. Khởi động server (Hỗ trợ **Paper/Purpur/Leaf 1.21.4+**, **Java 21+**).
3. Đã sẵn sàng! Người chơi vào server sẽ tự động nhận kiếm chiến đấu ở Slot 0 và có thể nhấp chuột phải để tham chiến ngay!

---

<div align="center">

**UniLobbyCombat — Nâng Tầm Trải Nghiệm Đấu Trường Sảnh Cho Máy Chủ Của Bạn!**

*Được phát triển bởi **hienleeone** cho hệ thống UniSky Network.*

</div>
