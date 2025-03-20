ShoeShop

1. Backend
C# & ASP.NET: Ngôn ngữ lập trình chính và framework để xây dựng ứng dụng web theo mô hình MVC (Model-View-Controller), giúp quản lý logic nghiệp vụ, xử lý yêu cầu từ người dùng và hiển thị dữ liệu.
Entity Framework (EF): ORM (Object-Relational Mapping) giúp thao tác với cơ sở dữ liệu SQL Server một cách dễ dàng bằng cách sử dụng Code First hoặc Database First.
WebSocket & SignalR: Hỗ trợ giao tiếp thời gian thực giữa server và client, dùng để cập nhật đơn hàng, chat trực tuyến, và thông báo tự động.
Send Mail (SMTP, MailKit): Gửi email xác nhận đơn hàng, thông báo giao dịch hoặc marketing qua SMTP.
PayPal API: Tích hợp cổng thanh toán trực tuyến, hỗ trợ xử lý đơn hàng và giao dịch an toàn.
2. Frontend
HTML, CSS, JavaScript: Xây dựng giao diện trang web thân thiện với người dùng.
Bootstrap: Framework hỗ trợ thiết kế giao diện responsive, tương thích trên nhiều thiết bị.
jQuery / AJAX: Cải thiện trải nghiệm người dùng bằng cách tải dữ liệu động mà không cần tải lại trang.
3. Cơ sở dữ liệu
SQL Server: Hệ quản trị cơ sở dữ liệu quan hệ (RDBMS) được sử dụng để lưu trữ thông tin sản phẩm, đơn hàng, người dùng.
Entity Framework (EF Core): Quản lý truy vấn dữ liệu một cách hiệu quả, hỗ trợ LINQ để làm việc với database dễ dàng hơn.
4. Bảo mật & Xác thực
ASP.NET Identity: Hỗ trợ quản lý tài khoản, đăng nhập, phân quyền người dùng (Admin, Khách hàng).
JWT: Xác thực bảo mật khi giao tiếp API.
5. Triển khai & Quản lý
IIS (Internet Information Services): Máy chủ web của Microsoft để chạy ứng dụng ASP.NET.
Docker: Container hóa ứng dụng giúp triển khai linh hoạt hơn.

Hướng dẫn chạy dự án
1. Yêu cầu hệ thống
Hệ điều hành: Windows 10/11
Phần mềm cần cài đặt:
.NET SDK: Tải tại đây
SQL Server: Tải tại đây
Visual Studio (Phiên bản hỗ trợ .NET & SQL Server): Tải tại đây
Docker (Nếu sử dụng container hóa): Tải tại đây
2. Cài đặt và chạy Backend
Bước 1: Clone source code từ repository:
sh
Sao chép
Chỉnh sửa
git clone <link-repository>
cd <tên-thư-mục-dự-án>
Bước 2: Cấu hình kết nối database trong appsettings.json:
json
Sao chép
Chỉnh sửa
"ConnectionStrings": {
  "DefaultConnection": "Server=YOUR_SERVER;Database=YOUR_DATABASE;User Id=YOUR_USER;Password=YOUR_PASSWORD;"
}
Bước 3: Chạy migration để khởi tạo database:
sh
Sao chép
Chỉnh sửa
dotnet ef database update
Bước 4: Chạy ứng dụng:
sh
Sao chép
Chỉnh sửa
dotnet run
Bước 5: API sẽ chạy tại http://localhost:5000 hoặc https://localhost:5001 nếu có SSL.
