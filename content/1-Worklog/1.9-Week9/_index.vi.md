---
title: "Worklog Tuần 9"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---



### Mục tiêu tuần 9:
* Tìm hiểu vai trò của Amazon S3 và AWS Storage Gateway trong quá trình lưu trữ và di chuyển dữ liệu trên AWS.
* Tạo S3 Bucket để lưu trữ dữ liệu và phục vụ cho các bước thực hành tiếp theo.
* Cấu hình các thiết lập cơ bản cho S3 Bucket, bao gồm tên bucket, khu vực (Region) và quyền truy cập phù hợp.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6   | -   Tạo bucket S3          | 12/06/2025   | 12/06/2025      |<https://000024.awsstudygroup.com/1-prepare/1.1-creates3/>
| 7   | -       Tạo EC2 cho Storage Gateway                                   | 13/06/2025   | 13/06/2025      | <https://000024.awsstudygroup.com/1-prepare/1.2-createstoragegwinstance/> |
| 2   | -  Sử dụng AWS Storage Gateway| 15/06/2025   | 15/06/2025      | <https://000024.awsstudygroup.com/2-useawsstoragegw/> |
| 3   | -        Tạo AWS Storage Gateway        | 16/06/2025   | 16/06/2025      | <https://000024.awsstudygroup.com/2-useawsstoragegw/2.1-createstoragegw/> |
| 4   | -       Tạo các thư mục chia sẻ                                      | 17/06/2025   | 17/06/2025      | <https://000024.awsstudygroup.com/2-useawsstoragegw/2.2-createfileshare/> |
| 5   | - Gắn kết (Mount) các thư mục chia sẻ trên máy On-premises             | 18/06/2025   | 18/06/2025      | <https://000024.awsstudygroup.com/2-useawsstoragegw/2.3-mountfileshare/> |

### Kết quả đạt được tuần 9:

* Tạo thành công Amazon S3 Bucket để lưu trữ dữ liệu trên AWS
* Hoàn thành cấu hình cơ bản cho S3 Bucket theo yêu cầu của bài thực hành
* Khởi tạo thành công EC2 Instance từ AMI Storage Gateway do AWS cung cấp
* Ảnh minh họa:
* 
{{< figure src="/images/1-Worklog/1.9-Week9/createS3.png" title="Tạo bucket S3" >}}