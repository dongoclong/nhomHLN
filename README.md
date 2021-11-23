# Nhóm HLN
 Báo cáo tìm hiểu về mẫu thiết kế
 ## Thành viên: Họ và tên - MSSV
 ## 1. Đỗ Ngọc Long - 20021385
 ## 2. Cấn Mạnh Hùng - 20021364
 ## 3. Nguyễn Phúc Nguyên - 20021406

### **Cách thức thực hiện bài báo cáo**: Mỗi thành viên làm phần bài báo cáo của mình rồi commit vào reposition của nhóm ([Link reposition của nhóm](https://github.com/dongoclong/nhomHLN)), bạn Đỗ Ngọc Long tổng hợp và sắp xếp phần báo cáo của các thành viên vào file báo cáo của nhóm.
 
 - **[Link đến reposition được sử dụng trong bài báo cáo] (https://github.com/sshahine/JFoenix/tree/master/demo)**
 - 
## Abstract Factory:
●	Cung cấp một interface cho việc tạo lập các đối tượng (có liên hệ với nhau) mà không cần quy định lớp khi hay xác định lớp cụ thể (concrete) tạo mỗi đối tượng.
●	Hãy lấy một hãng sản xuất ô tô làm ví dụ, chẳng hạn Hyundai. Họ có nhà máy, hoặc xưởng, chế tạo bánh xe: bánh của Azera, bánh của Sonata, bánh của Veloster, v.v… Đến lượt cửa xe, cũng có nhà máy chế tạo cửa Azera, cửa Sonata, cửa Veloster. Thân xe, động cơ, đèn, và các thành phần khác có những nhà máy chế tạo chúng.
●	Example: https://github.com/JangirSumit/abstract-factory-design-pattern .

## Factory Method:
●	Định nghĩa Interface để sinh ra đối tượng nhưng để cho lớp con quyết định lớp nào được dùng để sinh ra đối tượng Factory method cho phép một lớp chuyển quá trình khởi tạo đối tượng cho lớp con.
●	Factory method, đầy đủ là Factory method pattern, là thiết kế mẫu hướng đối tượng trong việc thiết kế phần mềm cho máy tính, nhằm giải quyết vấn đề tạo một đối tượng mà không cần thiết chỉ ra một cách chính xác lớp nào sẽ được tạo
●	Example: https://github.com/iluwatar/java-design-patterns/tree/master/factory-method .

## Adapter:
●	Do vấn đề tương thích, thay đổi interface của một lớp thành một interface khác phù hợp với yêu cầu người sử dụng lớp.
●	Trong công nghệ phần mềm, Adapter pattern là một mẫu thiết kế tiếp hợp cho phép chuyển đổi một interface có sẵn thành một interface khác thích hợp cho lớp đang viết.
●	Example: https://github.com/Adapter-Hub/Hub .

## Bridge:
●	Tách rời ngữ nghĩa của một vấn đề khỏi việc cài đặt, mục đích để cả hai bộ phận (ngữ nghĩa và cài đặt) có thể thay đổi độc lập nhau.
●	Dạng thức bắc cầu là một dạng thức thiết kế được dùng trong công nghệ phần mềm. Dạng thức bắc cầu dùng để "tách riêng tính trừu tượng ra khỏi thực thể của nó để cho cả hai có thể thay đổi một cách độc lập".
●	Example: https://github.com/MoienTajik/Bridge-Pattern-Sample .

## Command: 
●	Mỗi yêu cầu (thực hiện một thao tác nào đó) được bao bọc thành một đối tượng. Các yêu cầu sẽ được lưu trữ và gởi đi như các đối tượng.Đóng gói request vào trong một Object, nhờ đó có thể nthông số hoá chương trình nhận request và thực hiện các thao tác trên request: sắp xếp, log, undo…
●	Chúng ta có thể xử lí vấn đề theo hướng command - đóng gói ý tưởng, những action cần làm khi button được ấn hoặc menu item được chọn. Tức là gom code để xử lý việc ấn button hoặc chọn menu trong object riêng. Những action này chính là những commands của Command pattern.
● Example:	https://github.com/joshnh/Git-Commands .

## Observer: 
●	Định nghĩa sự phụ thuộc một-nhiều giữa các đối tượng sao cho khi một đối tượng thay đổi trạng thái thì tất cả các đối tượng phụ thuộc nó cũng thay đổi theo.
●	Trong bài toán đưa ra, ta có thể thấy rằng mối quan hệ 1-n ở đây đó là 1-WeatherData và n-Screen(currentConditionstDisplay,statisticsDisplay, ...). Mỗi khi WeatherData có sự thay đổi về trạng thái (nhiệt độ, độ ẩm, áp suất) thì nó sẽ "thông báo" cho các màn hình đang "quan sát" sát nó để cập nhật lại việc hiển thị thông tin.
●	Example: https://github.com/design-pattern-list/observer-pattern .

#Kết luận: Trong dự án trên do nội dung là về design pattern nên mẫu thiết kế được sử dụng khá tương đồng với 23 mẫu thiết kế chuẩn.







