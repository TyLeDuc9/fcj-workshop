---
title: "Worklog Tuần 4"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:

* Thiết lập kết nối VPC Peering.
* Thiết lập AWS Transit Gateway.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6   | - Khởi tạo mẫu CloudFormation <br> - Tạo nhóm bảo mật <br> - Tạo phiên bản EC2                                                                                          | 08/05/2026   | 08/05/2026  | <https://000019.awsstudygroup.com/2-prerequiste/>
| 7   | - Cập nhật ACL mạng <br> - Kết nối VPC  <br> - DNS giữa các máy ngang hàng                                     | 09/05/2026   | 09/05/2026      | <https://000019.awsstudygroup.com/3-updatenetworkacl/> |
| 2   | - Thiết lập AWS Transit Gateway <br> - Tạo Cổng trung chuyển | 11/05/2026   | 11/05/2026      | <https://000020.awsstudygroup.com/1-introduce/> |
| 3   | - Tạo tệp đính kèm cổng trung chuyển <br> - Tạo bảng tuyến đường cổng trung chuyển                  | 12/05/2026   | 12/05/2026      | <https://000020.awsstudygroup.com/4-transigatewayattachments/> |
| 4   | - Thêm các tuyến Transit Gateway vào bảng định tuyến VPC                          | 13/05/2026   | 13/05/2026      | <https://000020.awsstudygroup.com/6-result/> |


### Kết quả đạt được tuần 4:

* Hiểu được cách thiết lập  AWS Transit Gateway và kết nối VPC Peering: 
  * Cập nhật Route Table, Network ACL và DNS để đảm bảo kết nối hoạt động
  * Tạo và cấu hình AWS Transit Gateway
  * Thêm các tuyến vào bảng định tuyến của VPC
  * Kiểm tra kết nối giữa các EC2 trong các VPC khác nhau
  * Nắm được sự khác biệt giữa VPC Peering và AWS Transit Gateway
* Ảnh minh họa:

{{< figure src="/images/1-Worklog/1.4-Week4/createVPC.png" title="Tạo VPC" >}}
{{< figure src="/images/1-Worklog/1.4-Week4/createHGVPC.png" title="Tạo nhóm bảo mật HG VPC" >}}
{{< figure src="/images/1-Worklog/1.4-Week4/createEC2.png" title="Tạo phiên bản EC2" >}}
{{< figure src="/images/1-Worklog/1.4-Week4/updateACL.png" title="Cập nhật ACL mạng" >}}
{{< figure src="/images/1-Worklog/1.4-Week4/connectVPC.png" title="Kết nối VPC" >}}
{{< figure src="/images/1-Worklog/1.4-Week4/createKeypair.png" title="Tạo cặp khóa" >}}
{{< figure src="/images/1-Worklog/1.4-Week4/createTransitGateway.png" title="Tạo Cổng trung chuyển" >}}
{{< figure src="/images/1-Worklog/1.4-Week4/createGatewayRoute.png" title="Tạo bảng tuyến đường cổng trung chuyển" >}}