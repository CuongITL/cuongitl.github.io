SafeGuard
===============

✨ SafeGuard's Crypto Bot! - Bot tự động đặt sl/tp theo % cài đặt sẵn, hoặc DCA lệnh theo %(nếu cho phép)


**🦅 Safety first, then profit will come.🍀**

`TÍNH NĂNG`
-------------------
💥 **Bot gồm có các thông số sau:**

 ``1. equity_protect(%):`` khi tổng toàn bộ lệnh bị âm vượt thông số này thì bot sẽ đóng hết lệnh.

 ``2. Break-Event:`` khi lệnh dương, bot tự động dời stoploss về entry+%
   - be_trigger(%): mặc định=0.9
   - be_protect(%): mặc định=0.4

   với thông số trên, khi lệnh dương >= 0.9% thì bot sẽ dời sl về mức entry+0.4%

 ``3. Stop-Loss(%):`` tự động cắt lệnh (sl) theo %giá hoặc theo %vốn vào lệnh
   - sl_percent: Mặc định = 0  - Tắt.
   - sl_by: percent hoặc margin, mặc định='margin'. Thông số này quyết định bot sẽ tính toán sl theo % giá cố định hoặc % của vốn lệnh hiện tại.

    Ví dụ với thông số như sau: sl_by: margin, sl_percent = 30%. Bạn vào lệnh 12$, khi lệnh bị âm -4$ (~30%) thì bot sẽ cắt lệnh này.

 ``4. Take-Profit(%):``
    - tp_percent: Mặc định = 10%

     Bot tự đặt tp ở mức entry+10%  với thông số trên.

 ``5. dca_percent(%):`` Mặc định = 0 - KHÔNG CHO PHÉP DCA.
    - multi: mặc định=1.5. Thông số này quyết định DCA có gấp thếp vốn không?
    - max_dca_per_day: mặc định=2. Số lần DCA trong 1 ngày.
    - minutes_between_dca: mặc định=59. Thời gian tối thiểu(theo phút) giữa 2 lần DCA.
    - max_margin($): khống chế vốn tối đa của 1 lệnh (dùng khi bật tính năng DCA). Mặc định = 50.

    Khi margin của 1 lệnh(vị thế) LỚN HƠN HOẶC BẰNG max_margin thì bot sẽ không nhồi lệnh (DCA) cho vị thế lện đó nữa.

 ``6. symbols_skip:`` bot sẽ bỏ qua các coin trong danh sách này.
 
Bên trên là các thông số cơ bản, ngoài ra còn một số thông số khác nhằm hạn chế rủi ro, không cho phép chỉnh.

👉  Nếu bạn ``giao dịch dưới ref`` của @Cuongitl sẽ được ``MIỄN PHÍ`` tất cả các loại bot tín hiệu.

 * Sàn Bitget: https://signal.lecuong.info/s/bg
 
 * Sàn Binance:  https://signal.lecuong.info/s/bnb


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
 
Ví dụ #2: Thay đổi phương thức sl là margin, %sl = 25%
 
 .. code-block:: console

   /guard sl_margin 25

Ví dụ #3: Thay đổi phương thức sl là price, %sl = 2%
 
 .. code-block:: console

   /guard sl_price 2

Ví dụ #4: Thay đổi break-event về tỷ lệ: trigger(bẫy) = 1%, bảo vệ ở mức: 0.5%
 
 .. code-block:: console

   /guard be 1 0.5

Ví dụ #5: Thêm coin LUNAUSDT vào danh sách loại trừ (không cần bot bảo vệ)
 
 .. code-block:: console

   /guard add LUNAUSDT


Ví dụ #6: Gỡ coin LUNAUSDT khỏi danh sách loại trừ.
 
 .. code-block:: console

   /guard remove LUNAUSDT


Danh sách thông số: 
---------------------

* equity_protect
* be
* max_margin
* sl_price
* sl_margin
* tp_percent
* dca_percent
* multi
* max_dca_per_day
* minutes_between_dca
* add
* remove
* help

 
Các thông số bảo vệ được lưu trữ trên hệ thống, bạn muốn thay đổi thì hãy chat với bot 
Telegram: |location_link|

.. |location_link| raw:: html

 <a href="https://t.me/Cuongitl_bot" target="_blank">@Cuongitl_bot</a>
