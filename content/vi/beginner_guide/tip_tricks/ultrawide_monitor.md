---
title: "Màn hình Ultrawide 21:9"
linkTitle: "Màn hình Ultrawide 21:9"
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

Màn hình WFHD cho tầm quan sát rộng gấp 2 màn hình FHD. Trong pvp, màn hình rộng giúp cho bạn quan sát đối thủ tốt hơn, di chuyển tốt hơn. Trong pve, quan sát map, boss tốt hơn. Nếu bạn đã có cho mình màn hình 21:9 thì không cần lo lắng gì cả. Tuy nhiên, nếu không có thì hướng dẫn sau đây sẽ giúp bạn thêm custom resolution vào Option của Elsword.

## Cài đặt trên card màn hình rời (dGPU)

Cách này dùng cho các máy tính để bàn (Desktop) có sử dụng card màn hình rời.

Hưỡng dẫn sau sẽ hướng dẫn các bạn setup trên card màn hình rời NVIDIA còn AMD thì các bạn xem thêm ở [đây nhé](https://www.amd.com/en/support/kb/faq/dh-032)

### Mở NVIDIA Control Panel

Chuột phải lên màn hinh desktop

{{< imgproc2 nvidia_control_panel >}}

### Vào phần Display > Change resolution

{{< imgproc2 nvidia_change_resolution >}}

### Chọn Customize > Create Custom Resolution

{{< imgproc2 nvidia_customize >}}

### Cài đặt custom resolution

Ở đây bạn điền resolution mong muốn vào

{{< imgproc2 nvidia_create_custom >}}

Những resolution cho độ phân giải 21:9:
- 1920x820 (thông dụng)
- 2560x1080 (thông dụng)
- 2880×1200
- 3440×1440

Xem thêm [Ultrawide resolution](https://en.wikipedia.org/wiki/Ultrawide_formats)

**Lưu ý**: Bạn có thể set như nào cũng được không nhất thiết phải là ultrawide. Tuy nhiên, **tuyệt đối không set độ phân giải quá lớn so với màn hình của bạn hỗ trợ**. E.g. Màn hình bạn đang xài 1920x1080, bạn customize lên 5120×2160 thì khả năng cao là die cái màn hình. Đối với màn hình 1920x1080 thì bạn customize thành 1920x800 là được.

## Cài đặt trên card màn hình tích hợp (iGPU)

Cách này dùng cho các máy laptop hoặc desktop sử dụng card màn hình tích hợp.

### Download Custom Resolution Utility

Download [Custom Resolution Utility](https://custom-resolution-utility.en.lo4d.com/windows). App này dùng được cho cả iGPU AMD và NVIDIA.

Trong trường hợp gặp sự cố không set được custom resolution trên APU của AMD, bạn tham khảo thêm [Radeon Custom Reolution Manager](https://www.softpedia.com/get/System/System-Miscellaneous/RCRM.shtml)

### Cài đặt custom resolution

Những resolution cho độ phân giải 21:9:
- 1920x820 (thông dụng)
- 2560x1080 (thông dụng)
- 2880×1200
- 3440×1440

Refresh rate thích hợp:
- 60 Hz (thông dụng)
- 80 Hz: Nếu màn hình của bạn hỗ trợ refresh rate lớn hơn 80 thì nên set 80 Hz

Restart máy sau khi cài đặt xong.

{{< imgproc2 cru.png >}}

## Cài đặt resolution trên elsword

Sau khi cài đặt xong custom resolution thì mở elsword lên. Custom resolution sẽ xuất hiện trong option của game. Sau khi chọn resolution thì hãy **bật fullscreen**, custom resolution **không có tác dụng trong window mode**.

{{< imgproc2 in_game_option >}}