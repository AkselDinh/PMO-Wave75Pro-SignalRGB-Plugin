# PMO/WOB Wave75 Pro RGB (Womier RD75) - SignalRGB Plugin
*[Phiên bản Tiếng Việt ở bên dưới](#phiên-bản-tiếng-việt)*

A custom SignalRGB plugin for the **PMO/WOB Wave75 Pro** keyboard. This project is the result of reverse engineering the keyboard's HID protocol with Wireshark to enable custom RGB streaming by intercepting "Aurora" effect in the PMO Hub application.

## Works seamlessly without requiring the official PMO Hub

## ⚠️ Important Notes & Known Issues
- **Womier RD75 Compatibility:** The PMO Wave75 Pro shares the exact same hardware and PCB as the **Womier RD75**. It should theoretically work, but is untested. If you want to try it on an RD75, use Windows Device Manager to find your RD75 specific `VID` and `PID`, and replace those values at the top of the `.js` plugin file.
- **Caps Lock Double LEDs:** The keyboard has 81 physical switches but SignalRGB may recognize 82 LEDs. This is because Caps Lock key uniquely utilizes two independent LEDs (Indices 45 & 46) instead of 1.
- **Random LED Flashes (Hardware Glitch):** You may occasionally see random keys flash for a split second. This is a known hardware/firmware quirk, not related to this plugin and cannot be fully fixed via software.
- **Logo LED:** The Logo LED is currently not supported by this plugin.
- **QMK Firmware:** This plugin was reverse-engineered on the stock firmware. It has **NOT** been tested on boards flashed with QMK/VIA.
- **Connectivity:** Only Wired USB connection is supported. Bluetooth mode and 2.4G is not supported with this plugin.

## Installation
1. Download the `Wave75ProRGB.js` plugin file from this repository.
2. Navigate to your SignalRGB Plugins folder: `Documents\WhirlwindFX\Plugins` (or `Documents\SignalRGB\Plugins`).
3. Paste the `.js` file into that folder.
4. **Important:** Completely close the official PMO Hub software (ensure it is not running in the System Tray).

---

# Phiên bản Tiếng Việt

Plugin SignalRGB tùy chỉnh cho bàn phím **PMO/WOB Wave75 Pro RGB**. Dự án này là kết quả của quá trình dịch ngược giao thức HID bằng phần mềm Wireshark, cho phép truyền dữ liệu LED RGB tùy chỉnh bằng cách khai thác hiệu ứng "Aurora" trong ứng dụng PMO Hub.

## Hoạt động ổn định mà không cần phần mềm PMO Hub chính thức

## ⚠️ Lưu ý Quan trọng & Các vấn đề đã biết
- **Khả năng tương thích với Womier RD75:** PMO Wave75 Pro sử dụng chung phần cứng và bảng mạch (PCB) với **Womier RD75**. Về lý thuyết, plugin có thể hoạt động trên bàn phím này nhưng chưa được test thực tế. Nếu bạn muốn thử trên RD75, hãy mở Windows Device Manager để tìm mã `VID` và `PID` của bàn phím của bạn, sau đó thay thế các giá trị tương ứng ở phần khai báo đầu file plugin `.js`.
- **Bóng LED kép ở phím Caps Lock:** Bàn phím có 81 phím vật lý nhưng SignalRGB nhận 82 phím. Lý do là vì phím Caps Lock có đến hai đèn LED độc lập (Index 45 và 46) thay vì chỉ 1 đèn.
- **Hiện tượng nháy đèn ngẫu nhiên (Lỗi phần cứng):** Trong quá trình sử dụng, một vài phím có thể nháy sáng đột ngột trong tích tắc với màu sắc ngẫu nhiên. Đây là lỗi có sẵn của phần cứng/firmware, không liên quan đến plugin này và không thể khắc phục hoàn toàn bằng phần mềm.
- **LED Logo:** Đèn LED Logo hiện chưa được hỗ trợ trong plugin này.
- **Firmware QMK:** Plugin được dịch ngược dựa trên firmware gốc. **CHƯA ĐƯỢC THỬ NGHIỆM** trên các bàn phím đã flash firmware QMK/VIA.
- **Kết nối:** Chỉ hỗ trợ kết nối có dây. Bluetooth và 2.4G không được hỗ trợ.

## Hướng dẫn Cài đặt
1. Tải file plugin `Wave75ProRGB.js` từ repository này.
2. Truy cập vào thư mục Plugins của SignalRGB theo đường dẫn: `Documents\WhirlwindFX\Plugins` (hoặc `Documents\SignalRGB\Plugins`).
3. Sao chép tệp `.js` vào thư mục trên.
4. **Quan trọng:** Tắt hoàn toàn phần mềm PMO Hub (đảm bảo ứng dụng không còn chạy ngầm trong khay hệ thống - System Tray).