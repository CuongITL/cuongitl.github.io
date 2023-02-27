SafeGuard
===============

✨ SafeGuard's Crypto Bot! - Bot tự động đặt sl/tp theo % cài đặt sẵn, hoặc DCA lệnh theo %(nếu cho phép)


**🦅 Safety first, then profit will come.🍀**

💥 `Bot gồm có các thông số sau:`

 `1. equity_protect(%):` khi tổng toàn bộ lệnh bị âm vượt thông số này thì bot sẽ đóng hết lệnh.

 `2. Break-Event:` khi lệnh dượng, bot tự động dời stoploss về entry+%
 - be_trigger(%): mặc định=1.2
 - be_protect(%): mặc định=0.5

 `3. Stop-Loss(%):`
  - sl_percent: Mặc định = 35%
  - sl_by: percent hoặc margin, mặc định='margin' Thông số này quyết định bot sẽ cài sl theo % giá cố định hoặc % của vốn lệnh hiện tại.

 `4. Take-Profit(%):`
  - tp_percent: Mặc định = 5%

 `5. dca_percent(%):` Mặc định = 0 - KHÔNG CHO PHÉP DCA.
 - multi: mặc định=1.5. Thông số này quyết định DCA có gấp thếp vốn không?
 - max_dca_per_day: mặc định=2. Số lần DCA trong 1 ngày.
 - minutes_between_dca: mặc định=59. Thời gian tối thiểu(theo phút) giữa 2 lần DCA.
 - max_margin($): khống chế vốn tối đa của 1 lệnh (dùng khi bật tính năng DCA). Mặc định = 50.

  Khi Margin của 1 lệnh(vị thế) LỚN HƠN HOẶC BẰNG max_margin thì bot sẽ không nhồi lệnh (DCA) cho vị thế lện đó nữa.

 `6. symbols_skip:` bot sẽ bỏ qua các coin trong danh sách này.
===============
Bên trên là các thông số cơ bản, ngoài ra còn một số thông số khác nhằm hạn chế rủi ro, không cho phép chỉnh.

👉  Nếu bạn giao dịch dưới ref của @Cuongitl sẽ được miễn phí tất cả các loại bot tín hiệu.

 * Sàn Bitget: https://signal.lecuong.info/s/bg
 
 * Sàn Binance:  https://signal.lecuong.info/s/bnb
 

Các thông số bảo vệ được lưu trữ trên hệ thống, bạn muốn thay đổi thì hãy chat với bot Telegram: 
`<https://t.me/Cuongitl_bot >`_


`XEM`
-------------------

Để xem thông số bảo vệ của tài khoản:

.. code-block:: console
   /guard <tên-tài-khoản>

Ví dụ xem thông số bảo vệ của tài khoản tên là bitget_m1:
 
 .. code-block:: console

   /guard bitget_m1


`THAY ĐỔI`
-------------------

Để thay đổi thông số, sử dụng cú pháp: 

.. code-block:: console
   /guard <tên-thông-số> <giá-trị-mới>


`VÍ DỤ`
---------------------


Ví dụ #1: khống chế vốn nhồi lệnh tối đa khi DCA ở mức 50$
 
 .. code-block:: console

   /guard max_margin 50
 
Ví dụ #2: Thay đổi stoploss(%) bằng 25
 
 .. code-block:: console

   /guard sl_percent 25

Ví dụ #3: Thay đổi phương thức stoploss theo % vốn vào lệnh(margin), thay vì % giá so với entry.
 
 .. code-block:: console

   /guard sl_by margin


Ví dụ #4: Thêm coin LUNAUSDT vào danh sách loại trừ (không cần bot bảo vệ)
 
 .. code-block:: console

   /guard add LUNAUSDT


Ví dụ #5: Gỡ coin LUNAUSDT khỏi danh sách loại trừ.
 
 .. code-block:: console

   /guard remove LUNAUSDT


Danh sách thông số: 
---------------------

* equity_protect
* be_trigger,
* be_protect
* max_margin
* sl_percent
* sl_by
* tp_percent
* dca_percent
* multi
* max_dca_per_day
* minutes_between_dca
* add
* remove
* help
