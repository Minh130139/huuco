# <span style="color: #4CAF50;">🌱 Nông nghiệp Hữu Cơ</span>

[![Netlify Status](https://img.shields.io/badge/Netlify-Deployed-00C58E?logo=netlify)](https://your-app.netlify.app)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Ứng dụng web cung cấp hướng dẫn chi tiết về nông nghiệp hữu cơ cho người mới bắt đầu với các tính năng thông minh: lịch chăm sóc cá nhân hóa, công thức phân bón tự nhiên, và quản lý nội dung dễ dàng qua Netlify CMS.

## ✨ Tính năng chính

### 🌿 **Lịch chăm sóc cây trồng**
- 📅 Lịch trình chi tiết cho 7 loại cây phổ biến
- 🎯 Thời vụ phù hợp cho từng cây trồng
- 📝 Ghi chú cá nhân hóa
- 📊 Theo dõi tiến độ trồng trọt

### 🧪 **Công thức hữu cơ tự làm**
- 🌱 Phân bón lỏng hữu cơ (FAA, BAA, EM)
- 🦠 Vi sinh vật có ích
- 🧫 Canxi, vi lượng từ nguyên liệu tự nhiên
- 🌿 Thuốc bảo vệ thực vật thảo mộc

### 📚 **Kiến thức cơ bản**
- 🗺️ Chiếu dẫn về đất và pH
- 🪱 Quản lý vi sinh vật và đất
- 🦟 Thu hút thiên địch (bọ rùa, ong ký sinh)
- 🧫 Phân compost đa dạng (nóng, lạnh, Bokashi, giun)

### 🧮 **Máy tính nông nghiệp**
- 📏 Tính diện tích và mật độ trồng
- 🚰 Ước tính nước tưới
- 💰 Dự toán phân bón và chi phí

## 🚀 Cách sử dụng

### 📲 Truy cập trực tiếp
Website được host trên Netlify, bạn có thể truy cập ngay tại: [https://your-app-name.netlify.app](https://your-app-name.netlify.app)

### 🛠️ Chạy local (nhà phát triển)
```bash
# Clone repository
git clone https://github.com/your-username/nong.git
cd nong

# Mở file index.html bằng trình duyệt
# Đây là static HTML + React, không cần server
```
✨ Không cần cài đặt dependency phức tạp - chỉ cần mở file index.html!

## 📁 Cấu trúc project

```
nong/
├── index.html              # Ứng dụng chính (HTML + React)
├── admin/
│   ├── index.html         # Panel quản trị Netlify CMS
│   └── config.yml         # Cấu hình CMS
├── content/
│   ├── crops/             # Bài viết về cây trồng (Markdown)
│   ├── formulas/          # Công thức phân bón (Markdown)
│   ├── tips/              # Mẹo hữu ích (Markdown)
│   └── settings/          # Cài đặt CMS
├── static/
│   ├── netlify.toml       # Cấu hình Netlify
│   └── images/            # Hình ảnh upload
└── README.md             # Tài liệu này
```

## 🛠️ Công nghệ sử dụng

- **Frontend**: HTML5, React 18, Tailwind CSS, Lucide Icons
- **CMS**: Netlify CMS - Quản lý nội dung trực quan
- **Deployment**: Netlify - Auto-deploy từ GitHub
- **Hosting**: GitHub Pages hoặc Netlify

## ⚙️ Setup và triển khai

### 1. 🌐 Tạo repository GitHub
```bash
# Đảm bảo bạn đã có GitHub account
# Tạo repository mới tên "nong" hoặc tên bạn thích
```

### 2. 🚀 Deploy lên Netlify

#### Cách 1: Từ GitHub (Khuyến nghị)
1. 🌱 **Push code lên GitHub**:
   ```bash
   git add .
   git commit -m "Initial commit: Nong nghiep huu co app"
   git branch -M main
   git remote add origin https://github.com/your-username/nong.git
   git push -u origin main
   ```

2. 🏗️ **Kết nối Netlify**:
   - Truy cập [netlify.com](https://netlify.com) và đăng nhập
   - Click "New site from Git"
   - Chọn GitHub repository vừa tạo
   - Netlify sẽ tự động detect cấu hình từ `netlify.toml`
   - Deploy! Website sẽ có tại: `https://random-name.netlify.app`

#### Cách 2: Direct upload (Một lần)
1. 📦 Nén toàn bộ thư mục thành ZIP
2. 🖱️ Upload lên [app.netlify.com/drop](https://app.netlify.com/drop)
3. 🎉 Website hoạt động ngay!

### 3. 🛡️ Cấu hình Netlify CMS
1. 📝 Tạo repo GitHub private mới tên `nong-admin`
2. 🔗 Kết nối với Git phát triển chính
3. 🆔 Enable [Netlify Identity](https://docs.netlify.com/security/secure-access-to-sites/post-processing/)
4. 👤 Cài đặt `netlify-identity-widget`

## 📊 Cấu hình Netlify CMS

### Tiêu đề: Content Manager
### Collections: Crops (Cây trồng), Formulas (Công thức), Tips (Mẹo)
### Admin: `/admin` endpoint

## 📈 Lộ trình phát triển

- [x] 🌱 Cây trồng & lịch chăm sóc
- [x] 🧪 Công thức hữu cơ
- [x] 📚 Kiến thức nông nghiệp
- [x] 🧮 Máy tính nông nghiệp
- [x] 🗄️ Netlify CMS integration
- [ ] 🌍 Đa ngôn ngữ (Tiếng Anh)
- [ ] 📱 PWA (Progressive Web App)
- [ ] 📊 Biểu đồ tiến độ chi tiết
- [ ] 🔔 Thông báo lịch chăm sóc
- [ ] 🔗 API kết nối với ứng dụng mobile

## 🤝 Đóng góp

Chúng tôi luôn chào đón các đóng góp!

### Cách đóng góp:
1. 🍴 Fork project này
2. 🌿 Tạo branch tính năng: `git checkout -b feature/TenTinhNang`
3. 📝 Commit changes: `git commit -m 'Add ten tinh nang'`
4. ⬆️ Push lên branch: `git push origin feature/TenTinhNang`
5. 🔄 Tạo Pull Request

### Hình thức đóng góp:
- 🐛 Báo lỗi và đề xuất cải thiện
- 📖 Viết và bổ sung tài liệu
- 🌿 Thêm nội dung cây trồng mới
- 🔬 Nghiên cứu và bổ sung công thức
- 🌍 Dịch thuật sang ngôn ngữ khác

## 📞 Liên hệ

- 👤 **Tác giả**: Minh Lee
- 📧 **Email**: your.email@example.com
- 📱 **Facebook**: [fb.com/your-profile](https://facebook.com/your-profile)
- 💼 **LinkedIn**: [linkedin.com/in/your-profile](https://linkedin.com/in/your-profile)

## 📜 Giấy phép

Dự án này được phân phối theo giấy phép MIT - xem file [LICENSE](LICENSE) để biết chi tiết.

---

<div align="center">

🇻🇳 **Made with ❤️ in 🇻🇳 Việt Nam**

⭐ Nếu project này hữu ích, hãy cho chúng tôi một star!

</div>
