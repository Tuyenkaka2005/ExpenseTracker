<img width="210"  alt="dashboard" src="https://github.com/user-attachments/assets/37251bf9-c089-486d-96e9-5d9078b7414f" />
<img width="210"  alt="add-expense" src="https://github.com/user-attachments/assets/d2aae060-fcc3-4610-90e4-7117920fdfe5" />
<img width="210"  alt="darkmode" src="https://github.com/user-attachments/assets/d3ac2207-edd0-4468-acb3-0b56bd04737f" />
<img width="210" alt="delete" src="https://github.com/user-attachments/assets/e8bdf763-fa42-4a64-99fe-0596c4ffd66a" />


# 💸 Expense Tracker App

Ứng dụng Quản lý Chi tiêu Cá nhân được phát triển bằng **SwiftUI** (Lab 2 — SwiftUI Intermediate Foundation). Dự án tập trung vào việc xây dựng luồng giao diện người dùng (UI Flow) mượt mà, quản lý trạng thái dữ liệu (State Management) và áp dụng các tiêu chuẩn **Clean Code** thông qua việc module hóa các UI Components.

---

## ✨ Tính năng nổi bật (Features)

* 📊 **Dashboard Tổng quan**: Hiển thị tổng số tiền đã chi tiêu (Summary Card) và tự động tính toán lại ngay khi có thay đổi dữ liệu.
* 🏷️ **Bộ lọc Danh mục (Category Filter)**: Lọc danh sách giao dịch nhanh chóng theo các danh mục (*Food, Transport, Shopping, Entertainment, Other*) bằng thanh Filter Chips nằm ngang.
* ➕ **Thêm Khoản chi (Add Expense)**: Form nhập liệu trực quan tận dụng tối đa các thành phần Native của iOS (TextField, Picker, DatePicker).
* 🛡️ **Xác thực Dữ liệu (Validation)**: Tự động vô hiệu hóa nút *Save* nếu người dùng để trống tiêu đề hoặc nhập sai định dạng số tiền.
* 🗑️ **Xóa Giao dịch (Delete Expense)**: Hỗ trợ thao tác vuốt để xóa (Swipe-to-delete) trực tiếp trên danh sách.
* 🌗 **Hỗ trợ Dark Mode**: Sử dụng các dải màu hệ thống (`.primary`, `.secondary`, `.accentColor`) giúp giao diện hiển thị độ tương phản hoàn hảo trên cả Light Mode và Dark Mode.
* 🎨 **Trạng thái Trống (Empty State)**: Tích hợp `ContentUnavailableView` của iOS 17 để hiển thị thông báo đẹp mắt khi danh mục không có giao dịch nào.

---

## 📱 UI Flow & Giao diện

```text
[ Dashboard Screen ] ──(Filter/Swipe Delete)──> [ Expense List ]
         │
    (Tap "+" Button)
         │
         ▼
[ Add Expense Sheet ] ──(Fill Form & Save)──> [ Updates Dashboard ]
