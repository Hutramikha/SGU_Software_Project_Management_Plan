# 📚 Dự Án Quản Lý Phát Triển Website Bán Sách Trực Tuyến (Fahasa Marketplace Model)
  
> **Mã dự án (Project Code):** `BOOK_MP_SWPM_2025`  
> **Mã tài liệu (Document Code):** `BOOK_MP_SWPM_2025-PLAN – v1.1`  
> **Thời gian thực hiện:** 06/10/2025 – 30/01/2026 (85 ngày làm việc / 1,997.41 giờ làm việc ~ 12.5 Man-Months)  

---

## 📌 1. Tổng Quan Dự Án (Project Overview)

Dự án tập trung vào việc lập kế hoạch, quản lý và mô hình hóa quy trình phát triển một **nền tảng thương mại điện tử chuyên bán sách, dụng cụ học tập và sản phẩm văn hóa** (theo mô hình Marketplace tương tự Fahasa.com). 

Hệ thống được thiết kế theo kiến trúc Web Responsive kết hợp ứng dụng di động (Android/iOS) và tích hợp hệ thống backend API kết nối các cổng thanh toán, đơn vị vận chuyển bên thứ ba.

### 🎯 Mục tiêu Dự án (Project Objectives)
* **Thời lượng & Lịch trình:** Đảm bảo hoàn thành đúng hạn 85 ngày làm việc (kết thúc trước 01/02/2026).
* **Ngân sách Nỗ lực:** Khống chế trong ngân sách cam kết 12.5 Man-Months (~1,997.41 giờ làm việc).
* **Chất lượng:** 
  * Tỷ lệ lỗi rò rỉ sau bàn giao (Defect Leakage) $\le 0.05$.
  * Mức độ hài lòng của Khách hàng (Hội đồng đánh giá) $\ge 4.0/5.0$.
  * Tuân thủ quy trình phát triển phần mềm $\ge 90\%$.
* **Phạm vi Chức năng Cốt lõi:** Hoàn thành tối thiểu 10 User Stories chính (Tìm kiếm, Đặt hàng, Flash Sale, Tích điểm F-Point, Ví Voucher, Sổ địa chỉ, v.v.).

---

## 👥 2. Cơ Cấu Tổ Chức & Phân Công Nhân Sự (Project Team & Roles)

Dự án được quản lý và thực hiện bởi **Nhóm 3:00 PM** gồm 4 thành viên Fresher đảm nhiệm theo mô hình quy trình chuẩn:

| Vai trò Quản lý / Kỹ thuật | Trách nhiệm chính trong MS Project & Dự án |
| :--- | :---: | :--- | :--- |
| **Project Manager (PM)** / Configuration Controller | Lập kế hoạch (WBS, MS Project), quản lý rủi ro, kiểm soát cấu hình (Git Flow/Version), báo cáo hội đồng. |
| **Business Analyst (BA)** / QA Support | Phân tích nghiệp vụ, khảo sát người dùng, đặc tả tài liệu SRS, quản lý yêu cầu thay đổi (CR). |
| **Developer A (Tech Lead / PTL)** | Thiết kế kiến trúc hệ thống, DB Schema, lập trình Frontend & Backend cốt lõi, Code Review. |
| **Developer B & Tester** | Lập trình các Module phụ, tích hợp API bên thứ 3, viết Test Plan/Test Case, thực hiện kiểm thử hệ thống độc lập (ST/UAT). |

---

## 🛠 3. Kiến Trúc Công Nghệ & Môi Trường (Tech Stack & Environment)

* **Backend:** Node.js (Express Framework), RESTful APIs.
* **Frontend:** React.js / Vue.js (Responsive Design, HTML5, CSS3, JavaScript).
* **Database:** MySQL / PostgreSQL.
* **Mobile Integration:** Android (Java/Kotlin) và iOS (Swift) qua API.
* **Third-Party APIs:** Cổng thanh toán (VNPAY, MoMo), Đơn vị vận chuyển (GHN, GHTK), Google Maps API, dịch vụ SMS/Zalo ZNS OTP.
* **Môi trường & Công cụ:** VS Code, Git/GitHub, Postman, Jest, TestLink, Trello/Jira.
* **Quy trình Quản lý Chất lượng:** Áp dụng mô hình **CMMI**, **DAR** (Phân tích & Giải quyết Quyết định) và **CAR** (Phân tích Nguyên nhân gốc rễ - 5 Whys).

---

## 📊 4. Cấu Trúc Phân Chia Công Việc (WBS & Effort Allocation)

Dự án có quy mô ước tính **150 Function Points (FP)** với tổng nỗ lực **1,997.41 hrs** được chia thành 5 giai đoạn chính theo MS Project:

```text
BOOK_MP_SWPM_2025 (Website Bán Sách Fahasa) ------------------- [85.00 ngày | 1,997.41 hrs]
├── 1.0 Thu thập & Phân tích yêu cầu (Tasks 1.1 - 1.7) -------- [38.92 ngày |   388.00 hrs]
├── 2.0 Thiết kế hệ thống (Tasks 2.1 - 2.5) ------------------- [20.50 ngày |   152.80 hrs]
├── 3.0 Phát triển phần mềm (Tasks 3.1 - 3.2) ----------------- [50.00 ngày |   581.20 hrs]
│   ├── 3.1 Frontend (Tasks 3.1.1 - 3.1.20) ------------------- [33.00 ngày |   252.00 hrs]
│   └── 3.2 Backend & Security (Tasks 3.2.1 - 3.2.25) --------- [47.00 ngày |   329.20 hrs]
├── 4.0 Tích hợp hệ thống (Tasks 4.1 - 4.3) ------------------- [29.50 ngày |    36.00 hrs]
└── 5.0 Kiểm thử & Triển khai website (Tasks 5.1 - 5.13) ------- [68.50 ngày |   839.41 hrs]
```

---

## 📅 5. Các Mốc Bàn Giao Quan Trọng (Project Milestones)

Dự án triển khai theo chiến lược **Waterfall điều chỉnh (Fast-tracking & Continuous Integration)**:

| Task ID | Tên Mốc Milestone | Ngày hoàn thành | Sản phẩm bàn giao chính (Deliverables) |
| :---: | :--- | :---: | :--- |
| **9** | **Hoàn thành phân tích** | `27/11/2025` | Tài liệu Đặc tả Yêu cầu Phần mềm (**SRS**). |
| **16** | **Hoàn thành thiết kế** | `14/11/2025` | Tài liệu Thiết kế Phần mềm (**SWD**), Architecture & DB Schema. |
| **65** | **Hoàn thành lập trình** | `02/01/2026` | Đóng băng mã nguồn Frontend & Backend (**Code Freeze**). |
| **74** | **Hoàn thành tích hợp** | `28/01/2026` | Tích hợp hoàn tất API VNPAY/MoMo, GHN/GHTK, Google Maps, Social Login. |
| **89** | **Hoàn thành kiểm thử & triển khai** | `08/01/2026` | Hệ thống chạy trên môi trường Staging/Live, UAT Sign-off. |
| **0** | **Kết thúc toàn bộ Dự án** | `30/01/2026` | Bàn giao Code, Tài liệu Hướng dẫn Cài đặt & Hướng dẫn Sử dụng. |

---

## 📑 6. Danh Mục 17 Trang & Module Chức Năng Cốt Lõi (SRS & Requirements)

Dự án bao gồm 17 Module màn hình chi tiết được đặc tả luồng biến cố nghiệp vụ:

1. **Trang Chủ (Homepage):** Banner slide khuyến mãi, tìm kiếm động (max 100 ký tự), chuyển đổi ngôn ngữ VN/EN, danh mục nổi bật, gợi ý sản phẩm cá nhân hóa.
2. **Trang Sản Phẩm (Product Listing):** Menu Sidebar danh mục, bộ lọc đa tiêu chí (Giá, Thể loại/Genres, Thương hiệu, Độ tuổi, NXB), thanh sắp xếp AJAX.
3. **Trang Chi Tiết Sản Phẩm:** Khung thông tin cố định bên trái, form tra cứu nhà sách còn hàng (Google Maps API), đánh giá sao & nhận xét ẩn danh.
4. **Trang Sách Giáo Khoa & Đồ Dùng Học Tập:** Lọc theo cấp học (Lớp 1–12, Đại học), bộ lọc nhanh dụng cụ học sinh (Bút bi, Balo, Tập vở).
5. **Giỏ Hàng & Quà Tặng (Cart & Gifts):** Tính tổng tiền realtime, áp dụng đồng thời mã Freeship + Coupon, modal chọn quà tặng theo mốc giá trị đơn hàng.
6. **Trang Flash Sale:** Đồng hồ đếm ngược (Countdown real-time), chuyển đổi phiên sale theo khung giờ (Đang bán, Sắp bán, Ngày mai).
7. **Trang Mã Khuyến Mãi (Voucher Store):** Lưu mã trực tiếp vào ví cá nhân, xem điều kiện áp dụng, sao chép mã nhanh.
8. **Trang Sản Phẩm Mới:** Tải danh sách tự động từ Backend, hỗ trợ lọc theo Mới nhất, Bán chạy, Chiết khấu.
9. **Form Đăng Ký / Đăng Nhập / Khôi Phục Mật Khẩu:** Xác thực OTP qua SMS/Zalo ZNS, mã hóa mật khẩu bcrypt, bảo mật RBAC, tùy chọn ẩn/hiện mật khẩu.
10. **Trang Thông Tin Tài Khoản:** Quản lý hồ sơ cá nhân, cập nhật ngày sinh, giới tính, hiển thị cấp độ thành viên & số F-Point tích lũy.
11. **Trang Sổ Địa Chỉ (Address Book):** Quản lý địa chỉ giao hàng & thanh toán mặc định, tích hợp cây địa giới hành chính Việt Nam (Tỉnh/Thành, Quận/Huyện, Xã/Phường).
12. **Trang Đổi Mật Khẩu:** Kiểm tra mật khẩu hiện tại trên server, kiểm tra độ mạnh mật khẩu mới.
13. **Trang Đơn Hàng & Chi Tiết Đơn Hàng:** Bộ lọc tab trạng thái đơn, dòng thời gian (Timeline) giao hàng, nút mua lại đơn cũ, tra cứu vận chuyển API.
14. **Trang Thông Báo:** Phân loại thông báo (Đơn hàng, Sự kiện, Mã giảm giá), đánh dấu trạng thái Đã đọc/Chưa đọc.
15. **Trang Ưu Đãi Thành Viên:** Thông tin phân hạng (Bạc, Vàng, Kim Cương), tỷ lệ tích lũy F-Point, ưu đãi quà sinh nhật.
16. **Trang Ví Voucher:** Quản lý Voucher của tôi và Voucher đối tác, cảnh báo mã hết hạn.
17. **Trang Tài Khoản F-Point / Freeship:** Hiển thị số dư điểm thưởng, bảng lịch sử biến động điểm (cộng/trừ), ô nạp điểm qua mã PIN.

---

## 🛡 7. Quản Lý Chất Lượng & Rủi Ro (QA & Risk Management)

### Chiến lược kiểm thử & Giảm thiểu Rủi ro Nhân sự
* **Shift-Left Testing:** Tester viết Test Case ngay từ giai đoạn Phân tích Yêu cầu (Task 5.1 từ 28/10/2025).
* **Bắt buộc Peer Code Review 100%:** Dev A (Tech Lead) và Dev B review mã nguồn chéo trước khi merge nhánh `develop` nhằm kiểm soát rủi ro nhân sự Fresher.

### Chiến lược Phân bổ 150 Lỗi mục tiêu (Defect Allocation):
* **Requirements Review:** 18 lỗi (12%)
* **Design Review:** 15 lỗi (10%)
* **Code Review:** 38 lỗi (25%)
* **Unit Test:** 52 lỗi (35%)
* **Integration Test:** 15 lỗi (10%)
* **System Test:** 8 lỗi (5%)
* **UAT Leakage Target:** 4 lỗi ($\le 3\%$)