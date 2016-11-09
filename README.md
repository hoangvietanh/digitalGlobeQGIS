# Cách mở ảnh Digital Globe trong QGIS sử dụng Digital Globe API

## Bước 1: đăng ký tài khoản tại địa chỉ https://mapsapi.digitalglobe.com
Bạn sẽ được yêu cầu cung cấp email, mật khẩu. Sau đó tài khoản sẽ được verify thông qua email. Thao tác thông thường như khi đăng ký tài khoản tại các trang khác.

## Bước 2: lấy token
Sau khi đã có tài khoản bạn hãy vào trang dưới đây để copy mã token
https://mapsapi.digitalglobe.com/account

### Bước 3: tạo đường link WMS để sử dụng cho QGIS
Các bước để tạo đường link WMS được hướng dẫn tại đây http://mapsapidocs.digitalglobe.com/v1.0/docs/maps-api-qgis-desktop-map-style
Cụ thể như sau:
- Mở QGIS
- Mở mục Add WMS layer (mục thứ 8 trên thanh công cụ add layers)
- Chọn New để cấu hình 1 kết nối WMS mới
- Trong mục Name gõ "DG Maps API Recent Imagery" hoặc tên tùy chọn
- Trong mục URL gõ http://api.mapbox.com/styles/v1/digitalglobe/ciode6t5k0081aqm7k06dod4v/wmts?access_token=
- Sau dấu = paste token đã được lưu ở bước 2. Đóng cửa sổ tạo WMS mới lại --> tại của sổ chính của Add WMS layer ta đã có tên của WMS vừa tạo
- Chọn connect tới WMS layer đó --> ảnh Digital Globe đã được add vào phiên làm việc QGIS của bạn

Các bước nói trên có thể xem video tại link sau
http://screencast.com/t/xRVHldcRc7uS
