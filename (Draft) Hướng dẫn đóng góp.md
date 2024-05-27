
## Giai đoạn 0: Đề xuất mới

1. **Tạo issue mới trên GitHub:**
    - Bạn đang đề xuất thành phần (component), biến thể (variant) hoặc tính năng (function) của thành phần mới nào?
    - Vui lòng mô tả các trường hợp sử dụng (use case) liên quan.
    - Đề xuất này có phù hợp với hệ thống thiết kế hiện tại không? Nếu đề xuất có mục đích cải tiến hệ thống thiết kế, vui lòng giải thích.
    - Vui lòng kèm theo các thiết kế và hình ảnh minh họa liên quan.
2. **Chờ đề xuất được xét duyệt**

## Giai đoạn I: Design + Code + Documentation

Sau khi đề xuất ở giai đoạn 0 được xét duyệt, issue bước sang giai đoạn I. Giai đoạn này bao gồm ba mảng công việc được thực hiện đồng thời: Design, Code và Documentation. Các thành viên trong nhóm sẽ được thêm vào mảng công việc liên quan.

### Design

1. **Hoàn thiện thiết kế**
    - Bạn đã bao gồm tất cả các thông số và token thiết kế cần thiết (màu sắc, kiểu chữ, khoảng cách, kích cỡ, breakpoint, ...) chưa?
    - Thiết kế đã thể hiện cách đáp ứng nhiều kích cỡ màn hình / xử lý nội dung tràn (content overflow) chưa?
    - Thiết kế đã thể hiện các trạng thái (state) khác nhau chưa?
    - Có bất kỳ cân nhắc cụ thể nào về khả năng tiếp cận của người dùng (accessibililty) trong thiết kế không?
2. **Chờ ý kiến phản hồi trong issue và cập nhật thiết kế theo phương án được thống nhất**

### Code

1. **Tạo branch mới (branch gốc của issue) và phát triển code**
2. **Tạo pull request**
	- Thành phần có cấu trúc như thế nào? Có những bộ phận nào?
	- Thành phần có những thuộc tính (attributes / props) nào?
	- Thành phần có những methods và events nào?
	- Code đang phát triển có nhất quán giữa các nền tảng khác nhau không?
	- Code đang phát triển có tương thích với phiên bản cũ không?
	- Code có phụ thuộc vào thư viện bên thứ ba không?
3. **Chờ ý kiến phản hồi trên pull request và cập nhật code theo phương án được thống nhất**

### Documentation

1. **Dùng branch nháp đặc biệt để biên soạn bản dự thảo tài liệu mô tả**
2. **Cập nhật tài liệu mô tả liên quan xuyên suốt quá trình phát triển**
	- Sử dụng (Usage)
	- Biến thể (Variants)
		- Trong trường hợp không thể đính kèm demo code hoạt động, đính kèm hình ảnh minh họa
	- Phát triển (Dev)

## Giai đoạn II: Tinh chỉnh & và kiểm tra

1. **Tinh chỉnh và tối ưu hóa code**
2. **Khắc phục các lỗi tồn đọng và xử lý các trường hợp hiếm phát sinh**
3. **Thực hiện kiểm tra**
    - **Trường hợp sử dụng**
        - Thành phần hoạt động như thế nào so với trường hợp sử dụng được đề xuất ban đầu?
    - **Tương thích trình duyệt**
        - Thành phần hoạt động như thế nào trên các trình duyệt khác nhau?
        - Có bất kỳ trình duyệt hoặc phiên bản cụ thể nào phát sinh vấn đề cần lưu ý không?
    - **Khả năng tiếp cận**
        - Thành phần đã được kiểm tra về khả năng tiếp cận như thế nào (ví dụ: trình đọc màn hình, điều hướng bằng bàn phím)?
    - **Tình trạng đồng bộ giữa các nền tảng**
        - Tình trạng đồng bộ hóa thư viện giữa các nền tảng như thế nào?
        - Có bất kỳ vấn đề hoặc khác biệt cụ thể nào cần lưu ý không?
- **Hoàn thiện tài liệu mô tả và di chuyển nội dung sang branch gốc của issue**
	- Hình ảnh minh họa đã được thay thế bằng demo code hoạt động ở những nơi cần thiết chưa?

## Giai đoạn III: Đóng gói và phát hành

1. **Chuẩn bị cho việc phát hành**
	- Có bất kỳ vấn đề hoặc lo ngại nào chưa được giải quyết không? Nếu hiện tại chưa thể xử lý, có kèm theo ghi chú trong tài liệu mô tả không?
	- Package đã được đóng gói thử và kiểm tra chưa?
	- Phiên bản của package chuẩn bị được phát hành có tuân thủ theo nguyên tắc của semantic versioning không? 
2. **Phát hành package trên npm**