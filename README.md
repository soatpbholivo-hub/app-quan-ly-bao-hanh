# Olivo – Quản lý bảo hành

App web 1 file (`index.html`), JS thuần, giao diện tiếng Việt, dùng được trên điện thoại. Mở file bằng trình duyệt là chạy, không cần cài đặt.

## Tính năng
- **Phiếu bảo hành**: tiếp nhận, tìm kiếm, lọc theo trạng thái / kỹ thuật / quá hạn, phân trang, xem chi tiết, chuyển trạng thái nhanh, lịch sử thay đổi (trạng thái, kỹ thuật).
- **Tự động**: mã phiếu `BHyymm-0001`; tự điền mã/nhóm khi chọn sản phẩm; tính còn hạn/hết hạn bảo hành theo ngày mua; tự điền ngày khi đổi trạng thái (chỉ khi ô trống); đánh dấu quá hạn theo "Hạn xử lý" trong Cấu hình chung; chia phiếu mới xoay vòng cho kỹ thuật cùng khu vực.
- **Sản phẩm**: danh mục kèm thời hạn bảo hành (tháng).
- **Người dùng & quyền**: Quản trị (toàn quyền), Tiếp nhận/CSKH (tạo, sửa phiếu, danh mục), Kỹ thuật (chỉ sửa phần xử lý trên phiếu được giao).
- **Cấu hình chung**: tên đơn vị, hạn xử lý, bật/tắt tự chia việc; quản lý danh sách giá trị + màu (trạng thái, ưu tiên, khu vực, phụ kiện…). Đổi tên giá trị cập nhật luôn các phiếu đang dùng; xóa giá trị thì phiếu cũ vẫn giữ.
- **Excel**: xuất/nhập phiếu và sản phẩm (nhập phiếu khớp theo Mã phiếu thì cập nhật, không có mã thì tạo mới).
- **Sao lưu / khôi phục** toàn bộ dữ liệu ra file `.json`.

## Tài khoản mẫu
`admin` / `admin123` · `cskh` / `123456` · `kt.hn` / `123456` · `kt.hcm` / `123456` — đổi mật khẩu trong mục Người dùng. Dữ liệu mẫu xóa được bằng nút "Xóa dữ liệu mẫu".

## Lưu ý về dữ liệu
Dữ liệu lưu trong trình duyệt (localStorage) của từng máy, **không tự đồng bộ giữa nhiều người/máy**. Dùng Sao lưu/Khôi phục để chuyển dữ liệu. Nếu cần nhiều người dùng chung một kho dữ liệu, cần nối thêm nơi lưu trữ dùng chung (ví dụ Google Sheets, Supabase, Firebase).
