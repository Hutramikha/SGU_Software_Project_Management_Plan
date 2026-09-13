# 📚 Dự Án Quản Lý Phát Triển Website Bán Sách Trực Tuyến (Fahasa Marketplace Model)
  
> **Mã dự án (Project Code):** `BOOK_MP_SWPM_2025`  
> **Mã tài liệu (Document Code):** `BOOK_MP_SWPM_2025-PLAN – v1.1`  
> **Thời gian thực hiện:** 06/10/2025 – 30/01/2026 (85 ngày làm việc / 1,997.41 giờ làm việc ~ 12.5 Man-Months)  

---

## 📌 1. Tổng Quan Dự Án (Project Overview)

Dự án tập trung vào việc lập kế hoạch, quản lý và mô hình hóa quy trình phát triển một **nền tảng thương mại điện tử chuyên bán sách, dụng cụ học tập và sản phẩm văn hóa** (theo mô hình Marketplace tương tự Fahasa.com). 

Hệ thống được thiết kế theo kiến trúc Web Responsive kết hợp ứng dụng di động (Android/iOS) và tích hợp hệ thống backend API kết nối các cổng thanh toán, đơn vị vận chuyển bên thứ ba[cite: 1, 2].

### 🎯 Mục tiêu Dự án (Project Objectives)
* **Thời lượng & Lịch trình:** Đảm bảo hoàn thành đúng hạn 85 ngày làm việc (kết thúc trước 01/02/2026).
* **Ngân sách Nỗ lực:** Khống chế trong ngân sách cam kết 12.5 Man-Months (~1,997.41 giờ làm việc).
* **Chất lượng:** 
  * Tỷ lệ lỗi rò rỉ sau bàn giao (Defect Leakage) $\le 0.05$.
  * Mức độ hài lòng của Khách hàng (Hội đồng đánh giá) $\ge 4.0/5.0$.
  * Tuân thủ quy trình phát triển phần mềm $\ge 90\%$.
* **Phạm vi Chức năng Cốt lõi:** Hoàn thành tối thiểu 10 User Stories chính (Tìm kiếm, Đặt hàng, Flash Sale, Tích điểm F-Point, Ví Voucher, Sổ địa chỉ, v.v.)[cite: 1, 2].

---

## 👥 2. Cơ Cấu Tổ Chức & Phân Công Nhân Sự (Project Team & Roles)

Dự án được quản lý và thực hiện bởi **Nhóm 3:00 PM** gồm 4 thành viên Fresher đảm nhiệm theo mô hình quy trình chuẩn:

| Thành viên | Mã SV | Vai trò Quản lý / Kỹ thuật | Trách nhiệm chính trong MS Project & Dự án |
| :--- | :---: | :--- | :--- |
| **Huỳnh Trần Minh Khang** | `3122410169` | **Project Manager (PM)**[cite: 1] / Configuration Controller | Lập kế hoạch (WBS, MS Project), quản lý rủi ro, kiểm soát cấu hình (Git Flow/Version), báo cáo hội đồng[cite: 1]. |
| **Nguyễn Duy Sơn**[cite: 1] | `3122410360` | **Business Analyst (BA)**[cite: 1] / QA Support | Phân tích nghiệp vụ, khảo sát người dùng, đặc tả tài liệu SRS, quản lý yêu cầu thay đổi (CR)[cite: 1, 2]. |
| **Châu Nguyễn Trường Vũ**[cite: 1] | `3122410479` | **Developer A (Tech Lead / PTL)** | Thiết kế kiến trúc hệ thống, DB Schema, lập trình Frontend & Backend cốt lõi, Code Review. |
| *Fresher Dev B & Tester*[cite: 1] | *Nội bộ*[cite: 1] | **Developer B & Tester** | Lập trình các Module phụ, tích hợp API bên thứ 3, viết Test Plan/Test Case, thực hiện kiểm thử hệ thống độc lập (ST/UAT)[cite: 1, 4]. |

---

## 🛠 3. Kiến Trúc Công Nghệ & Môi Trường (Tech Stack & Environment)

* **Backend:** Node.js (Express Framework), RESTful APIs[cite: 1, 2].
* **Frontend:** React.js / Vue.js (Responsive Design, HTML5, CSS3, JavaScript)[cite: 1, 2].
* **Database:** MySQL / PostgreSQL[cite: 1, 2].
* **Mobile Integration:** Android (Java/Kotlin) và iOS (Swift) qua API[cite: 2].
* **Third-Party APIs:** Cổng thanh toán (VNPAY, MoMo), Đơn vị vận chuyển (GHN, GHTK), Google Maps API, dịch vụ SMS/Zalo ZNS OTP[cite: 2, 4].
* **Môi trường & Công cụ:** VS Code, Git/GitHub, Postman, Jest, TestLink, Trello/Jira[cite: 1].
* **Quy trình Quản lý Chất lượng:** Áp dụng mô hình **CMMI**, **DAR** (Phân tích & Giải quyết Quyết định) và **CAR** (Phân tích Nguyên nhân gốc rễ - 5 Whys)[cite: 1].

---

## 📊 4. Cấu Trúc Phân Chia Công Việc (WBS & Effort Allocation)

Dự án có quy mô ước tính **150 Function Points (FP)** với tổng nỗ lực **1,997.41 hrs** được chia thành 5 giai đoạn chính theo MS Project[cite: 1, 4]:

```text
BOOK_MP_SWPM_2025 (Website Bán Sách Fahasa) ------------------- [85.00 ngày | 1,997.41 hrs]
├── 1.0 Thu thập & Phân tích yêu cầu (Tasks 1.1 - 1.7) -------- [38.92 ngày |   388.00 hrs]
├── 2.0 Thiết kế hệ thống (Tasks 2.1 - 2.5) ------------------- [20.50 ngày |   152.80 hrs]
├── 3.0 Phát triển phần mềm (Tasks 3.1 - 3.2) ----------------- [50.00 ngày |   581.20 hrs]
│   ├── 3.1 Frontend (Tasks 3.1.1 - 3.1.20) ------------------- [33.00 ngày |   252.00 hrs]
│   └── 3.2 Backend & Security (Tasks 3.2.1 - 3.2.25) --------- [47.00 ngày |   329.20 hrs]
├── 4.0 Tích hợp hệ thống (Tasks 4.1 - 4.3) ------------------- [29.50 ngày |    36.00 hrs]
└── 5.0 Kiểm thử & Triển khai website (Tasks 5.1 - 5.13) ------- [68.50 ngày |   839.41 hrs]