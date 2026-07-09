---
title: "Worklog Tuần 7"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---


### Mục tiêu tuần 7:

* Tạo bucket S3
* Quản lý kế hoạch sao lưu (Backup Plan) cho các tài nguyên trên AWS

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6   | -  Tạo S3 Bucket             <br>- Triển khai hạ tầng                                                                  | 29/05/2026   | 29/05/2026      |<https://000013.awsstudygroup.com/2-prerequiste/2.1-creates3bucket/>
| 7   | -  Tạo kế hoạch sao lưu                                         | 30/05/2026   | 30/05/2026      | https://000013.awsstudygroup.com/3-createbackupplan/> |
| 2   | - Thiết lập thông báo| 01/06/2026   | 01/06/2026      | <https://000013.awsstudygroup.com/4-enablenoti/> |
| 3   | - Kiểm tra khôi phục dữ liệu                 | 02/06/2026   | 02/06/2026      | <https://000013.awsstudygroup.com/5-testrestore/>
| 4   | -  Xuất (Export) máy ảo từ môi trường tại chỗ (On-premises).             | 03/06/2026   | 03/06/2026      | <https://000014.awsstudygroup.com/2-import-vm-to-aws/1-export-vm-from-virtual-env/> |
| 5   | - Tải (Upload) máy ảo lên AWS              | 04/06/2026   | 04/06/2026      | <https://000014.awsstudygroup.com/2-import-vm-to-aws/2-upload-vm-to-aws/> |

### Kết quả đạt được tuần 7:

* Hiểu được cách sử dụng AWS Backup để tạo và quản lý kế hoạch sao lưu (Backup Plan) cho các tài nguyên trên AWS.
* Thiết lập thành công Backup Plan nhằm tự động hóa quá trình sao lưu dữ liệu.
* Thực hiện thành công quá trình backup và restore, xác nhận dữ liệu có thể được khôi phục khi cần thiết.
* Ảnh minh họa:


{{< figure src="/images/1-Worklog/1.7-Week7/createS3.png" title="Tạo bucket S3" >}}
{{< figure src="/images/1-Worklog/1.7-Week7/createPlan.png" title="Tạo  folder" >}}
{{< figure src="/images/1-Worklog/1.7-Week7/backupPlan.png" title="Lập kế hoạch dự phòng" >}}

