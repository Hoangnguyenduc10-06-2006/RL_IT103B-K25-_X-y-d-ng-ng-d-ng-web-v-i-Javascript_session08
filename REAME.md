lỗi 1 : do mã nguồn cũ sử dụng sử dụng lệnh pop() 
=>>> nên dẫn đến thứ tự các xe đến sạc bị sai vì pop() nó lấy ra phần tử cuối 
cùng của mảng 
giải quyết: thay pop() bằng shift() vì shif laayys phần từ đầu tiên của mảng 

lỗi 2: dùng điều kiện  dừng i <= completedSessionsKwh.length nên là sẽ gây ra lỗi vì nó sẽ gi nhận
1 phần từ ko có trong mảng thứ tự sẽ là 01234 nhưng thực tế ra chỉ cần 0123 đại diện có 4 element

giai pháp là thay đổi đièu kiện dừng i < completedSessionsKwh.length

kiểm thừ 

trường hợp: Điều phối xe vào sạc theo hàng đợi
đầu vào : waitingQueue = ['29A-112.33', '30E-889.12', '51K-678.99']
kết quả sai: Xe được điều phối vào sạc: 51K-678.99
kết quả đúng: Xe được điều phối vào sạc: 29A-112.33


trường hợp: Tính tổng sản và doanh thu ca trực
đầu vào :   completedSessionsKwh = [45.2, 30.5, 62.8, 28.0]
            fastChargingRate = 4500
kết quả sai:    Tổng sản lượng: NaN kWh
                Tổng doanh thu: NaN VNĐ
kết quả đúng:   Tổng sản lượng: 166.5 kWh
                Tổng doanh thu: 749250 VNĐ