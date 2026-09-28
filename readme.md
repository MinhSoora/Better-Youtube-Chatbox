# 🎀 Chat CSS Studio

**Chat CSS Studio** là công cụ trực quan giúp tùy chỉnh giao diện **YouTube Live Chat** để sử dụng làm **Browser Source trong OBS**.

Không cần tự viết CSS từ đầu — chỉ cần chỉnh màu sắc, kích thước, font, animation và hiệu ứng, công cụ sẽ tự động tạo CSS tương ứng để bạn sao chép vào OBS.

## 🎥 Demo

<video src="./km_20260928-2_480p_60f_20260928_211438.mp4" controls width="100%"></video>

> Video demo: `km_20260928-2_480p_60f_20260928_211438.mp4`

## ✨ Tính năng

### 🎨 Tùy chỉnh màu sắc

Có thể thay đổi trực tiếp:

* Màu name tag
* Màu chữ name tag
* Màu nền bong bóng tin nhắn
* Màu chữ tin nhắn
* Màu băng keo vàng
* Màu băng keo xanh
* Màu phần đầu Member
* Màu phần cuối Member

Các thay đổi được cập nhật ngay trên bản xem trước.

### 📐 Kích thước & chữ

Cho phép điều chỉnh:

* Cỡ chữ tin nhắn
* Cỡ chữ tên người dùng
* Kích thước avatar
* Tốc độ animation
* Font chữ

Các font được hỗ trợ:

* Quicksand
* Nunito
* Baloo 2
* Be Vietnam Pro
* Patrick Hand

### 🎞️ Animation tin nhắn

Có nhiều hiệu ứng xuất hiện cho tin nhắn:

* Trượt từ trái
* Phóng to
* Nổi lên
* Nảy xuống
* Lật
* Không có animation

Ngoài tin nhắn thông thường, **Super Chat** và **Member** cũng có animation riêng.

### 💎 Hiệu ứng Super Chat / Member

Hỗ trợ tùy chỉnh hiệu ứng cho các thông báo đặc biệt:

* Hiệu ứng nảy lên
* Phát sáng viền
* Tia sáng quét qua card
* Ruy băng chào mừng Member
* Hiệu ứng chuyển động cho ruy băng

### 👀 Preview trực tiếp

Khu vực Preview mô phỏng nhiều loại nội dung:

* Tin nhắn thông thường
* Member
* Moderator
* Channel Owner
* Super Chat
* Welcome Member

Có thể:

* Phát lại animation
* Thêm tin nhắn mới
* Đổi nền preview
* Thay đổi chiều rộng preview

Các nền preview gồm:

* Nền caro
* Nền đen
* Nền game
* Nền sáng

### 📋 Tự động tạo CSS

CSS được sinh tự động dựa trên các tùy chỉnh hiện tại.

Có thể:

1. Chỉnh giao diện.
2. Xem trước kết quả.
3. Sao chép CSS.
4. Dán trực tiếp vào Browser Source của OBS.

## 🎥 Sử dụng với OBS

### Bước 1 — Mở YouTube Live Chat

Sử dụng URL dạng:

```text
https://www.youtube.com/live_chat?is_popout=1&v=ID_LIVESTREAM
```

Thay `ID_LIVESTREAM` bằng ID livestream YouTube của bạn.

### Bước 2 — Thêm Browser Source

Trong OBS:

```text
Sources
→ Browser
→ URL
```

Nhập URL YouTube Live Chat Popout.

### Bước 3 — Thêm Custom CSS

Mở **Chat CSS Studio**, tùy chỉnh giao diện theo ý muốn.

Sau đó:

```text
CSS cho Browser Source
→ Sao chép CSS
```

Dán CSS vào:

```text
OBS
→ Browser Source
→ Custom CSS
```

### Bước 4 — Điều chỉnh kích thước

Điều chỉnh kích thước Browser Source trong OBS sao cho phù hợp với layout livestream.

## 🖥️ Chạy Chat CSS Studio

Đây là một trang HTML độc lập nên không yêu cầu backend.

Chỉ cần mở:

```text
index.html
```

bằng trình duyệt.

Cấu trúc tối thiểu:

```text
Chat-CSS-Studio/
├── index.html
├── README.md
└── km_20260928-2_480p_60f_20260928_211438.mp4
```

## 🧩 Công nghệ

Dự án sử dụng:

* HTML5
* CSS3
* JavaScript
* CSS Custom Properties
* CSS Keyframes Animation
* Google Fonts
* YouTube Live Chat DOM selectors

Không sử dụng framework hoặc backend.

## ⚙️ Cơ chế hoạt động

Chat CSS Studio có hai phần chính:

```text
Giao diện tùy chỉnh
       ↓
JavaScript lưu cấu hình
       ↓
CSS Generator
       ↓
CSS Preview
       ↓
CSS cho Browser Source
       ↓
YouTube Live Chat + OBS
```

Các thiết lập được lưu trong object JavaScript `S`.

Ví dụ:

```javascript
{
    tag: '#f2799f',
    bubble: '#ffffff',
    bubbleText: '#1e1e1e',
    msg: 15,
    name: 12.5,
    ava: 44,
    dur: 0.5,
    font: 'Quicksand',
    anim: 'slide',
    sc: 'pop'
}
```

## 🔄 Đặt lại cấu hình

Nút **Đặt lại** sẽ đưa toàn bộ tùy chỉnh về cấu hình mặc định.

Cấu hình mặc định bao gồm:

* Font: `Quicksand`
* Animation tin nhắn: `slide`
* Animation Super Chat / Member: `pop`
* Phát sáng viền: bật
* Tia sáng quét: bật
* Cỡ chữ tin nhắn: `15px`
* Cỡ chữ tên: `12.5px`
* Avatar: `44px`

## 🎀 Phong cách giao diện

Chat CSS Studio sử dụng phong cách:

```text
Cute
Pastel
Scrapbook
Paper / Sticker
Rounded
Colorful
```

Tin nhắn được thiết kế giống các mảnh giấy/sticker với:

* Name tag
* Băng keo trang trí
* Avatar dạng polaroid
* Bong bóng chat
* Shadow
* Animation
* Hiệu ứng Super Chat

## 📱 Responsive

Giao diện hỗ trợ màn hình nhỏ.

Khi chiều rộng màn hình giảm xuống, khu vực tùy chỉnh và Preview sẽ chuyển từ layout hai cột sang một cột.

```css
@media(max-width:860px) {
    main {
        grid-template-columns: 1fr;
    }
}
```

## ⚠️ Lưu ý

CSS được tạo dựa trên cấu trúc DOM của **YouTube Live Chat**.

Nếu YouTube thay đổi cấu trúc HTML hoặc tên các phần tử của Live Chat, một số selector CSS có thể cần được cập nhật.

Một số hiệu ứng chỉ áp dụng khi Browser Source thực sự tải được các phần tử tương ứng của YouTube Live Chat.

## 📄 License

Bạn có thể tự quyết định license phù hợp nếu phát hành dự án công khai.

---

**Chat CSS Studio**
*Customize your YouTube Live Chat for OBS — without writing CSS manually.*
