# bof1
Bài khởi đầu cho chuyên mục học PWNABLE là 1 bài Buffer Overflow !
Dịch file "bof1" sang code C bằng IDA 
![image](https://github.com/hieubmt1112004/bof1/assets/125638408/7eb31313-0dcd-4ac8-8634-1a67e475a7ea)
ta thấy hiện tại biến buf được chỉ định 16 byte, còn v5,v6,v7 đang rỗng 
![image](https://github.com/hieubmt1112004/bof1/assets/125638408/ad9d350f-bd1d-43a6-863e-4164eedfc4d8)
tiếp theo :
![image](https://github.com/hieubmt1112004/bof1/assets/125638408/84e7802c-5952-48d1-9fcf-e7ae086311f1)
đoạn code này đang thể hiện giá trị ban đầu trước khi được nhập vào của biến buf là 0 byte và giá trị max của biến buf là 48byte
Tiếp theo Debug file bof1 :
+  Ni cho tới hàm read !
+  bước tiếp theo tạo 1 chuỗi kí tự để check lỗi của bài bằng lệnh pattern creat !
![image](https://github.com/hieubmt1112004/bof1/assets/125638408/264536a0-23fe-484d-9141-ef443db2fe65)
+  Dán chuỗi kí tự và kiểm tra
+  ![image](https://github.com/hieubmt1112004/bof1/assets/125638408/eac73b3a-68c5-4254-980f-ef871f4fe601)
+  ta dễ dàng thấy các chuỗi kí tự bị tràn từ trên xuống tương ứng với mỗi địa chỉ của biến 
 
 




