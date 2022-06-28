# Cơ chế hoạt động của Website
## 1. Cơ chế hoạt động của Internet
* Internet là một hệ thống thông tin toàn cầu giúp các máy tính, thiết bị điện tử thông minh kết nối và trao đổi dữ liệu với nhau trên toàn thế giới. Tất cả các máy tính, thiết bị kết nối internet đều có một địa chỉ IP. Trang web có địa chỉ IP là địa chỉ IP của máy chủ lưu trữ trang web, tuy nhiên để dễ nhớ thì chúng ta sử dụng tên miền để truy cập. Khi truy cập 1 trang web bằng trình duyệt, trình duyệt sẽ gửi yêu cầu tới máy chủ DNS để tìm xem địa chỉ IP nào tương ứng với tên miền mà bạn đã nhập. Sau khi lấy được địa chỉ IP, trình duyệt sẽ yêu cầu tới máy chủ để truy cập được vào trang web. Quá trình này chỉ diễn ra trong vòng vài giây hoặc ít hơn. 

## 2. Giải thích về protocol của HTTP/HTTPS
* Protocol là tập hợp các quy tắc được thiết lập nhằm xác định các để định dạng, truyền và nhận dữ liệu sao cho các thiết bị mạng máy tính - từ server và router tới endpoint - có thể giao tiếp với nhau, bất kể sự khác biệt về cơ sở hạ tầng, thiết kế hay các tiêu chuẩn cơ bản giữa chúng
* **HTTP** là giao thức truyền tải siêu văn bản, giao thức tiêu chuẩn cho World Wide Web (www) truyền tải dữ liệu dưới dạng văn bản, hình ảnh, âm thanh, video từ web server tới trình duyệt của người dùng và ngược lại. HTTP hoạt động theo mô hình Client (máy khách) - Server (máy chủ), trong đó khi yêu cầu truy cập 1 trang web trình duyệt sẽ kết nối để server của trang web thông qua địa chỉ IP do DNS cung cấp, máy chủ khi nhận lệnh sẽ trả về lệnh tương ứng để hiển thị nội dung trang web. Tuy nhiên trong quá trình kết nối và trao đổi thông tin này, *trình duyệt sẽ thừa nhận địa chỉ IP đó đến từ server của chính website mà bạn yêu cầu truy cập, không có bất kì biện pháp xác thực nào*. Các thông tin được gửi đi qua giao thức HTTP (bao gồm địa chỉ IP, thông tin nhập vào website) cũng không hề được mã hóa và bảo mật. Đây là kẽ hở nhiều hacker đã lợi dụng để đánh cắp thông tin người dùng (tấn công Sniffing)
* **HTTPS** là giao thức truyền tải siêu văn bản an toàn. Đây là giao thức HTTP tích hợp thêm chứng chỉ bảo mật (SSL hoặc TLS) để mã hóa các thông tin gửi đi nhằm tăng tính bảo mật. *Khi máy khách truy cập 1 website giao thức HTTPS sẽ hỗ trợ xác thực danh tính của website thông qua việc kiểm tra xác thực bảo mật*. HTTPS là tiêu chuẩn bảo mật tối thiểu mà tất cả các website doanh nghiệp cần đáp ứng do 1 số lý do sau:
    * Bảo mật thông tin người dùng
    * Tránh lừa đảo website giả mạo
    * Tăng uy tín đổi với người dùng
    * Tăng SEO (do Google đẩy xếp hạng tìm kiếm đối với website sử dụng phương thức HTTPS)
    * Tuy HTTPS chậm hơn HTTP nhưng ko đáng kể do công nghệ phát triển sự khác biệt đã đạt tới giới hạn tiệm cận bằng 0

## 3. Cơ chế hoạt động của browser và sự khác nhau giữa các browser
* Browser hay còn gọi là Web Browser (Trình duyệt web) là một công cụ dùng để tìm, duyệt thông tin và hiển thị nội dung trang web cho người dùng.
* Có rất nhiều trình duyệt web hiện nay nhưng có 1 số trình duyệt phổ biến hiện nay như: Google Chrome, Mozilla Firefox, Microsoft Edge, Safari, Opera,...  
    * **Google Chrome**: trình duyệt phổ biến nhất hiện nay 
        * Ưu điểm:
            - Tương thích với mọi hệ điều hành
            - Hỗ trợ hầu hết các ngôn ngữ trên toàn quốc tế
            - Tìm kiếm nhanh trên thanh địa chỉ
            - Tốc độ xử lý nhanh
            - Nhiều extension hỗ trợ
            - Hỗ trợ quản lý hồ sơ người dùng và đồng bộ tất cả lịch sử duyệt web, mật khẩu, dấu trang ...
        * Nhược điểm:
            - Tốn nhiều dung lượng
            - Chế độ ẩn danh không che dấu hoàn toàn hoạt động người dùng
    * **Mozilla Firefox**:
        * Ưu điểm:
            - Bảo mật mạnh và an toàn đối với người dùng
            - Tốc độ lượt web ổn định và hỗ trợ đầy đủ tính năng cơ bản
            - Điều hướng web nhanh chóng
            - Rất nhiều extension
        * Nhược điểm:
            - Landing page nhiều quảng cáo
            - Di chuyển không mượt mà như các trình duyệt khác
            - Update phiên bản không thông minh
    * **Microsoft Edge**:
        * Ưu điểm:
            - Tương thích với hầu hết mọi nền tàng
            - Hỗ trợ tiện ích mở rộng tương tự Chrome
            - Chế độ đọc tích hợp
            - Không ngốn RAM như Chrome
        * Nhược điểm:
            - Trình duyệt có thể treo khi các trang có quá nhiều quảng cáo
            - Load video nhúng chậm
            - Máy tính cấu hình mạnh mới mở được nhiều tab
    * **Safari**: tương thích với hệ điều hành MacOS, iOS
        * Ưu điểm:
            - Có sẵn trên các sản phẩm của Apple
            - Dấu trang và lịch sử đồng bộ trên thiết bị cùng ID Apple
            - Tải trang web nhanh
        * Nhược điểm:
            - Không tùy chỉnh được thanh công cụ
            - Không tương thích với hệ điều hành Windows, Android
    * **Opera**:
        * Ưu điểm:
            - Tùy chỉnh giao diện trình duyệt
            - Trình chặn quảng cáo tích hợp
            - Bảo mật cao
        * Nhược điểm:
            - Ít plugin hơn các trình duyệt khác
            - Không vào các trang web quá cũ


## 4. Cơ chế hoạt động của DNS và domain
* **Domain** hay còn gọi là tên miền là địa chỉ đại diện của một trang web giúp định vị và điều hướng người dùng đến đúng máy chủ (web server) của trang web muốn truy cập. Một tên miền có tối thiểu 2 phần cách nhau bởi dấu chấm (.) là: Top Level Domain và Second Level Domain (ví dụ: www.google.com => *www* là Subdomain, *google* là SLD, *com* là TLD). 
    * Cơ chế hoạt động: Khi nhập domain name vào thanh URL của trình duyệt web, trình duyệt gửi yêu cầu truy cập đến DNS, tại đây DNS tìm kiếm và trả về địa chỉ IP của máy chủ của trang web. Trình duyệt sẽ sử dụng địa chỉ này để truy cập máy chủ của trang web và máy chủ sẽ trả về nội dung của trang web để hiển thị lên trình duyệt.
* **DNS (Domain name system)** còn gọi là hệ thống phân giải tên miền là một hệ thống giúp con người và máy tính có thể "giao tiếp" với nhau một cách dễ dàng hơn, hệ thống biên dịch tên miền (hostname) thành dãy số để máy tính có thể hiểu. DNS có chức năng ghi nhớ tên miền đã phân giải, giúp những lần truy cập tới nó sẽ ưu tiên sử dụng, giúp cho người dùng sử dụng nhanh chóng và dễ dàng hơn.
    * Cơ chế hoạt động: hoạt động dựa theo cấu trúc truy vấn để lấy thông tin gọi là *DNS query*. Đầu tiên, máy chủ DNS sẽ tự động tìm kiếm thông tin đã phân giải tại file hosts của hệ điều hành (chịu trách nhiệm chuyển hostname thành địa chỉ IP). Nếu không thấy thông tin DNS sẽ tiếp tục tìm kiếm tại bộ nhớ cache. Nếu không nhận được bất kì thông tin nào DNS hiển thị mã lỗi.

## 5. Giải thích về hosting server
- Server Hosting là đề cập đến việc quản lý offsite và duy trì các tài nguyên phần cứng được chỉ định cho việc sử dụng của công ty thông qua hình thức trả phí hàng tháng cho dịch vụ hosting. Qua đó công ty có thể có được cơ sở hạ tầng công nghệ thông tin đầy đủ mà không phải trả chi phí liên quan đến bảo trì, đào tạo và cập nhật thiết bị (bao gồm phần cứng server, thuê nhân viên IT). Dịch vụ hosting đảm bảo mọi thứ để chắc chắn máy chủ luôn sẵn sàng khi cty cần mà không cần phải lo lắng đến việc bảo trì phần cứng, duy trì hoạt đồng hay khắc phục sự cố ... 
- Giải pháp Server Hosting bao gồm máy chủ riêng (managed hosting), máy chủ riêng ảo, máy chủ chuyên dụng


