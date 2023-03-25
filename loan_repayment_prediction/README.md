# Loan repayment prediction

Khoản vay trong ngân hàng chia ra làm các loại:

![Untitled](Loan%20repayment%20prediction%206835ae97fb1d41cc8ec281525a96048e/Untitled.png)

- Personal: vay tiêu dùng cá nhân
- Credit Card: thẻ ghi nợ
- Home: vay cho nhà cửa (khoản vay lớn)
- Small business: vay cho kinh doanh
- Auto
- Student

# 1. LOAN LIFECYCLE

![Untitled](Loan%20repayment%20prediction%206835ae97fb1d41cc8ec281525a96048e/Untitled%201.png)

![Untitled](Loan%20repayment%20prediction%206835ae97fb1d41cc8ec281525a96048e/Untitled%202.png)

![Untitled](Loan%20repayment%20prediction%206835ae97fb1d41cc8ec281525a96048e/Untitled%203.png)

Có nhiều mô hình để making predictions, tùy thuộc vào dữ liệu và bài toán như thế nào mà ta sử dụng model cho phù hợp:

![Untitled](Loan%20repayment%20prediction%206835ae97fb1d41cc8ec281525a96048e/Untitled%204.png)

# Demo sử dụng python

Hướng đi:

- import dataframe vào
- view dataframe xem có các cột nào, giá trị của các cột như nào, có hàng nào bị NaN ⇒ xử lý NaN
- Xem label của data xem có bị imbalance giữa các class hay không
- Tiền xử lý dữ liệu
    - Xem xét các cột có dữ liệu không phải dữ liệu số, chuyển nó về dữ liệu số
    - Kiểm tra xem có cột nào bất thường ( dữ liệu quá lệch hoặc chỉ có 1 giá trị ⇒ không cần thiết)
    - Kiểm tra dữ liệu đầu vào có độc lập tuyến tính với nhau không (check bằng corrrelation matrix)- Nếu corre cao vượt quá 0.6 ⇒ cần phải xử lý, bỏ cột nào đó đi
    - Scaling dữ liệu về cùng khoảng 0-1 để mô hình hội tụ nhanh hơn (scale input)
- Chia data ra train, test
- Chọn model để training. Lưu ý về việc imbalanced data khi chọn model