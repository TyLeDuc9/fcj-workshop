---
title: "Worklog Tuần 5"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---



### Mục tiêu tuần 5:

* Triển khai AWS Backup vào hệ thống.
* Học cách khôi phục dữ liệu từ bản sao lưu và tự động hóa toàn bộ quy trình.
* Thông báo kiểm tra khi các quy trình hoàn tất.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6   | - Tạo nhóm lưu trữ S3  <br> - Triển khai cơ sở hạ tầng                                                                                | 15/05/2026   | 15/05/2026   | <https://000013.awsstudygroup.com/2-prerequiste/2.1-creates3bucket/>   |
| 7   | - Lập kế hoạch dự phòng                                         | 16/05/2026   | 16/05/2026      | <https://000013.awsstudygroup.com/3-createbackupplan/> |
| 2   | - Thiết lập thông báo | 18/05/2026   | 18/05/2026      | <https://000013.awsstudygroup.com/4-enablenoti/> |
| 3   | - Kiểm tra khôi phục               | 19/05/2026   | 19/05/2026      | <https://000013.awsstudygroup.com/5-testrestore/> |
| 4   | - Sử dụng Cổng Lưu trữ Tệp               | 20/05/2026   | 20/05/2026      | <https://000024.awsstudygroup.com/2-prerequiste/> |
| 5   | - Sử dụng AWS Storage Gateway               | 21/05/2026   | 21/05/2026      | <https://000024.awsstudygroup.com/2-useawsstoragegw/> |



### Kết quả đạt được tuần 5:
* Tạo thành công nhóm lưu trữ Amazon S3 để phục vụ sao lưu dữ liệu hệ thống.
* Triển khai cơ sở hạ tầng AWS Backup và cấu hình Backup Vault.
* Thiết lập thông báo bằng Amazon SNS nhằm theo dõi trạng thái backup và restore.
* Làm quen với AWS Storage Gateway và File Gateway để kết nối lưu trữ giữa môi trường local và AWS.
* Hiểu được quy trình tự động hóa backup, restore và giám sát hệ thống trên AWS.
* Ảnh minh họa:

{{< figure src="/images/1-Worklog/1.5-Week5/createS3Bucket.png" title="Tạo nhóm lưu trữ S3" >}}
{{< figure src="/images/1-Worklog/1.5-Week5/createFolder.png" title="Tạo thư mục" >}}
{{< figure src="/images/1-Worklog/1.5-Week5/uploadFile.png" title="Tải lên tập tin" >}}
{{< figure src="/images/1-Worklog/1.5-Week5/permissions.png" title="Chặn quyền truy cập công khai" >}}
{{< figure src="/images/1-Worklog/1.5-Week5/editPolicy.png" title=" Chỉnh sửa chính sách nhóm lưu trữ" >}}
{{< figure src="/images/1-Worklog/1.5-Week5/createBackUp.png" title="Tạo kế hoạch sao lưu" >}}
{{< figure src="/images/1-Worklog/1.5-Week5/testRestore.png" title="Kiểm tra khôi phục" >}}
{{< figure src="/images/1-Worklog/1.5-Week5/createStorageGateway.png" title="Tạo Cổng lưu trữ" >}}