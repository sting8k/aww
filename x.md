

# New Features v3.0 !
  - Thay đổi ngôn ngữ từ **Python** sang **Golang** với khả năng xử lý **multithreads**. 
  - Tốc độ được cải thiện nhanh gấp **~2x** - **5x** lần
  - Tối ưu tập luật, sử dụng `parser` cho kết quả đẹp và giảm tương đối *False positive*. Đặc biệt với ngôn ngữ `PHP`
  - Menu người dùng gọn và dễ sử dụng.
  - Thêm tính năng dump source code các file bị nghi ngờ (thay vì dump toàn bộ webroot như `v2`)
  - Sửa lỗi chức năng tự động **phát hiện Webserver đang chạy** và **lấy Webroot**
  - Sửa một số lỗi khi lưu kết quả ra file `csv`

### Requirements

Hỗ trợ các hệ điều hành sau:
- Windows `32-bit`, `64-bit`
- Centos `>= 6.0`  `32-bit`, `64-bit` hoặc các distro có phiên bản kernel tương tự.

Không hỗ trợ
- Centos `<= 5.0` (Có thể tạm sử dụng v2)

### Menu sử dụng


| MODE: | 1. Auto | 2. Manual | Ghi chú |
|--|--|--|--|
| Tự phát hiện Webserver | `IIS`, `Apache`, `Nginx`, `Weblogic`, `Jboss`, `Tomcat` | Không có | (Yêu cầu **Root permission**)
| Tự lấy Webroot | `IIS`, `Apache`, `Nginx` | Không có | (Yêu cầu **Root permission**)
|Quét theo extensions|Tất cả / Tự gợi ý / Tùy chỉnh| = | Tự gợi ý: Lấy từ tập luật trong DB
|Quét theo loại ngôn ngữ|Tất cả / Tự gợi ý / Tùy chỉnh| = | Tự gợi ý: Lấy từ tập luật trong DB
|Dump files| Tùy chỉnh (*Enable* hoặc *Disable*) | = | Mặc định: **Enable**
|Threads| Tùy chỉnh | = | Mặc định: `2 threads`.  Nên sử dụng ít hơn `10 threads`.
|Output CLI| Chỉ hiện thị đường dẫn file nghi ngờ | = | Thông tin chi tiết được lưu ra file output.

`=` : Như bên cạnh


### Screenshot

![enter image description here](https://github.com/sting8k/aww/blob/master/ShellScreenshot.PNG?raw=true)



### Todos

 - Thêm chức năng dump `MFT Record` để hỗ trợ việc tra cứu files bị thay đổi `ctime`
 - Bổ sung tự động lấy Webroot từ các java-based Webservers
 - Fix bugs

License
----

VCS
**Free Software, Hell Yeah!**

