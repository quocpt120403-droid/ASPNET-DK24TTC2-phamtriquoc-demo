## Mô tả cơ bản các chức năng
Đây là một hệ thống website tuyển dụng việc làm được phát triển bằng ASP.NET Core MVC (phiên bản .NET 8.0), sử dụng SQL Server làm cơ sở dữ liệu. Website cho phép người tìm việc, nhà tuyển dụng, và admin tương tác để tìm kiếm việc làm, đăng tin tuyển dụng, quản lý hồ sơ và duyệt tin
---Phân quyền:
Nhà tuyển dụng
Người tìm việc
Admin
---Đối với người tìm việc
Đăng ký/ Đăng nhập
Tìm kiếm việc làm
Xem danh sách việc làm
Ứng tuyển việc làm
Xem trạng thái ứng tuyển
Upload CV cá nhân
Chỉnh sửa thông tin cá nhân
Nhận mail báo kết quả và mail gọi đi phỏng vấn
---Đối với nhà tuyển dụng
Đăng ký/ Đăng nhập
Đăng ký tên công ty (nộp hồ sơ giấy phép kinh doanh, mã số thuế, ảnh công ty,…)
Chỉnh sửa công ty
Đăng tin tuyển dụng
Xem các ứng viên ứng tuyển vào công việc
Gửi mail báo kết quả trúng tuyển
Gửi mail gọi phỏng vấn (có thể tạo phỏng vấn online/offline)
Xem CV ứng viên
---Đối với Admin
Đăng nhập
Quản lý tài khoản user
Xem danh sách và duyệt yêu cầu của các nhà tuyển dụng đăng ký
Xem và chỉnh sửa phiếu đăng tuyển dụng
## Import file SQL
-B1 import file vào sql sever phiên bản 2019 trở lên

-B2 Thay đổi đường dẫn local vào file web.config
Đoạn code  
  <connectionStrings>
   <add name="TuyenDungDbContext" connectionString="data source=智国;initial catalog=Career;Trusted_Connection=True;" providerName="System.Data.SqlClient" />
 </connectionStrings> trong đó data source=智国 sẽ thay thành sever name của database sql trên máy bạn.

-B3 Buid and Run
Thông tin đăng nhập Admin1@gmail.com pass 123456Aa@ và ungvien2@gmail.com pass 123456Aa@
các tài khoản ứng viên và nhà tuyển dụng có thể đăng ký mới rồi đăng nhập
