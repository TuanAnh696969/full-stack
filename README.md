# Node.js Express – Web Api
# Build Node.js Rest Apis with Express and databases.
# Node.js Express & PostgreSQL: CRUD Rest APIs ví dụ với Sequelize.

Express là một trong những khung web phổ biến nhất dành cho Node.js hỗ trợ định tuyến, phần mềm trung gian, hệ thống xem… Sequelize là một ORM Node.js dựa trên lời hứa hỗ trợ các phương ngữ cho PostgreSQL, MySQL, SQL Server… Trong hướng dẫn này, tôi sẽ chỉ cho bạn từng bước xây dựng Node.js Restful CRUD API sử dụng Express, Sequelize với cơ sở dữ liệu PostgreSQL

Chúng tôi sẽ xây dựng Rest Apis có thể tạo, truy xuất, cập nhật, xóa và tìm.
Đầu tiên, chúng tôi bắt đầu với một máy chủ web Express. Tiếp theo, chúng tôi thêm cấu hình cho cơ sở dữ liệu PostgreSQL, tạo mô hình Hướng dẫn với Sequelize, viết bộ điều khiển. Sau đó, chúng tôi xác định các tuyến để xử lý tất cả các hoạt động CRUD (bao gồm cả công cụ tìm tùy chỉnh).

#
Bảng sau đây hiển thị thông tin tổng quan về các API còn lại sẽ được xuất:



Cuối cùng, chúng ta sẽ kiểm tra Rest Apis bằng Postman.

# khởi tạo Ứng dụng Node.js bằng tệp pack.json
npm init

# cần cài đặt các module cần thiết:express, sequelize, pg, pg-hstore
npm install express sequelize pg pg-hstore cors --save

*pg cho PostgreSQL và pg-hstore để chuyển đổi dữ liệu sang định dạng hstore PostgreSQL.

# Chạy ứng dụng bằng lệnh
node server.js
