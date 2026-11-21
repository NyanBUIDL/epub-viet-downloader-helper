# Chính sách quyền riêng tư của Epub Việt Downloader

Áp dụng cho phiên bản 0.12.2, cập nhật ngày 21/11/2026.

Epub Việt Downloader đọc nội dung truyện theo yêu cầu của người dùng và tạo tệp EPUB để lưu trên máy. Một số chức năng sử dụng ứng dụng Scrapling Helper cài riêng trên Windows.

## Dữ liệu được xử lý

- Liên kết truyện và chương do người dùng chọn, tên sách, tên tác giả, mục lục và nội dung chương.
- Cài đặt tải, tiến độ, danh sách chương còn thiếu và bản lưu để tiếp tục tải.
- Khi bật dịch offline, ngôn ngữ nguồn và đích, bảng tên riêng do người dùng nhập và bản dịch.
- Trong chế độ tab trình duyệt, website sử dụng phiên đăng nhập hiện có của trình duyệt. Tiện ích thực hiện yêu cầu đọc nội dung trong phiên đó.
- Helper sử dụng hồ sơ Chrome riêng. Hồ sơ này có thể lưu cookie, thông tin đăng nhập trên website và bộ nhớ đệm theo hoạt động của Chrome và website.

Tiện ích sử dụng các dữ liệu trên để đọc nội dung đã chọn, tiếp tục tác vụ, dịch khi người dùng bật chức năng này và xuất EPUB.

## Lưu trữ trên máy

Cài đặt và bản lưu chương của tiện ích nằm trong bộ nhớ cục bộ của extension, gồm IndexedDB. Helper lưu bản ghi chương và hồ sơ Chrome trong thư mục STV-EPUB-Scrapling bên dưới thư mục Local AppData của tài khoản Windows. Tệp EPUB nằm tại vị trí người dùng chọn hoặc trong thư mục tải xuống.

Dữ liệu tiếp tục được giữ để người dùng có thể đọc, xuất và tiếp tục tải vào lần sau. Bộ gỡ Helper giữ lại bản lưu chương và hồ sơ Chrome.

Người dùng có thể xóa dữ liệu extension bằng chức năng quản lý dữ liệu của Chrome hoặc gỡ extension. Để xóa dữ liệu Helper còn lại, đóng Helper và các cửa sổ Chrome do Helper mở, sau đó xóa thư mục STV-EPUB-Scrapling trong Local AppData. Tệp EPUB đã xuất được quản lý và xóa riêng như các tệp khác trên máy.

## Kết nối và bên nhận dữ liệu

- Sáng Tác Việt nhận các yêu cầu đọc mục lục và chương. Website và các dịch vụ được website tải có thể nhận thông tin kết nối, cookie và dữ liệu trình duyệt theo cách vận hành của họ.
- Cloudflare có thể tham gia xử lý xác minh Turnstile và yêu cầu DNS dự phòng. Luồng xác minh được thực hiện trong phiên Chrome do Helper quản lý.
- GitHub nhận yêu cầu tải bộ cài Helper. Khi dùng dịch offline lần đầu, Helper có thể tải bộ chạy từ GitHub và model từ Hugging Face. Các nhà cung cấp này có thể nhận địa chỉ IP, thông tin yêu cầu tải và các thông tin kết nối thông thường.
- Extension gửi dữ liệu công việc tới Helper trên chính máy qua cầu nối Native Messaging và địa chỉ loopback được bảo vệ bằng mã kết nối theo phiên.

Mã ứng dụng hiện tại không gửi nội dung truyện hoặc văn bản cần dịch tới máy chủ của nhà phát triển. Chức năng dịch xử lý văn bản trên máy sau khi tải các thành phần cần thiết. Mã extension hiện không tích hợp dịch vụ quảng cáo hoặc phân tích hành vi của nhà phát triển.

## Giới hạn sử dụng dữ liệu

Dữ liệu được xử lý để cung cấp các chức năng đọc mục lục, tải và lưu chương, tiếp tục công việc, dịch offline tùy chọn và xuất EPUB. Nhà phát triển không bán dữ liệu người dùng, không dùng hoặc chuyển dữ liệu để quảng cáo cá nhân hóa, đánh giá tín dụng hoặc cho vay. Việc sử dụng và chuyển dữ liệu tuân thủ Chính sách dữ liệu người dùng của Chrome Web Store, bao gồm các yêu cầu về Giới hạn sử dụng (Limited Use): https://developer.chrome.com/docs/webstore/program-policies/user-data.

## Ủng hộ tự nguyện

Ứng dụng có thể hiển thị mã QR ủng hộ nhà phát triển. Người dùng thực hiện giao dịch trong ứng dụng thanh toán của mình. Epub Việt Downloader không yêu cầu người dùng nhập thông tin thẻ, mật khẩu thanh toán hoặc cung cấp biên nhận để mở chức năng.

## Liên hệ và thay đổi chính sách

Người dùng có thể liên hệ qua mục Issues tại https://github.com/NyanBUIDL/epub-viet-downloader-helper/issues. Mục Issues là công khai; người dùng nên mô tả lỗi và che thông tin riêng tư trước khi đăng.

Chính sách này cần được cập nhật cùng với thay đổi thực tế về cách xử lý dữ liệu của sản phẩm.