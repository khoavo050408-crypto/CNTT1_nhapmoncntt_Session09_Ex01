Hai sai lầm trong tư duy của Nam
Nhầm lẫn giữa công cụ soạn thảo trực quan (WYSIWYG) và hệ thống quản lý mã nguồn (Version Control): Nam cho rằng Word tốt vì có giao diện chọn font, màu sắc trực quan. Tuy nhiên, định dạng .docx thực chất là một gói nén ZIP chứa cấu trúc XML phức tạp, biến tài liệu thành một khối nhị phân (binary blob). Git không thể đọc hiểu và so sánh từng dòng văn bản (line-by-line diff) bên trong file Word, dẫn đến việc chỉ cần một thay đổi nhỏ như một dấu phẩy cũng làm xáo trộn toàn bộ cấu trúc ngầm và gây xung đột (conflict) toàn bộ file.
Đánh giá thấp sức mạnh của Markdown: Nam cho rằng Markdown chỉ là "văn bản thô, không chuyên nghiệp". Thực tế, Markdown sử dụng cú pháp ký tự nhẹ nhàng để định dạng (tiêu đề, danh sách, bảng biểu, mã nguồn) và được các nền tảng như GitHub hỗ trợ hiển thị trực quan, chuyên nghiệp ngay trên trình duyệt mà không cần cài đặt phần mềm chuyên dụng.
Tại sao Markdown an toàn và nhẹ hơn?
Khả năng chống hư hại file (Rủi ro mất dữ liệu): Cấu trúc nén của file Word rất nhạy cảm; nếu một sự cố mạng hoặc lỗi ghi đĩa làm mất hoặc sai lệch chỉ một byte duy nhất, toàn bộ file .docx sẽ bị hỏng hoàn toàn và Microsoft Word không thể giải nén hay mở lại được nữa. Ngược lại, Markdown là văn bản thô (Plain Text) có dung lượng cực nhẹ. Nếu file gặp lỗi dữ liệu, chỉ ký tự hoặc dòng bị ảnh hưởng tại chỗ đó, toàn bộ phần nội dung còn lại vẫn hoàn toàn nguyên vẹn và đọc được bằng bất kỳ trình soạn thảo nào.
Tối ưu cho Git và cộng tác nhóm: Markdown lưu dưới dạng văn bản thuần túy, cho phép Git theo dõi từng dòng thay đổi, hỗ trợ tính năng Merge thông minh và giúp các thành viên trong nhóm dễ dàng xem trực tiếp tài liệu ngay trên trình duyệt web.

Đoạn giới thiệu dự án sau khi chuyển đổi sang định dạng .md:
Markdown
# Dự án: Hệ thống Định vị Khẩn cấp Không cần GPS
## Giới thiệu
Ứng dụng di động hỗ trợ xác định vị trí và phát tín hiệu cứu hộ trong các tình huống khẩn cấp mà không phụ thuộc vào kết nối GPS, đảm bảo an toàn tối ưu cho người dùng trong điều kiện hiểm trở hoặc mất sóng định vị vệ tinh.
## Tính năng chính- Kích hoạt nút khẩn cấp (Emergency Button) nhanh chóng bằng thao tác đơn giản.- Tự động ghi nhận và truyền tải thông tin định vị thay thế.- Giao diện thân thiện, dễ tiếp cận cho cả trẻ em và người lớn tuổi.
## Thành viên nhóm- Đội phát triển: khoa
