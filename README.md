# DataDid_Auto_Daily
==========================================================================
        HƯỚNG DẪN CÀI ĐẶT & SỬ DỤNG METAMEMO SMART BOT (DELUXE)
==========================================================================

1. YÊU CẦU HỆ THỐNG
-------------------
- Đã cài đặt Node.js (Phiên bản mới nhất hoặc LTS).
- Máy tính có kết nối Internet ổn định.

2. CÀI ĐẶT THƯ VIỆN (MỞ TERMINAL/CMD VÀ CHẠY LỆNH SAU)
------------------------------------------------------
npm install fs-extra axios ethers chalk@4.1.2 moment https-proxy-agent socks-proxy-agent readline-sync node-machine-id

3. DANH SÁCH VÀ CHỨC NĂNG CÁC FILE CẤU HÌNH
-------------------------------------------
Bạn cần tạo các file .txt sau trong cùng thư mục với file p2.js:

- mail.txt (BẮT BUỘC): Chứa danh sách mail.
  Định dạng: email|password|mail_token
  (mail_token lấy từ mail.tm để tool tự nhận OTP nếu cần).

- ref.txt (BẮT BUỘC): Chứa mã mời (Referral Code). 
  Mỗi dòng 1 mã, tool sẽ lấy xoay vòng để bind.

- proxy.txt (TÙY CHỌN): Chứa danh sách proxy.
  Định dạng: http://user:pass@ip:port hoặc socks5://user:pass@ip:port
  Nếu không có, tool sẽ chạy bằng IP máy (không khuyến khích chạy nhiều acc).

- User_agents.txt (TÙY CHỌN): Chứa danh sách User Agent. 
  Mỗi dòng 1 UA để giả lập trình duyệt.

- license.txt (TỰ ĐỘNG): 
  Lần đầu chạy tool sẽ yêu cầu nhập Key. Key sau đó sẽ được lưu vào file này.

4. CÁC FILE DỮ LIỆU ĐẦU RA (TOOL TỰ TẠO)
----------------------------------------
- profiles.json: Lưu trữ thông tin ví (Private Key), Token đăng nhập, địa chỉ ví của từng mail. 
  => CỰC KỲ QUAN TRỌNG, KHÔNG ĐƯỢC XÓA nếu muốn giữ ví cũ.
- account.txt: Lưu lại danh sách mail và pass đã đăng ký thành công.
- token.txt: Lưu Access Token để sử dụng cho các mục đích khác.
- last_index.txt: Lưu lại vị trí ví đang chạy để có thể chạy tiếp nếu tool bị ngắt.

5. CÁC CHỨC NĂNG CHÍNH CỦA TOOL
-------------------------------
- Tự động Đăng ký/Đăng nhập qua Email (Hỗ trợ Mail.tm lấy OTP).
- Tự động tạo ví EVM và liên kết DID (Decentralized ID).
- Tự động Bind mã mời (Ref) theo danh sách.
- DID Check-in: Điểm danh hàng ngày nhận +10 Point.
- Alive Check (Hệ thống kiểm tra sự sống): 
  + Subscribe dịch vụ.
  + Cấu hình Email Template cứu hộ.
  + Thực hiện Check-in nhận điểm Alive hàng ngày.
- Mở rương (Unbox): Tự động mở các loại Box 1, 5, 6 nếu có lượt.
- Chế độ ngủ (Auto Sleep): Sau khi chạy hết danh sách, tool sẽ tự tính toán thời gian và ngủ đến 07:00 sáng mai để tự động chạy lại vòng mới.

6. CÁCH CHẠY TOOL
-----------------
Mở Terminal/CMD tại thư mục chứa code và gõ:
node p2.js

--------------------------------------------------------------------------
LƯU Ý: Luôn kiểm tra file mail.txt và ref.txt trước khi chạy. 
Chúc các bạn cày cuốc thành công!
==========================================================================
Tham Gia NHóm tele : https://t.me/HVchannelss

Tham Gia Discor ( Vip ) : https://discord.gg/gKxvTNu5

Tham gia NHóm VIp Với Chi Phí 1 Tháng 4u - 15u 6thang Lợi ích tham gia nhóm ViP Sẽ được cấp keey sử dụng các tool vip trong discor hỗ trợ Và tham khao Code các tool dự án mà các bạn đề xuất

Gửi Phí tháng vào đây và chụp hình gửi trực tiếp cho tôi tại discor để xác nhận Role VIp ☕ https://huynhviet933.github.io/donate_viet_mmo/ Có thể tặng tôi ít cafe tại đây

Donenat : https://huynhviet933.github.io/donate_viet_mmo/
