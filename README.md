💸 Thực Hiện Giao Dịch Trên Blockchain
Đây là một dự án mô phỏng quá trình thực hiện giao dịch giữa người bán và người cho mua thông qua Smart Contract trên nền tảng Blockchain. Ứng dụng sử dụng giao diện web đơn giản (HTML + JS) để tương tác trực tiếp với MetaMask và hợp đồng thông minh đã triển khai.

🎯 Mục tiêu
Xây dựng giao diện web cho phép người dùng thực hiện các hành động mua và bán.
Kết nối với ví MetaMask để ký và gửi giao dịch.
Tương tác với Smart Contract viết bằng Solidity.
Ghi lại lịch sử và trạng thái các khoản vay trên blockchain.
chức năng của hệ thống
🧩 1. Thêm giao dịch mới Người dùng nhập Tên người bán và Tên người mua.

Nhấn nút "Thêm giao dịch".

Giao dịch được lưu vào blockchain thông qua hàm recordPayment(seller, buyer).

Sau khi thành công, giao dịch sẽ hiện ở bảng DS giao dịch bên dưới. image

Xem danh sách giao dịch Nhấn nút "DS giao dịch" để gọi getPaymentCount() và getPaymentByIndex(i) từ smart contract.
Dữ liệu được hiển thị trong bảng với các cột:

#: chỉ số

Người bán

Người mua

Thời gian

Hành động: 2 nút Edit và Delete image Lịch sử chỉnh sửa và xóa Nhấn nút "DS giao dịch đã sửa" hoặc "DS giao dịch đã xóa" để tải lịch sử.

Gọi lần lượt:

getEditHistoryCount() + getEditHistory(index)

getDeleteHistoryCount() + getDeleteHistory(index)

Dữ liệu hiển thị trong 2 bảng tương ứng bên dưới.

image

Chức năng	Mô tả ngắn
Ghi giao dịch	Gửi thông tin người bán/người mua lên blockchain
Hiển thị giao dịch	Lấy danh sách và hiển thị vào bảng
Chỉnh sửa	Cập nhật thông tin và lưu lịch sử
Xóa	Xóa giao dịch, lưu thời gian xóa
Lịch sử	Hiển thị các giao dịch đã chỉnh/xóa
🛠 Công nghệ sử dụng
⚙️ Solidity – Viết Smart Contract
🌐 HTML + CSS + JavaScript
🔌 Ethers.js – Giao tiếp với blockchain
🔒 MetaMask – Ví phi tập trung để ký giao dịch
🧪 Hardhat / Ganache – Môi trường kiểm thử hợp đồng
