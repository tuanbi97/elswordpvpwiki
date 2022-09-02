---
title: "Màn hình Ultrawide"
linkTitle: "Màn hình Ultrawide"
weight: 1
description: >
  Trick này dùng để tăng phạm vi quan sát của màn hình.
---

## Tổng quan

Trước hết chúng ta hãy cùng so sánh 2 độ phân giải màn hình sau:
- Resolution FHD: 1920x1080 chuẩn của Elsword
{{< imgproc2 1920_1080 >}}

- Resolution WFHD (21:9): 2560x1080
{{< imgproc2 2560_1080 >}}

Màn hình WFHD cho tầm quan sát rộng gấp 2 màn hình FHD. Trong pvp, màn hình rộng giúp cho bạn quan sát đối thủ tốt hơn, di chuyển tốt hơn. Trong pve, quan sát map, boss tốt hơn. Nếu bạn đã có cho mình màn hình 21:9 thì không cần lo lắng gì cả. Tuy nhiên, nếu không có thì hướng dẫn sau đây sẽ giúp bạn điều chỉnh độ phân giải của Elsword tùy ý muốn.

## Cài đặt Borderless Gaming

Download từ github: https://github.com/Codeusa/Borderless-Gaming

Vào mục release, download borderless gaming về và cài đặt

## Cài đặt độ phân giải Ultrawide

1. Mở game Elsword
2. Mở Borderless gaming

Bạn sẽ thấy Elsword xuất hiện trong danh sách Applications của Borderless Gaming (khung bên trái). Click chuột vào sau đó bấm mũi tên để đưa Elsword vào danh sách favorite

{{< imgproc2 borderless_gaming_config_1 >}}

3. Chuột phải chọn No Size Change

{{< imgproc2 borderless_gaming_config_2 >}}

4. Chuột phải vào lần nữa chọn Set Window Size.

{{< imgproc2 borderless_gaming_config_3 >}}

5. Chọn **No** để nhập độ phân giải mong muốn vào. Hoặc chọn **Yes** sau đó vẽ một khung chữ nhật lên màn hình để xác định độ phân giải mới.

6. Ở đây mình chọn **No**, app sẽ yêu cầu nhập 4 số:
- Giá trị trục X và giá trị trục Y: 2 điểm này nhằm xác định vị trí bắt đầu của window.
- Width và Height: Resolution của window
7. Các resolution thông dụng
Quy tắc: Tỉ lệ Width / Height càng lớn thì window càng dài.
- 1920x800
- 1920x600
- 2560x1080
- 2560x800

**Lưu ý**: Bạn có thể set như nào cũng được. Tuy nhiên, **tuyệt đối không set độ phân giải quá lớn so với màn hình của bạn hỗ trợ**. E.g. Màn hình bạn đang xài 1920x1080, bạn customize lên 5120×2160 thì khả năng cao là die cái màn hình. Đối với màn hình 1920x1080 thì bạn customize thành 1920x800 là được.

8. Sau khi đã set xong resolution, chọn vào nút như hình. App sẽ điều chỉnh Elsword về resolution đã set.

{{< imgproc2 borderless_gaming_config_4 >}}

9. Sau khi đã cài đặt xong, những lần sau khi bạn mở game và borderless gaming, app sẽ tự động chỉnh game về resolution bạn đã set. Trong trường hợp chưa hài lòng với resolution đã set thì quay lại bước 4.