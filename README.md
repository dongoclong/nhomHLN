# OOP-2021
Môn học Lập trình hướng đối tượng với Java
# Nhóm HLN
 ## Báo cáo tìm hiểu về mẫu thiết kế
 ## Thành viên: Họ và tên - MSSV
 ## 1. Đỗ Ngọc Long - 20021385
 ## 2. Cấn Mạnh Hùng - 20021364
 ## 3. Nguyễn Phúc Nguyên - 20021406

### **Cách thức thực hiện bài báo cáo**: Mỗi thành viên làm phần bài báo cáo của mình rồi commit vào reposition của nhóm ([Link reposition của nhóm]), bạn Đỗ Ngọc Long tổng hợp và sắp xếp phần báo cáo của các thành viên vào file báo cáo của nhóm.

 - **[Link đến reposition được sử dụng trong bài báo cáo] (https://github.com/Naphier/unity-design-patterns)**

## Abstract Factory:
-	Cung cấp một interface cho việc tạo lập các đối tượng (có liên hệ với nhau) mà không cần quy định lớp khi hay xác định lớp cụ thể (concrete) tạo mỗi đối tượng.
-	Giúp tránh được việc sử dụng điều kiện logic bên trong Factory Pattern. Khi một Factory Method lớn (có quá nhiều sử lý if-else hay switch-case), chúng ta nên sử dụng theo mô hình Abstract Factory để dễ quản lý hơn (cách phân chia có thể là gom nhóm các sub-class cùng loại vào một Factory).
-	Hãy lấy một hãng sản xuất ô tô làm ví dụ, chẳng hạn Hyundai. Họ có nhà máy, hoặc xưởng, chế tạo bánh xe: bánh của Azera, bánh của Sonata, bánh của Veloster, v.v… Đến lượt cửa xe, cũng có nhà máy chế tạo cửa Azera, cửa Sonata, cửa Veloster. Thân xe, động cơ, đèn, và các thành phần khác có những nhà máy chế tạo chúng.
-	Example: https://github.com/JangirSumit/abstract-factory-design-pattern .
```
	@@ -27,19 +28,43 @@ Môn học Lập trình hướng đối tượng với Java
			if(shapeType.equals("SQUARE")
				return new Square();
```
=> https://github.com/Naphier/unity-design-patterns/tree/master/Assets/abstract%20factory

## Factory Method:
-	Định nghĩa Interface để sinh ra đối tượng nhưng để cho lớp con quyết định lớp nào được dùng để sinh ra đối tượng Factory method cho phép một lớp chuyển quá trình khởi tạo đối tượng cho lớp con.
-	Factory method, đầy đủ là Factory method pattern, là thiết kế mẫu hướng đối tượng trong việc thiết kế phần mềm cho máy tính, nhằm giải quyết vấn đề tạo một đối tượng mà không cần thiết chỉ ra một cách chính xác lớp nào sẽ được tạo
-	Factory Pattern giúp giảm sự phụ thuộc giữa các module (loose coupling): cung cấp 1 hướng tiếp cận với Interface thay thì các implement. Giúp chuơng trình độc lập với những lớp cụ thể mà chúng ta cần tạo 1 đối tượng, code ở phía client không bị ảnh hưởng khi thay đổi logic ở factory hay sub class.
-	Thống nhất về naming convention: giúp cho các developer có thể hiểu về cấu trúc source code.
-	Example: https://github.com/iluwatar/java-design-patterns/tree/master/factory-method .
```
	public class BankFactory {
 
    private BankFactory() {
    }
 
    public static final Bank getBank(BankType bankType) {
        switch (bankType) {
 
        case TPBANK:
            return new TPBank();
 
        case VIETCOMBANK:
            return new VietcomBank();
 
        default:
            throw new IllegalArgumentException("This bank type is unsupported");
        }
    }
 
}
```
## Adapter:
-	Do vấn đề tương thích, thay đổi interface của một lớp thành một interface khác phù hợp với yêu cầu người sử dụng lớp.
-	Trong công nghệ phần mềm, Adapter pattern là một mẫu thiết kế tiếp hợp cho phép chuyển đổi một interface có sẵn thành một interface khác thích hợp cho lớp đang viết.
-	Tăng khả năng sử dụng lại thư viện với interface không thay đổi do không có mã nguồn.
-	Cho phép nhiều đối tượng có interface giao tiếp khác nhau có thể tương tác và giao tiếp với nhau.
-	bạn muốn sử dụng một lớp hiện có và giao diện của nó không khớp với một lớp bạn cần.
-	bạn muốn tạo một lớp có thể sử dụng lại hợp tác với các lớp không nhất thiết phải có giao diện tương thích.
- Example: https://github.com/Adapter-Hub/Hub .
```
package com.gpcoder.patterns.structural.adapter;
	@@ -56,6 +81,7 @@ public class JapaneseAdaptee {
## Bridge:
-	Tách rời ngữ nghĩa của một vấn đề khỏi việc cài đặt, mục đích để cả hai bộ phận (ngữ nghĩa và cài đặt) có thể thay đổi độc lập nhau.
-	Dạng thức bắc cầu là một dạng thức thiết kế được dùng trong công nghệ phần mềm. Dạng thức bắc cầu dùng để "tách riêng tính trừu tượng ra khỏi thực thể của nó để cho cả hai có thể thay đổi một cách độc lập".
-	Bridge Pattern được sử dụng để tách thành phần trừu tượng (abstraction) và thành phần thực thi (implementation) riêng biệt. Do đó, các thành phần này có thể thay đổi một cách độc lập mà không ảnh hưởng đến các thành phần khác. Thay vì liên hệ với nhau bằng quan hệ kế thừa, hai thành phần này liên hệ với nhau thông qua quan hệ “chứa trong” (object composition).
-	Example: https://github.com/MoienTajik/Bridge-Pattern-Sample .
```
	public interface Weapon {
	@@ -103,6 +129,7 @@ public class Account {
    }
}
```
=> https://github.com/Naphier/unity-design-patterns/tree/master/Assets/command%20pattern

## Observer: 
-	Định nghĩa sự phụ thuộc một-nhiều giữa các đối tượng sao cho khi một đối tượng thay đổi trạng thái thì tất cả các đối tượng phụ thuộc nó cũng thay đổi theo.
	@@ -117,8 +144,11 @@ public interface EventListener {
	void update(String eventType, File file);
}
```
=> https://github.com/Naphier/unity-design-patterns/tree/master/Assets/ObserverPattern/Example

## Buider:
+ Trong HouseBuilder.java khởi tạo lớp abstract HouseBuilder có chứa các phương thức abstract sử dụng mẫu thiết kế Fluent Interface Pattern trả về chính HouseBuider
+ đối tượng được tạo ra để xây dựng một đôi tượng phức tạp bằng cách sử dụng các đối tượng đơn giản và sử dụng tiếp cận từng bước, việc xây dựng các đối tượng đôc lập với các đối tượng khác.
```
  public abstract HouseBuilder addWalls();
  
	@@ -128,6 +158,7 @@ public interface EventListener {
 ``` 
+ Các lớp WoodHouseBuilder, StoneHouseBuilder, GingerbreadHouseBuilder kế thừa các thuộc tính trong lớp abstract HouseBuilder
=> Tách tiến trình xây dựng 1 đối tượng phức tạp sao cho một tiến trình tạo được các biểu diễn khác nhau => Builder Design Pattern
=> https://github.com/Naphier/unity-design-patterns/tree/master/Assets/builder%20pattern/example


## Kết luận: Trong dự án trên do nội dung là về design pattern nên mẫu thiết kế được sử dụng khá tương đồng với 23 mẫu thiết kế chuẩn.
